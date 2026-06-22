
# Noisy Label


## Title List

1. [Adaptive Integration of Partial Label Learning and Negative Learning for Enhanced Noisy Label Learning (2024:AAAI)]
2. [Regroup Median Loss for Combating Label Noise (2024:AAAI)]
3. [Learning Accurate Pseudo-Labels via Feature Similarity in the(MDPI)]
4. [LSV-Learner: Support-Vector Contrastive Learning for Robust Learning with Noisy Labels (IEEE2024)]
5. [SigCo: Eliminate the inter-class competition via sigmoid for learning with noisy labels (CVPR2022)]
6. [Manifold DivideMix: A Semi-Supervised Contrastive Learning Framework for Severe Label Noise (CVPR2024)]
7. [Selective-Supervised Contrastive Learning With Noisy Labels (CVPR2022)]
8. [UniCon: Combating Label Noise Through Uniform Selection and Contrastive Learning (CVPR2022)]
9. [Adaptive Contrastive Learning for Learning Robust (2023)]
10. [UniCon: Combating Label Noise Through Uniform Selection and Contrastive Learning (CVPR2022)]
11. [RankMatch: Fostering Confidence and Consistency in Learning with Noisy Labels (ICCV2023)]
12. [Supervised contrastive learning with corrected labels for noisy label learning (2023)]
13. [NoiseBox: Towards More Efficient and Effective Learning with Noisy Labels (IEEE2024)]
14. [Learning with Structural Labels for Learning with Noisy Labels (CVPR2024)]
15. [Learning with Noisy Labels Interconnection of Two Expectation-Maximizations (CVPR2024)]
16. [Subclass-Dominant Label Noise: A Counterexample for the Success of Early Stopping (NeurIPS2023)]
17. [BPT-PLR: A Balanced Partitioning and Training Framework with Pseudo-Label Relaxed Contrastive Loss for Noisy Label Learning]
18. [Enhancing Noisy Label Learning Via Unsupervised Contrastive Loss with Label Correction Based on Prior Knowledge]
19. [ProMix: Combating Label Noise via Maximizing Clean Sample Utility]
20. [Prediction Consistency Regularization for Learning with Noise Labels Based on Contrastive Clustering]
21. [Learning transferable visual models from natural language supervision]
22. [Improving CLIP Robustness with Knowledge Distillation and Self-Training]
23. [Robust Noisy Label Learning via Two-Stream Sample Distillation]
24. [CLIPCleaner: Cleaning Noisy Labels with CLIP]
25. [Vision-Language Models are Strong Noisy Label Detectors]
26. [FedPPO: Reinforcement Learning-Based Client Selection for Federated Learning With Heterogeneous Data]
27. [Reinforcement Learning-Guided Semi-Supervised Learning]
28. [Domain adaptation in reinforcement learning: a comprehensive and systematic study]

---

### Adaptive Integration of Partial Label Learning and Negative Learning for Enhanced Noisy Label Learning(2024:AAAI)
[[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/28284/28559)
[[Code]](https://github.com/NUST-Machine-Intelligence-Laboratory/NPN)
[[bibtex]](https://ojs.aaai.org/index.php/AAAI/article/view/28284)
<details><summary>summary</summary><div>
データセットがCIFAR-100から派生したCIFAR-100N使っている．
部分ラベル学習(PLL:各サンプルに複数のラベルが与えられる)とNegative learning(NL)を統合している．
PLLで複数のラベルが含まれているから正解ラベルが含まれていることが保証されるようにしている．信頼性とかを使っているぽい
NLを用いて入力された画像はこの補完ラベルに属さないみたいなことを学習しているぽい?
</div></details> 

### Regroup Median Loss for Combating Label Noise (2024:AAAI)
[[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/29250/30360)
[[Code]](https://github.com/Feng-peng-Li/Regroup-Loss-Median-to-Combat-Label-Noise)
[[bibtex]](https://ojs.aaai.org/index.php/AAAI/article/view/29250)
<details><summary>summary</summary><div>
Instanceノイズが登場している(CIFAR)
CIFAR-10のSymmetric50%で90%弱だったのであまり正解率高くない?
ノイズのあるサンプルの損失を修正する．
トレーニングサンプルと同じラベルを持つサンプルをランダムに選択し，再グループ化する．
</div></details> 

### Learning Accurate Pseudo-Labels via Feature Similarity in the(MDPI)
[[Paper]](https://www.mdpi.com/2076-3417/14/7/2759/pdf?version=1711447152)
[[bibtex]](https://www.mdpi.com/2076-3417/14/7/2759)
<details><summary>summary</summary><div>
モデル予測と特徴量の類似性からの情報を利用する特徴擬似ラベル(FPL)を使っている．
精度Clothing1Mで73.54%
CIFARは少し低そうな印象
各クラスの特徴の中心(式を見た感じ論文で用いた重心とは違いそうだった)を計算し，各サンプルとのcos類似度を求め，最も類似性の高いクラスを特徴ラベル(ハードラベル？)とする．特徴ラベルとモデルの予測クラスから特徴擬似ラベルを作成している．
特徴量に対する擬似ラベルを考えている．
次やりたかったことに似ている気がする．
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### LSV-Learner: Support-Vector Contrastive Learning for Robust Learning with Noisy Labels(IEEE2024)
[[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10495194)
[[code]](https://github.com/yanliji/SV-Learner)
[[bibtex]](https://ieeexplore.ieee.org/abstract/document/10495194)
<details><summary>summary</summary><div>
対照学習にサポートベクターマシン(SVM)を導入した(SVCL)を使っている．
各クラスの特徴分布境界でSVMを考える．ここで，サポートベクトルはクリーンなセットから選択する．
TCLが引用されていた
サポートベクトル対照学習(SVCL)は、サポートベクトルを使用して超平面を構築し、異なるカテゴリの特徴分布間の超平面マージンを最大化することで、特徴分布の収束を最適化し、半教師付き分類に役立つ。
精度が高い
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### SigCo: Eliminate the inter-class competition via sigmoid for learning with noisy labels
[[Paper]](https://openaccess.thecvf.com/content/CVPR2022/papers/Li_Selective-Supervised_Contrastive_Learning_With_Noisy_Labels_CVPR_2022_paper.pdf)
[[bibtex]](https://www.sciencedirect.com/science/article/pii/S0950705124002867)
<details><summary>summary</summary><div>
データセットはCIFAR-10N, CIFAR-100Nなどを使っている
クラスごとにしきい値を用いて判断しており，複数のクラスでしきい値を超えたサンプルはハードとしている．
データをシグモイド予測に基づいて，サンプルをクリーン，ハード，ノイジーに分割する
また，ネットワークの表現学習を暗黙的に学習している．
そのため，対照学習も用いている．
この際ポジティブとしてクリーンセット内の同じクラスのサンプルを選択している．
精度が高い
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### Manifold DivideMix: A Semi-Supervised Contrastive Learning Framework for Severe Label Noise(CVPR2024)
[[Paper]](https://openaccess.thecvf.com/content/CVPR2024W/VAND/papers/Fooladgar_Manifold_DivideMix_A_Semi-Supervised_Contrastive_Learning_Framework_for_Severe_Label_CVPRW_2024_paper.pdf)
[[code]](https://github.com/Fahim-F/ManifoldDivideMix)
[[bibtex]](https://openaccess.thecvf.com/content/CVPR2024W/VAND/html/Fooladgar_Manifold_DivideMix_A_Semi-Supervised_Contrastive_Learning_Framework_for_Severe_Label_CVPRW_2024_paper.html)
<details><summary>summary</summary><div>
ベースはDivideMix
はじめに対照学習を用いて埋め込み空間を学習する(warmup)
ラベルの信頼度は埋め込み空間に基づいて分布外検出を用いて行われている(TCLと同じやと思う)
MixUpにサンプル，ラベルの他に埋め込み空間でも結合している
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### Selective-Supervised Contrastive Learning With Noisy Labels(CVPR2022)
[[Paper]](https://openaccess.thecvf.com/content/CVPR2024W/VAND/papers/Fooladgar_Manifold_DivideMix_A_Semi-Supervised_Contrastive_Learning_Framework_for_Severe_Label_CVPRW_2024_paper.pdf)
[[code]](https://github.com/ShikunLi/Sel-CL)
[[bibtex]](https://openaccess.thecvf.com/content/CVPR2022/html/Li_Selective-Supervised_Contrastive_Learning_With_Noisy_Labels_CVPR_2022_paper.html)
<details><summary>summary</summary><div>
選択的教師あり対照学習を用いている
選択手法は，対照サンプルに対して類似度の高いサンプルのラベルで多数決を取る. 1つのクラスが擬似ラベルとして割り振られるイメージ(擬似ラベル1とする)
擬似ラベル1を基に，類似性の高いサンプルのラベルの割合を擬似ラベルとする．
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### UniCon: Combating Label Noise Through Uniform Selection and Contrastive Learning(CVPR2022)
[[Paper]](https://openaccess.thecvf.com/content/CVPR2022/papers/Karim_UniCon_Combating_Label_Noise_Through_Uniform_Selection_and_Contrastive_Learning_CVPR_2022_paper.pdf)
[[code]](https://github.com/nazmul-karim170/UNICON-Noisy-Label)
[[bibtex]](https://openaccess.thecvf.com/content/CVPR2022/html/Karim_UniCon_Combating_Label_Noise_Through_Uniform_Selection_and_Contrastive_Learning_CVPR_2022_paper.html)
<details><summary>summary</summary><div>
ラベルありサンプルの個数をクラス毎に均等にしている．
FixMatchベースのSSLに教師なし対照学習を組み込んでいる
</div></details> 
- Keywords : `` 'Contrastive Learning?'


### Adaptive Contrastive Learning for Learning Robust(2023)
[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3581783.3612491)
[[bibtex]](https://dl.acm.org/doi/abs/10.1145/3581783.3612491)
<details><summary>summary</summary><div>
ラベルありサンプルの個数をクラス毎に均等にしている．
FixMatchベースのSSLに教師なし対照学習を組み込んでいる
</div></details> 
- Keywords : `` 'Contrastive Learning?'


### UniCon: Combating Label Noise Through Uniform Selection and Contrastive Learning(CVPR2022)
[[Paper]](https://openaccess.thecvf.com/content/CVPR2022/papers/Karim_UniCon_Combating_Label_Noise_Through_Uniform_Selection_and_Contrastive_Learning_CVPR_2022_paper.pdf)
[[code]](https://github.com/nazmul-karim170/UNICON-Noisy-Label)
[[bibtex]](https://openaccess.thecvf.com/content/CVPR2022/html/Karim_UniCon_Combating_Label_Noise_Through_Uniform_Selection_and_Contrastive_Learning_CVPR_2022_paper.html)
<details><summary>summary</summary><div>
適応的対照学習法(ACLを提案)→ 固定されたしきい値の代わりに，自己適応的しきい値を使用して，対照学習のペアを選択する
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### RankMatch: Fostering Confidence and Consistency in Learning with Noisy Labels(ICCV2023):RankMatch
[[Paper]](https://openaccess.thecvf.com/content/ICCV2023/papers/Zhang_RankMatch_Fostering_Confidence_and_Consistency_in_Learning_with_Noisy_Labels_ICCV_2023_paper.pdf)
[[bibtex]](https://openaccess.thecvf.com/content/ICCV2023/html/Zhang_RankMatch_Fostering_Confidence_and_Consistency_in_Learning_with_Noisy_Labels_ICCV_2023_paper.html)
<details><summary>summary</summary><div>
信頼投票によるサンプリングを導入 → 信頼できるサンプルからの重心をクラスタ平均とする(各クラスプロトタイプ複数個できる感じやと思う)
対照学習では，特徴ベクトルに重要度をつけて重要度が高いところの類似性が高くなることを優先して学習している?
</div></details> 

### Supervised contrastive learning with corrected labels for noisy label learning(2023)
[[Paper]](https://link.springer.com/content/pdf/10.1007/s10489-023-05018-0.pdf)
[[code]](https://github.com/ChenyangLu922/SCL2.git)
[[bibtex]](https://link.springer.com/article/10.1007/s10489-023-05018-0)
<details><summary>summary</summary><div>
教師あり対照学習に修正ラベルの概念を導入した．同じソフトラベルを共有するサンプルは正のペアとしている．また，プロトタイプを用いた対照学習も行っている．
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### NoiseBox: Towards More Efficient and Effective Learning with Noisy Labels(IEEE2024)
[[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10594806)
[[bibtex]](https://ieeexplore.ieee.org/abstract/document/10594806)
<details><summary>summary</summary><div>
NoiseBoxを導入した学習法．精度がすごく高い．既存のサンプル選択の多くと組み合わせることが可能
</div></details> 
- Keywords : `` 'Contrastive Learning?'

### Learning with Structural Labels for Learning with Noisy Labels (CVPR2024)
[[Paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Kim_Learning_with_Structural_Labels_for_Learning_with_Noisy_Labels_CVPR_2024_paper.pdf)
[[bibtex]](https://openaccess.thecvf.com/content/CVPR2024/html/Kim_Learning_with_Structural_Labels_for_Learning_with_Noisy_Labels_CVPR_2024_paper.html)
<details><summary>summary</summary><div>
CIFAR-10 Sym.20%の正解率97%超えていた．
分布情報構造ラベルを導入した．これは，
</div></details> 
- Keywords : `` 

### Learning with Noisy Labels Interconnection of Two Expectation-Maximizations (CVPR2024)
[[Paper]](https://arxiv.org/pdf/2401.04390)
[[bibtex]](https://arxiv.org/abs/2401.04390)
<details><summary>summary</summary><div>
CIFAR-10 Sym.20%の正解率97%超えていた．
mineネットワークと補助ネットワークを使って学習していた．
補助ネットワークは擬似ラベルを推定するために存在する．
</div></details> 
- Keywords : `` 

### Subclass-Dominant Label Noise: A Counterexample for the Success of Early Stopping
[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2023/file/d763b4a2dde0ae7b77498516ce9f439e-Paper-Conference.pdf)
[[code]](https://github.com/tmllab/2023_NeurIPS_SDN)
[[bibtex]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d763b4a2dde0ae7b77498516ce9f439e-Abstract-Conference.html)
<details><summary>summary</summary><div>
NoiseClusterの基本原理は「レイターストッピング（later stopping）」に基づいている。従来はノイズデータが時間とともに表現を劣化させると考えられていたが，本研究では，レイターストッピングによって得られる長期間トレーニングされた表現が，ノイズのある例の高次の意味をより効果的に捉えることができることを示している。これにより，特徴が似ているノイズのある例の埋め込みが互いに近づくクラスタリング効果が生じる。
具体的には，まずネットワークのトレーニングをレイターストッピングで停止した後，特徴密度に基づいてこれらの特徴をクラスごとにグループ化し，最も大きなグループを「クリーングループ」として識別する。これは正しいラベルである可能性が高いためであり，残りのグループは「誤ラベルの可能性があるグループ」として扱う。
</div></details> 
- Keywords : `` 

### BPT-PLR: A Balanced Partitioning and Training Framework with Pseudo-Label Relaxed Contrastive Loss for Noisy Label Learning
[[Paper]](file:///Users/reo/Desktop/entropy-26-00589.pdf)
[[code]](https://github.com/LanXiaoPang613/BPT-PLR)
[[bibtex]](https://www.mdpi.com/1099-4300/26/7/589)
<details><summary>summary</summary><div>
本研究では「BPT-PLR」と呼ばれる，擬似ラベル緩和コントラスト損失を用いたバランス分割・訓練フレームワークを提案する。このフレームワークは，2次元ガウス混合モデルを用いたバランス分割プロセス（BP-GMM）と，擬似ラベル緩和コントラスト損失を用いた半教師ありオーバーサンプリング訓練プロセス（SSO-PLR）という2つの重要なプロセスから構成される。前者は，意味的な特徴情報とモデルの予測結果の両方を利用してノイズラベルを識別し，分割されたサブセット間のクラスバランスを可能な限り保つためのバランス調整戦略を導入する。後者は，最新の擬似ラベル緩和コントラスト損失を採用して教師なしコントラスト損失を置き換え，半教師あり学習と教師なしコントラスト損失間の最適化の衝突を軽減し，性能を向上させる。
精度はめっちゃ高い
</div></details> 
- Keywords : `` 

### Enhancing Noisy Label Learning Via Unsupervised Contrastive Loss with Label Correction Based on Prior Knowledge
[[Paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10446840)
[[code]](https://github.com/LanXiaoPang613/BPT-PLR)
[[bibtex]](https://ieeexplore.ieee.org/abstract/document/10446840)
<details><summary>summary</summary><div>
本手法では，事前学習済みの視覚・言語モデルの事前知識を導入することで，NLLの学習プロセスに依存せずにクリーンサンプルを効果的に選択することが可能となる。
提案手法では，データセット内の画像とラベルを事前学習済みの視覚と言語モデルによって構築された潜在空間に埋め込み，埋め込み表現間の距離に基づいてラベル修正を行う．
CIFAR-10,100のSym.80,90%しか実験してないが，CIFAR-10では，Sym.20%とあまり変わらない正解率(96.8)．CIFAR-100でも70を超えている．
</div></details> 
- Keywords : `` 

### ProMix: Combating Label Noise via Maximizing Clean Sample Utility
[[Paper]](https://arxiv.org/pdf/2207.10276)
[[code]](https://github.com/Justherozen/ProMix)
[[bibtex]](https://arxiv.org/abs/2207.10276)
<details><summary>summary</summary><div>
観測されたラベルに対して高い予測スコアを持つサンプルを収集することで，基礎となるクラスごとの選択セットを動的に拡張する「進行的選択メカニズム」を提案する。
この最大選択手順には，SSLに対する副作用が伴う可能性がある。第一に，クリーンサンプルが異なるラベル間で均等に分布しない可能性があり，ラベル分布に偏りが生じる。第二に，選択手順と半教師あり学習手順が緊密に依存しているため，自らのエラーを繰り返し確認する「確認バイアス」に起因する問題が発生する可能性がある。これらの問題を軽減するために，以下の2つの主要な要素を含む「デバイアス化SSLトレーニングフレームワーク」を開発した。1つ目は補助的な擬似ヘッドで，信頼性の低い擬似ラベルの生成と利用を分離し，モデルがエラーを自己確認することを防ぐものである。2つ目は，偏った擬似ラベルとクロスエントロピー損失を同時に補正するキャリブレーションアルゴリズムを組み込むことである。
精度高い．特に低ノイズ率に強い
</div></details> 
- Keywords : `` 

### Prediction Consistency Regularization for Learning with Noise Labels Based on Contrastive Clustering
[[Paper]](https://www.mdpi.com/1099-4300/26/4/308/pdf?version=1712068099)
[[bibtex]](https://www.mdpi.com/1099-4300/26/4/308)
<details><summary>summary</summary><div>
観測されたラベルに対して高い予測スコアを持つサンプルを収集することで，基礎となるクラスごとの選択セットを動的に拡張する「進本研究では，ラベルノイズのある画像データに効果的に対応するために，ツインコントラストクラスタリングに基づく予測一貫性正則化（TPCR）を提案する。本手法は2つの主要なコンポーネントから成る。サンプルの類似性を正確かつ効率的に特定し，自己教師あり学習に伴うリスクを軽減するために，TPCRは表現学習のフレームワークとしてツインコントラストクラスタリング（TCC）【12】を採用した。TCCをラベル一貫性を反映する表現を生成できるよう改善し，最初のリスクに対処している。TCCのプレテキストタスクが入力サンプルを異なるグループにクラスタリングするため，同じクラスタに属するサンプルは追加計算なしに本質的に類似していると見なすことができ，2つ目のリスクを回避する。次に，改良されたTCCのクラスタリング結果に基づき，各クラスタ内での分類の一貫性を高めるため，モデル出力とプロトタイプ間のクロスエントロピーを罰則化するプロトタイプベースの正則化手法を設計した
</div></details> 
- Keywords : `` 

### Learning transferable visual models from natural language supervision
[[Paper]](http://proceedings.mlr.press/v139/radford21a/radford21a.pdf)
[[code]](https://github.com/OpenAI/CLIP)
[[bibtex]](http://proceedings.mlr.press/v139/radford21a)
<details><summary>summary</summary><div>
CLIP
</div></details> 
- Keywords : ``

### Improving CLIP Robustness with Knowledge Distillation and Self-Training
[[Paper]](https://arxiv.org/pdf/2309.10361)
[[code]](https://github.com/OpenAI/CLIP)
[[bibtex]](https://arxiv.org/abs/2309.10361)
<details><summary>summary</summary><div>
CLIPを教師なし学習で再学習している
教師あり学習の参考にできそう
</div></details> 
- Keywords : ``

### Robust Noisy Label Learning via Two-Stream Sample Distillation
[[Paper]](https://arxiv.org/pdf/2404.10499)
[[bibtex]]([https://arxiv.org/abs/2309.10361](https://arxiv.org/abs/2404.10499?utm_source=chatgpt.com))
<details><summary>summary</summary><div>
この手法では、サンプル選択とラベル補正を組み合わせ、ノイズの多いラベルを持つデータセットに対して、学習中に高品質なサンプルを抽出するTwo-Stream Sample Distillation（TSSD）フレームワークが提案されている。CIFAR-10やCIFAR-100などでの実験において、ノイズの影響を受けにくいモデルの学習が可能であることが示されている。精度が高い
</div></details> 
- Keywords : ``

### CLIPCleaner: Cleaning Noisy Labels with CLIP
[[Paper]](https://dl.acm.org/doi/pdf/10.1145/3664647.3680664)
[[bibtex]](https://dl.acm.org/doi/abs/10.1145/3664647.3680664)
<details><summary>summary</summary><div>
clipの予測値使って学習している．
</div></details> 
- Keywords : ``


### Vision-Language Models are Strong Noisy Label Detectors
[[Paper]](https://proceedings.neurips.cc/paper_files/paper/2024/file/6af08ba9468f0daca4b8dd388cb95824-Paper-Conference.pdf)
[[bibtex]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/6af08ba9468f0daca4b8dd388cb95824-Abstract-Conference.html)
<details><summary>summary</summary><div>
clipをファインチューニングしている
精度すごく高い
</div></details> 
- Keywords : ``
