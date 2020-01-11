title: Lokiドキュメンテーション | Lokinet Linuxインストールガイド | オニオンルーティング
description: このガイドで、耐シビル攻撃性を持つオニオンルーターのLokinetをLinuxでインストールして使えるようになります。

# LokiNETインストールガイド　-　Linux
著者：Jason (jagerman), Johnathan (SonOfOtis)

ソース: [https://deb.imaginary.stream/](https://deb.imaginary.stream/)

## Linuxでの設定方法

### 1. パソコン準備
先ずはパッケージリストをアップデートすることを強くお勧めします。以下のコマンドはリポジトリーからパッケージリストをダウンロードし、最新バージョンやその依存関係についての情報をアップデートします。全てのリポジトリーとPPAはそのようにアップデートされます。

以下のコマンドを実行します：

```
sudo apt-get update
```

様々なパッケージリストがダウンロードされたことに気付くでしょう。ダウンロードは完了したら、以下のコマンドでシステムに現在インストールされるパッケージのアップデートをフェッチしてください。

```
sudo apt-get upgrade
```

ディスク領域使用を許可するよう求められます。許可するのに、「y」を入力してエンター・キーを押します。

>注意：利用可能なバージョンのダウンロードを求められたなら、パッケージメンテナのバージョンを選択できるまで上下の矢印キーを押し、そしてエンター・キーを押します。

後でcurlを使いますので、パソコンにインストールされていない場合は今すぐインストールしましょう：

```
sudo apt install curl
```

### 2. インストール方法

このステップは最初にリポジトリーを設定する時のみです。それ以降、システムアップデートをする時にリポジトリーは自動的にアップデートされます。

Lokiの'apt'リポジトリーを追加するため、以下のコマンドを実行してください：

このコマンドで、バイナリ実行ファイルを署名したJagermanさんの公開キーをインストールします。

```
curl -s https://deb.imaginary.stream/public.gpg | sudo apt-key add -
```

次のコマンドは'apt'がパッケージを見つけれるようにします：

```
echo "deb https://deb.imaginary.stream $(lsb_release -sc) main" | sudo tee /etc/apt/sources.list.d/imaginary.stream.list
```

> このdebは認識されない場合、[トラブルシューティング](#troubleshooting)を調べて下さい。

そしてパッケージリポジトリーを再シンクロします：

```
sudo apt update
```
次はlokinetをインストールします：

```
sudo apt install lokinet
```

おめでとうございます、Lokinetはインストールされバックグラウンドに実行されています。

SNAppをアクセスするのに、SNAppアクセスガイドを[ここ](../PublicTestingGuide/#2-accessing-snapps)から調べて下さい。

次のステップでは、手入力でlokinetをスタートおよび停止する方法を教えます。

--- 

## lokinetをスタートおよび停止する方法

手入力でlokinetをスタートするのに、以下のコマンドを実行します：

```
sudo systemctl start lokinet
```

そしてlokinetを停止するのに、以下のコマンドを実行します：

```
sudo systemctl stop lokinet
```

---

## トラブルシューティング

### ブートストラップRC解読失敗

ブートストラップは正しく設定されていないようにみえる場合、以下のコマンドを実行します：

```
sudo lokinet-bootstrap
```

そしてlokinetを再起動します

```
sudo systemctl restart lokinet
```


### (lsb-release)はLinux Mintで正常に機能しません

Linux Mintユーザは、[2. インストールする仕方](#2-installation)にある第2のコマンドの代わりに、以下のコマンドで上手くインストールできると思われます：

```
echo "deb https://deb.imaginary.stream bionic main" | sudo tee /etc/apt/sources.list.d/imaginary.stream.list
```

### DNSの設定

.lokiアドレスの変換には問題がある場合、resolv.confファイルを編集してDNSリゾルバを追加する必要があります。

#### メソッド１

以下のコマンドを実行します：

```
apt install resolvconf
```

そしてlokinetを再起動します：

```
systemctl restart lokinet
```

#### メソッド２
メソッド１が上手く行かない場合、手入力でネームサーバーを追加する必要があります。

以下のコマンドを実行します：

```
sudo nano /etc/resolvconf/resolv.conf.d/head
```

以下をファイルの最後に追加します：

```
nameserver 127.3.2.1
```

追加されたら、コントロールキーを押しながらXキーを押します。
ファイル変更を確認するため、エンターキーを押します。

次は、以下のコマンドで/etc/resolv.confファイルをアップデートする必要があります：

```
sudo resolvconf -u
```

そしてlokinetを再起動します：

```
systemctl restart lokinet
```

--- 

## Lokinetをアップデートします


手入力でlokinetをアップデートするのに、以下のコマンドを実行します：

```
sudo apt update && sudo apt install lokinet && sudo lokinet-bootstrap && sudo systemctl restart lokinet
```

---


## 完了

おめでとうございます。ガイドをクリアしました。ここから[Lokinetパブリックテストのガイド](../PublicTestingGuide/#2-accessing-snapps)へ戻りましょう。
