title: Lokiドキュメンテーション | よくある質問


description: Lokiとは？　Lokiにはマスターノードはありますか？　セッションとは？　「Lokiよくある質問ページ」は、Lokiプロジェクトがよくある質問にお答えます。

# よくある質問

## 一般的な質問

* [Lokiとは？](#what-is-loki)

* [Lokiはプルーフ・オブ・ワーク (PoW)あるいはプルーフ・オブ・サービス (PoS)ですか？](#is-loki-proof-of-work-pow-or-proof-of-service-pos)

* [トークン供給とは何ですか？](#what-is-the-token-supply)

* [モネロのやり方と比べて何が違いますか？](#what-do-you-do-differently-from-monero)

* [どのような人達がLokiネットワークを使うのですか？](#who-would-use-loki-network)

* [LokiはERC20トークンですか？](#is-loki-an-erc20-token)

* [Lokiという名前を選んだ理由は何ですか？](#why-the-name-loki)

* [このP2Pネットワークの背景にあるビジネスモデルは何ですか？](#what-is-the-business-model-behind-this-peer-to-peer-network)

* [モネロのソースコードへお返しにコミットするつもりはありますか？](#will-you-guys-commit-back-to-the-monero-source-code)

* [モネロと何が違いますか？](#whats-the-difference-from-monero)

* [プレマインについての詳細を教えてもらえますか？](#can-i-see-details-about-the-premine)

* [どうして5%のガバナンス報酬があるのですか？](#why-is-there-a-5-governance-reward)

* [マイニングのブロック報酬とは何ですか？](#what-is-the-block-reward-for-mining)

* [ブロック生成時間とは何ですか？](#what-is-the-block-generation-time)

* [LokiはLedger Nano Sのハードウェアウォレットでサポートするつもりですか？](#are-there-plans-to-support-loki-on-the-ledger-nano-s-hardware-wallet)

---

## サービスノード

* [どうしてサービスノードが必要なのですか？](#why-are-service-nodes-required)

* [Lokiにはマスターノードという概念はありますか？](#is-there-a-concept-of-masternodes-in-loki)

* [サービスノードを運営するための担保要件とは何でしょうか？](#what-is-the-collateral-requirement-to-run-service-nodes)

* [1つのVPSサーバーで複数のサービスノードを運営可能ですか？](#can-you-run-multiple-service-nodes-in-a-single-vps-server)

* [プールメンバーはステークをアンロックすることを要求できますか？](#can-a-pool-member-request-for-the-stake-to-be-unlocked)



---
## セッション


---

## SNApp

* [SNAppはサービスノードのみで運営されますか？](#do-snapps-run-on-service-nodes-only)

* [SNAppはDAppのようなものですか？](#are-snapps-like-dapps)

* [SNAppとそのデータのホスティングはどこですか？](#where-will-snapps-and-all-of-its-data-be-hosted)

---

## Lokiサービス

* [Lokiメッセンジャーとは？](#whats-loki-messenger)

---

一般的な質問
---

###**Lokiとは？**

Lokiはユーザーに匿名の、分散的で、安全な、そしてプライベートにオンラインで交流するためのツールを提供します。Lokiはプライベート取引ネットワーク、仮想通貨$LOKI、そして財政的に奨励された[サービスノード](../ServiceNodes/SNOverview)の結合で、[Lokinet](../Lokinet/LokinetOverview)という管理者の存在しない定足数に基づく混合ネットワークを創設することができます。[Lokiメッセンジャー](../LokiServices/Messenger)という分散的、匿名、そしてプライベートなメッセンジャーサービスもLokinetに組み込まれています。[サービスノードアプリ](../Lokinet/SNApps) (SNApps)と呼ばれるフロントエンドアプリケーションはLokinet上で作動してブラウザとの統合及びオープンソースコミュニティーからの貢献を可能とします。

###**Lokiはプルーフ・オブ・ワーク (PoW)あるいはプルーフ・オブ・サービス (PoS)ですか？**

Lokiは[プルーフ・オブ・ワーク](https://ja.wikipedia.org/wiki/%E3%83%97%E3%83%AB%E3%83%BC%E3%83%95%E3%83%BB%E3%82%AA%E3%83%96%E3%83%BB%E3%83%AF%E3%83%BC%E3%82%AF%E3%82%B7%E3%82%B9%E3%83%86%E3%83%A0) と[プルーフ・オブ・サービス](../ServiceNodes/SNOverview)のハイブリッドを利用しています。DASHと同様に、PoWによって保護され、マスターノードへの報酬はプルーフ・オブ・サービスに管理されます。

###**トークン供給とは？**

モネロと同じように、トークンの総供給はありません。現在の供給は[lokiblocks.com](https://lokiblocks.com) で見つけることができます。

###**モネロとの違いは？**

中核通貨へのアプローチにわずかな変化以外に、多様な機能を果たす[サービスノード](../ServiceNodes/SNOverview)ネットワークを実行します。その機能は[匿名ネットワーク層](../Lokinet/LLARP)、[Blink](../LokiServices/Blink)というシステムによって管理者が存在しない定足数に基づく瞬間取引、そして例えば[プライベート・メッセージング](../LokiServices/Messenger)を確保するなどのためにネットワーク層を活用する様々な機能を含みます。

###**どんな人達がLokiネットワークを使いますか？**

Lokiはプライベートな取引、そして通信機能を与えますので、そのユースケースはコミュニケーションに関する最高のプライバシーが欲しい方々に訴えかけることでしょう。[SNApp](../Lokinet/SNApps)開発の拡大につれて、Lokiはプライバシー中心のアプリケーションが実行する理想のネットワークに発展すると思われます。

###**LokiはERC20トークンですか？**

いいえ、LokiはERC20トークンではありません。自身でコインをマイニングしており、Loki自体がmainnetなのです。[lokiblocks.com](https://lokiblocks.com) をご覧ください。

###**なぜLokiという名前なんですか？**

Loki(ロキ)は、古期ノルド神話に登場する悪戯好きの神です。我々はいろんなデジタル「悪戯」を使用してトランザクション・データを難読化するからこそ、そういう神に因んで名付けるのはふさわしいと言えるでしょう。その上、ネットワーク上のトランザクションや通信は「low-key(低姿勢)」だから言葉遊びとして二重の意味を持ちます。

###**このP2Pネットワークの背景にあるビジネスモデルは何ですか？**

Lokiはネットワークによって提供される奨励構造に基づいて作動しています。ピアツーピア通信はすでに奨励されているサービスノードを介してのみ送られますので、さらなるビジネスモデルを提供する動機が薄いです。Loki財団の立ち上げる後のビジネスモデルは中核Lokiサービスの開発を続けること、そしてサービスノードで運用される第三者SNAppの開発を支援することです。

###**モネロのソースコードへお返しにコミットするつもりはありますか？**

最適化、バグ修正、新機能などの役立つ変更をお返しにモネロに提供するつもりです。

###**モネロと何が違いますか？**

最小10 mixinの[一定リング署名サイズ](/Advanced/CryptoNoteElements/#ring-signature-size)、[コミュニティープロジェクトや開発を財政支援する](/Governance/LokiFundingSystem)5%の[ガバナンスブロック報酬](/Advanced/Cryptoeconomics/#block-reward-split)、そして[通貨発行速度曲線(emission curve)](/Advanced/Cryptoeconomics/#loki-block-reward)の変更。Lokiをモネロと区別しているベースレイヤー変更はありますが、主な違いは第2レイヤーの奨励されてる[サービスノード](../ServiceNodes/SNOverview)、[Lokiサービス](/LokiServices/LokiServicesOverview)、そして[Lokinet](../ServiceNodes/SNOverview)です。

###**プレマインについての詳細を知ることはできますか？**

はい、[プレマイン報告書](https://loki.network/loki-premine-report/) をご覧ください。

###**どうして5%のガバナンス報酬がありますか？**

ユーザーが開発の資金調達は外力によって悪影響を与えられないという確信があるように、[自己資金によるシステム](../Governance/LokiFundingSystem)を作る意向です。5%ブロック報酬はそのためにガバナンス・ウォレットへ送られます。

他のプロジェクトと似たような方法です。例えば、始めの4年間20%ブロック報酬をもらうZCash財団、あるいはネットワークから10%ブロック報酬をもらうDASHプロジェクト。

ブロック報酬の割合をZCashとDASHよりもかなり低くしたいですが、同様にプロジェクトを無制限かつ十分に継続できるようにしたいと思います。

今後は、コミュニティーに対する報酬が高すぎる、低すぎる、もしくは不必要と判断する場合に、ハードフォークによってブロック報酬の配分条件を変更できるでしょう。

###**マイニングのブロック報酬とは何ですか？**

正確なブロック報酬情報を[www.lokiblocks.com](https://www.lokiblocks.com) で入手できます。ブロック報酬の配分は以下のように計算されます：サービスノードへ50%、マイナーへ45%、そしてガバナンス・プールへ5%。ブロック報酬の配分について、詳しくは[ここ](../Advanced/Cryptoeconomics/#block-reward-split)から。

###**ブロック生成時間はどれ程かかりますか？**

だいたい120秒程度です。

###**LokiはLedger Nano Sのハードウェアウォレットでサポートするつもりはありますか？**

はい。現在、準備中です。

---

サービスノード
---

###**どうしてサービスノードが必要なのですか？**

[サービスノード](../ServiceNodes/SNOverview)は新たなガーリックルーティング技術を使用する匿名ネットワーク形成を可能にする第2レイヤーのネットワークを形成します。サービスノードは[Lokinet](../Lokinet/LokinetOverview)と呼ぶ一般化ミックスネットを介するデータのルーティングを行います。[SNApp](../Lokinet/SNApps)はこのノードネットワークによって可能にされるユーザに向いてるフロントエンドのアプリケーションです。SNAppはブロックチェーン上に実行しませんが、ブロックチェーンの合意ルールに頼ってサービスノードの動作を施行します。つまり、SNAppはブロックチェーンのスケーラビリティに影響を与えません。サービスノードはブロックのマイニングをしませんが、フルノードと同じようにブロックを認証して伝搬します。

###**Lokiにはマスターノードという概念はありますか？**

はい。Lokiでは[サービスノード](../ServiceNodes/SNOverview)と呼ばれます。

###**サービスノードを運営するための担保要件とは何でしょうか？**

初期要求は4万5千$LOKIですが、時間をかけて下方修正するつもりです。最大4人までのプールも許可されます。担保要件について詳しくは[ここから](../ServiceNodes/StakingRequirement)。

現在の要求を調べるのに、ここから[担保電卓](https://jagerman.com/sn/) を見て下さい。シングルノードを実行することができて、またはプールノードと参加することもできます。シングルノードの場合、100%の担保を差し入れる必要があります。プールノードの場合、1人を除いた全メンバーは少なくとも25％の担保を差し入れる必要が発生します。サービスノードについて詳しくは、[サービスノードポータル](https://loki.network/service-nodes-portal/) をチェックして下さい。

###**1つのVPSサーバーでは複数のサービスノードを運営できますか？**

各[サービスノード](../ServiceNodes/SNOverview)を別のインスタンスとして実行することをお勧めしますが、必要条件ではありません。

###**プールメンバーはステークのアンロックを要請できますか？**

プールノードの場合、メンバーがステークのアンロックを要請する際、サービスノードは停止が予定されるでしょう。

---

SNApp
---

###**SNAppはサービスノードのみで運営されますか？**

[SNApp](../Lokinet/SNApps)をアクセスすると、データは様々なサービスノードを介することによって難読化されます。しかしながら、Torの（Hidden)秘匿サービスと同じようにSNAppそのものはあるサーバーにホストされ、クライアント側で算出されます。

###**SNAppはDAppのようなものですか？**

コア関数が「分散的」だという意味では、[SNApp](../Lokinet/SNApps)はDAppと似てますが、オンチェーンの実行や算出に頼りません。全てのSNAppはクライアント側で算出され、ネットワーキングはオフチェーンで[サービスノード](../ServiceNodes/SNOverview)ネットワークによって処理されます。

###**SNAppとそのデータのホスティングはどこですか？**

[SNApp](../Lokinet/SNApps)はTorの秘匿サービスと同じ様にユーザーによって個人サーバーにホストされます。

---

Lokiサービス
---

### **セッションとは？**

[セッション](../LokiServices/Messenger)は分散的、終端間暗号化されるメッセンジャーサービスです。内容の秘密性を確保するためのメッセージを送るプラットフォームを提供するアプリケーションはすでに存在しますが、その様なアプリは政府や第三者に狙われやすい集中型サーバーに頼ります。公開/秘密鍵暗号方式とLokiネットワーク上の[サービスノード](../ServiceNodes/SNOverview)アーキテクチャを利用して、Signalと似たようなサービスを提供することができます。セキュアなメッセンジャーアプリに加えて、分散化とネットワーク匿名性から付加価値が得られます。
