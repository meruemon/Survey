## テキストベース関連
- [x] **An Analysis of French-Language Tweets About COVID-19 Vaccines: Supervised Learning Approach(2022)**  
   [[link]](https://medinform.jmir.org/2022/5/e37831)
   BERTを用いてワクチンツイートの分類ができるか検証．
   <details><summary>概要</summary><div>
    ワクチン関連のツイートの特徴として，賛成反対いがいにも，曖昧，皮肉，無関係といったツイートが多くありこれらもうまく分類できるかどうかを検証．CamemBERT というフランス語BERTモデルを微調整して使用．ツイートは，(1) 賛成 反対 中立， (2) コンテンツの種類 (科学的，政治的，社会的，またはワクチン接種の状況) に分類．(1)の分類は困難，(2)の分類は(1)よりかは高いがまずまずの結果に．そこで，ツイート本文が170文字以上のものに限定して再度実験を行うと，結果が改善された．コメント：ツイートのラベル参考になりそう．ちなみにラベル付けは手動で行っていた．
--- 
- [x] **Hate Speech Detection Using Static BERT Embeddings(2021)**  
   [[link]](https://link.springer.com/chapter/10.1007/978-3-030-93620-4_6#citeas)
   ヘイトスピーチ検出で，他の自然言語処理で得られた埋め込みをBERTに置き換えることを提案
   <details><summary>概要</summary><div>
   ETHOSヘイトスピーチ検出データセットを使用し，単語埋め込み(fastText(FT)，GloVe(GV)，またはFT+GVをBERT埋め込みで置き換えまたは統合することによって，ヘイトスピーチ検出分類器のパフォーマンスを分析．実験の結果，単語埋め込みとしてFT，GV，またはFT+GVを使用する場合と比較して，BERTを使用した場合の方がパフォーマンスが優れていることを確認．
--- 
- [x] **A BERT-Based Transfer Learning Approach for Hate Speech Detection in Online Social Media(2019)**  
   [[link]](https://arxiv.org/abs/1910.12574)
   BERTを用いてヘイトスピーチ検出を行う
   <details><summary>概要</summary><div>
   BERTベースのヘイトスピーチ検出の先駆けになるような研究．ヘイトスピーチ検出にBERTに基づく新しい転移学習アプローチを導入．特に，転移学習に基づく新しい微調整方法を使用して，ソーシャルメディアコンテンツ内の憎悪に満ちたコンテキストをキャプチャするBERTの機能を調査．提案したアプローチを評価するためにTwitterの公に利用可能なデータセットを使用した実験結果では，このソリューションが既存のアプローチと比較して，精度とリコールの点でかなりのパフォーマンスを得ることを示した．
--- 
- [x] **Hate speech detection and racial bias mitigation in social media based on BERT model(2020)**  
   [[link]](https://arxiv.org/abs/2008.06460)
   BERTを用いたヘイトスピーチ検出と，訓練セットにおけるバイアスの影響を緩和するためのバイアス緩和メカニズムの導入
   <details><summary>概要</summary><div>
   先程の「BERTを用いたヘイトスピーチ検出」の改善手法．訓練された分類器から生じるバイアスについて問題視．まず，BERTと呼ばれる既存の事前訓練済み言語モデルに基づくヘイトスピーチ検出のための転移学習アプローチを導入し，Twitter上の人種差別，性差別，憎悪または攻撃的なコンテンツに注釈を付けた2つの公に利用可能なデータセットで提案モデルを評価．次に，ヘイトスピーチ検出タスクにおけるバイアス緩和メカニズムを導入して，事前訓練済みBERTベースモデルの微調整中に訓練セットにおけるバイアスの影響を緩和した手法を提案．
--- 
- [x] **Assessing the Impact of Contextual Information in Hate Speech Detection(2022)**  
   [[link]](https://ieeexplore.ieee.org/abstract/document/10076443)
   ヘイトスピーチ検出において，コンテキスト情報(返信情報)などを含める有効性を検証
   <details><summary>概要</summary><div>
   コンテキスト情報を持つことの重要さを評価するために，提案されたモデルに対して3つの異なるタイプの入力を検討．1)コンテキストを持たないコメント(None)，2)コンテキストとして返信されたツイートを持つコメント(Tweet)，3)返信されたツイートとニュース記事のテキストを持つコメント(Full)．ヘイトスピーチか否かの2値分類と，ヘイトスピーチの中の更に細かい分類まで行う多クラス分類の2つのタスクを行い，コンテキストによって2値分類では中程度の改善が見られ，多クラス分類ではより大幅な改善が見られた．
--- 
- [x] **Detection of Hate Speech using BERT and Hate Speech Word Embedding with Deep Model(2023)**  
   [[link]](https://www.tandfonline.com/doi/full/10.1080/08839514.2023.2166719)
   ヘイトスピーチ検出において，意図的なスペルミスや略語に対応するため，ドメイン固有の単語表現を用いた手法の提案
   <details><summary>概要</summary><div>
   ヘイトコミュニティは検出を回避するためにコミュニケーションにおいて略語，意図的なスペルミス，暗号化された単語を使用する傾向があり，ヘイトスピーチ検出タスクにさらなる課題があると指摘．論文では，特徴としてのドメイン固有の単語埋め込みとヘイトスピーチを自動的に検出するための分類器としての双方向性LSTMベースのディープモデルを利用することの実現可能性を検討．実験の結果，双方向性LSTMベースのディープモデルを用いたドメイン固有の単語埋め込みは93%のf1スコアを達成，BERTは利用可能なヘイトスピーチデータセットからの結合されたバランスのとれたデータセットで96%のf1スコアを達成．現在のSNSドメイン固有のコンテンツから大規模な事前訓練済みモデルを構築することは非常に有用と結論付けた．
---
## グラフベース関連
- [x] **Prediction of COVID-19 tweeting: classification based on graph neural networks(2022)**  
   [[link]](https://ieeexplore.ieee.org/abstract/document/9803426)
   GNNに基づく新型コロナウイルス感染症ツイート予測
   <details><summary>概要</summary><div>
    あるユーザが，今後コロナ関連のツイートをするかどうかを予測するモデルを構築．特に，node2vecを使用し，ユーザのフォロワーネットワークから抽出された特性のベクトルとしてユーザをモデル化している．
---
- [x] **Graph Contrastive Learning with Augmentations(2021)**  
   [[link]](https://arxiv.org/abs/2010.13902)
   GNNの対照学習
   <details><summary>概要</summary><div>
    対照学習の概念をGNNに適用．Graph Contrastive Learning（GCL）としている．グラフにおける不変表現の学習を促進させることが目的であり，実験により汎化性と頑健性が示された．拡張に関してはノードやエッジの削除，追加などが挙げられており，もう少し検討が必要な模様
---
- [x] **Local discriminative graph convolutional networks for text classification(2023)**  
   [[link]](https://link.springer.com/article/10.1007/s00530-023-01112-y)
   GNN 局所的大域的の両方から学習を行う
   <details><summary>概要</summary><div>
    従来のテキスト分類GNNの問題点として，正解ラベルと予測ラベルの適合度にのみ着目している点が挙げられる．つまり，グラフが暗黙的に符号化する局所的なクラス内多様性と局所的なクラス間類似性を無視しているといえる．テキスト分類の精度をより向上させるためには，クラス内とクラス間の両方の多様体構造を考慮することが重要となっている．そこで本論文では局所識別グラフ畳み込みネットワーク(LDGCN)を提案する．テキストデータの局所クラス間散布行列と局所クラス内散布行列を構築し，新しいLDGCNの特徴空間では，同じクラスのテキストは互いに密接にマッピングされ，異なるクラスのテキストはできるだけ離れてマッピングされるよう学習を行う．
---
- [x] **Graph Attention Networks(2017)**  
   [[link]](https://arxiv.org/abs/1710.10903)
   GNNにおける畳み込みにおいてAttentionの機構を組み込む．
   <details><summary>概要</summary><div>
    GCNにおける畳み込みで，近傍ソースノードの重要性を推定するAttention演算子，近傍ソースノードの情報を抽出するMessage演算子，Attention演算子とMessage演算子の積から全近傍情報を集約するAggregate演算子の計3つの演算子から，各近傍ソースノードのAttentionを考慮した学習を行い，重要なソースノードの情報をより集約するようなメカニズムを確立．
---
- [x] **Towards more robust hate speech detection: using social context and user data(2023)**  
   [[link]](https://link.springer.com/article/10.1007/s13278-023-01051-6)
   ヘイトスピーチ検出において，テキスト情報に加えユーザ情報などを加えたフレームワークを提案
   <details><summary>概要</summary><div>
   ヘイトスピーチのニュアンスをより良く捕捉し検出精度を改善するために，投稿者のテキスト，社会的コンテキスト及び言語的特徴を取り入れる．ヘイトスピーチを検出するためにテキスト内容と社会的コンテキストを組み合わせたフレームワークを提案．具体的には，変分グラフオートエンコーダ(VGAE)を使用してソーシャルネットワーク，テキスト，およびプロフィール情報を使用して投稿者の統一された特徴を共同で学習．この方法を2つの多様なTwitterデータセットで評価し，既存の最先端の方法よりも大幅に優れていることを示した．つまり，ヘイトスピーチ検出にコンテキスト情報を考慮する有効性を示した．
---
## 異種グラフ関連
 - [x] **GraphBERT: Bridging Graph and Text for Malicious Behavior Detection on Social Media(2022)**  
   [[link]](https://ieeexplore.ieee.org/document/10027673)
GNNとBERTを組み合わせて，悪質ツイートの検出
   <details><summary>概要</summary><div>
   ツイートの情報(ハッシュタグやエンティティなど)を，ツイートノードと情報ノードでエッジを形成し異種グラフで表現．これでグラフベースの関係情報を得る．この情報とBERTを組み合わせて悪質ツイート，ユーザの分類を行う．BERT単体，またはBERT+CNN や BERT+LSTMの手法よりも良い結果に．つまり，GNNから有用な構造情報を取得できているということに
---
- [x] **COVID-19 patients classification using Graph neural network on a Heterogeneous graph(2020)**  
   [[link]](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE10506109)
   [[github link]](https://github.com/KienMN/COVID-19-in-Korea-graph)
   異種グラフを用いてコロナ患者の分類を行う．
   <details><summary>概要</summary><div>
   コロナ患者と，患者の住む市，市のある県などをノードとして異種グラフを作成．GNNより患者の感染症例を分類．複雑なアプローチを施したが結果は改善されず．つまり，今回作成した異種グラフではニューラルネットワークの学習が困難だった．原因としてはクラスの不均衡さ，不十分な特徴量が考えられる．感染者の居住地情報が感染症例の分類に役立つと考えていたが，その情報のみでは不十分だった模様．データセットの改善や強力なGNNが解決策となると考えられる．
---
- [x] **Detecting Political Opinions in Tweets through Bipartite Graph Analysis: A Skip Aggregation Graph Convolution Approach(2023)**  
   [[link]](https://arxiv.org/abs/2304.11367)
   ツイートとユーザをノードとすグラフにGNNを適用する際，スキップ集約メカニズムを用いてユーザ特徴量問題を解消する
   <details><summary>概要</summary><div>
    ツイート中の政治的意見を検出するために，ユーザーの投稿とリツイートの行動に基づいてユーザーとツイートの二部グラフを構築し，GNNベースのノード分類問題に変換する．GNNを適用する際，ツイート表現を学習するために，新しいスキップ集約メカニズムを提案する．グラフを構築する際，ツイートノードはBERTを用いて初期特徴量を設定することができるが，ユーザノードはテキストではないため初期特徴量を設定することができない．そこで，ツイート表現を学習する際に2近傍先のノード，つまりユーザノードをスキップしたツイートノードの特徴量から学習を行うことで，先ほどの問題を解決する．
---
- [x] **Understanding Political Polarization via Jointly Modeling Users, Connections and Multimodal Contents on Heterogeneous Graphs(2022)**  
   [[link]](https://dl.acm.org/doi/abs/10.1145/3503161.3547898)
   異種グラフからユーザ埋め込みを学習し，政治的な意見を検出．
   <details><summary>概要</summary><div>
    最終的にはその結果から政治的偏向の理解を深めることが目的.コンテンツ(ツイート)のみでなく，ユーザとツイートがエッジで結ばれた異種グラフを作成．ユーザノードの初期特徴量はフォローフォロワー数やプロフィール文，ツイートノードはテキスト情報と投稿したユーザ情報から算出．この異種グラフにGNNを適用し政治的偏向の理解に有効なembeddingを得る．同種のGNNフレームワークを凌駕する精度でユーザー埋め込みを学習．
- [x] **A Heterogeneous Information Network based Cross Domain Insurance Recommendation System for Cold Start Users(2020)**  
   [[link]](https://arxiv.org/abs/2007.15293)
   異種ネットワークの情報集約
   <details><summary>概要</summary><div>
    ユーザへの保険推薦のための，異種情報ネットワークに基づくクロスドメイン推薦．推薦のために，3つのレベル（関係，ノード，意味）の注意集約(attention aggregation)を採用し，ユーザーと保険商品の表現を得る．具体的には，まず1ホップ異種隣接を集約するための関係的注意を提案する．これは，異なる1ホップ近傍間で同じ集計関数を使用するのではなく，関係の種類ごとに特定の集計関数を学習する．次にメタパスに基づく隣接を集約するためのノード注意，メタパスに基づく隣接集合を集約するための意味的注意を提案する．(メタパスが異なれば，意味も異なるという考えに基づき，メタパスにに基づく隣接の定義を与えている)最後に，関係的注意の集約と意味的注意の集約の結果を元のノード埋め込みに集約し，ノード表現を更新する．
---
- [x] **Heterogeneous Graph Attention Network(2019)**  
   [[link]](https://arxiv.org/abs/1903.07293)
   異種グラフにおけるAttentionを用いた学習
   <details><summary>概要</summary><div>
   ノードとそのメタパスに基づく隣接ノードとの間の重要度を学習する「ノードレベルAttention」と，異なるメタパスの重要度を学習する「セマンティックレベルAttention」が存在する．ノードレベルAttentionでは，各メタパスごと(どのノードを基準に近傍を考えるか)の近傍ノードから，重要なノードを決定，つまり，(1)Aベースにおける近傍ノードのうち重要なもの(2)Dベースにおける近傍ノードのうち重要なものを決定する．そしてそれらの重要性を考慮して，ソースノードに情報を集約させる．「セマンティックレベルAttention」では，「ノードレベルAttention」で得られた各メタパスごとの重要ノードを考慮したソースノードのうち，それぞれのメタパスの重要性を決定する．以上のプロセスで，異種グラフの学習を行う．
---
- [x] **Heterogeneous Graph Transformer(2020)**  
   [[link]](https://arxiv.org/abs/2003.01332)
   異種グラフにおけるTransformerのアーキテクチャを参考にした学習
   <details><summary>概要</summary><div>
   異種グラフにおける学習において，Attentionを計算する際にTransformerのアーキテクチャを用いて異種グラフの各メタパス情報を考慮した学習を行う．具体的には，同種GNNであるGATにおけるAttentionを計算する際，Transformerのアーキテクチャを参考に各ソースノード，ターゲットノードの種類ごとに固有の表現空間に，Query,Keyとしてマッピングする．そして，GATにおけるMessageを計算する際，ターゲットノードの種類ごとに固有の表現空間に，Vakueとしてマッピングする．そうすることで，異種グラフにおける各メタパスごとに固有の表現空間を保持する．
---
## その他
- [x] **CSI: A Hybrid Deep Model for Fake News Detection(2017)**  
   [[link]](https://arxiv.org/abs/1703.06959)
   フェイクニュース検出
   <details><summary>概要</summary><div>
    フェイクニュースの自動検出の際に，Capture，Score，Integrateという3つのモジュールからモデルを提案する．Captureは，RNNを用いてニュース記事に対するユーザの時間的表現を取得，Scoreはユーザの行動に基づいてスコアを学習し，Integrateはこの2つのモジュールの統合を行い，出力で記事がFakeかどうかを判断．ユーザの特徴量は，ユーザについては，どの記事に関与したかに着目していた
---
- [x] **A Survey on Automatic Detection of Hate Speech in Text(2018)**  
   [[link]](https://dl.acm.org/doi/10.1145/3232676)
   ヘイトスピーチの自動検出と，ヘイトスピーチの定義についての研究
   <details><summary>概要</summary><div>
   テキスト中のヘイトスピーチの自動検出が過去数年にわたってどのように進化してきたかについての調査．最初に，SNSから他の媒体までの異なる状況におけるヘイトスピーチの概念を分析．さらに，他文献に見られる分類のための例と規則を，それらの規則に賛成または反対する議論を行った．批判的な見解としては，我々が文献に見られる他の視点よりも，ヘイトスピーチについてより包括的で一般的な定義を持っていることを指摘．これは，インターネットやSNS上の微妙な形態の差別も発見されるべきであると主張．今回の分析により，ヘイトスピーチをネットいじめ，暴言，差別，毒，炎上，過激主義，過激化と比較することが重要であると結論づけた．
---
- [x] **Exploring Hate Speech Detection in Multimodal Publications(2019)**  
   [[link]](https://arxiv.org/abs/1910.03814)
   ヘイトスピーチ検出の際，テキストに加え画像も考慮したモデルを提案
   <details><summary>概要</summary><div>
   テキストと画像によって形成される投稿(Twitterなど)から大規模なデータセットを収集して注釈を付け，ヘイトスピーチ検出のためにテキストと視覚情報を共同で分析する異なるモデルを提案．それらを単一モード検出と比較．定量的および定性的結果を提供し，提案されたタスクの課題を分析，結果としては，画像がヘイトスピーチ検出タスクに有用であっても，現在のマルチモーダルモデルはテキストのみを分析するモデルよりも優れていないことが分かった．
- [x] **A Survey on Hate Speech Detection using Natural Language Processing(2017)**  
   [[link]](https://aclanthology.org/W17-1101/)
   自然言語処理処理を用いたヘイトスピーチ検出と，これらのアプローチの限界について研究
   <details><summary>概要</summary><div>
   ヘイトスピーチの自動検出に関する調査．これらのタスクは通常，教師付き学習問題としてフレーム化されている．テキストから得られた情報は，ヘイトスピーチの存在を示唆する唯一の手がかりではないかもしれないことを主張．メタ情報または他のモダリティからの情報(例えば，メッセージに添付された画像)によって補完することができると考えられる．結論としては，多くの複雑な特徴の一般的な有効性について判断することは困難．なぜなら，ほとんどの場合それらは個々のデータセットでのみ評価され，ほとんどがオープン用可能ではなく，特定の少数民族のいじめなどヘイトスピーチのサブタイプのみを扱うことが多いからであると主張．
---
- [x] **On the rise of fear speech in online social media(2023)**  
   [[link]](https://www.pnas.org/doi/abs/10.1073/pnas.2212270120)
   ヘイトスピーチに変わる悪質な投稿として，fear speech(恐怖スピーチ)について紹介
   <details><summary>概要</summary><div>
   恐怖スピーチは，その名が示すように対象コミュニティに対する恐怖を扇動しようとする内容のことを指す．Gab.comから収集した400Kの恐怖スピーチと700K以上のヘイトスピーチ投稿の普及を理解するための大規模な研究を行った．データセットの調査結果より，多数の恐怖スピーチを投稿したユーザーは，多数のヘイトスピーチを投稿したユーザーよりも多くのフォロワーを獲得し，ソーシャルネットワークの中心的な位置を占めていることが判明．また，返信，拡散，メンションを通じてヘイトスピーチユーザーよりも効果的に良性のユーザーに接触していることが確認．これは，ヘイトスピーチとは異なり恐怖スピーチには有害な内容がほとんど含まれておらず，もっともらしく見えるという事実と関連しているといえる．さらに，恐怖スピーチのトピックはほとんどの場合コミュニティを(偽の)議論の連鎖を使って加害者として描写しているが，ヘイトスピーチのトピックは直接的な複数の標的を攻撃している．したがって，一般ユーザーが恐怖スピーチに対してより騙されやすいという傾向も見られた．

---
