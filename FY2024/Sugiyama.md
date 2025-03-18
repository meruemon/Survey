+ ## Diversified Recommendation
    <details>
  　<summary>DGCN: Diversified Recommendation with Graph Convolutional Networks (WWW 2021)</summary>

    - [[paper]](https://dl.acm.org/doi/abs/10.1145/3442381.3449835) [[code]](https://github.com/tsinghua-fib-lab/DGCN)
    </details>


    <details>
  　<summary>DGRec: Graph Neural Network for Recommendation with Diversified Embedding Generation (WSDM 2023)</summary>

    - 類似度が最小になるように隣接ノードのアイテムをサンプリング，カテゴリ内のアイテム数が少ないアイテムが重要になるように重みづけ
    - [[paper]](https://arxiv.org/abs/2211.10486) [[code]](https://github.com/YangLiangwei/DGRec)
    </details>


    <details>
  　<summary>Contrastive Co-training for Diversified Recommendation (IJCNN 2022)</summary>

    - 普通のグラフと対照学習用のグラフで共同学習
    - 対照学習に用いるアイテムを相互作用数の逆数やカテゴリ数の逆数の比率でサンプリング
    - [[paper]](https://www.amazon.science/publications/contrastive-so-training-for-diversified-recommendation)
    </details>


    <details> 
  　<summary>The use of MMR, diversity-based reranking for reordering documents and producing summaries (SIGIR 1998)</summary>

    - 多様性のベースライン
    - 後処理による並べ替え
    - [[paper]](https://dl.acm.org/doi/10.1145/290941.291025)
    </details>


    <details>
  　<summary>Fast Greedy MAP Inference for Determinantal Point Process to Improve Recommendation Diversity (NeurIPS 2018)</summary>

    - 多様性のベースライン2
    - 後処理による並べ替え
    - [[paper]](https://arxiv.org/abs/1709.05135)
    </details>


    <details>
  　<summary>Disentangled Representation for Diversified Recommendations (WSDM 2023)</summary>

    - 識別器を用いてカテゴリに依存する表現と依存しない表現を獲得
    - [[paper]](https://arxiv.org/abs/2301.05492) [[code]](https://github.com/Xiaoyinggit/DCRS)
    </details>

+ ## Contrastive Learning for Recommendation 

  <details>
  <summary>Self-supervised Graph Learning for Recommendation (SIGIR 2021)</summary>

  - 対照学習を用いた推薦システムのベースとなる論文
  - グラフに2種類の拡張を加えたそれぞれのユーザ同士・アイテム同士を比較
  - 拡張はノードドロップアウト、エッジドロップアウト、ランダムウォークの3種類
  - [[paper]](https://arxiv.org/abs/2010.10783) [[code]](https://github.com/wujcan/SGL-Torch)
  </details>


  <details>
  <summary>Are Graph Augmentations Necessary?: Simple Graph Contrastive Learning for Recommendation (SIGIR 2022)</summary>

  - グラフの拡張の代わりに各層の埋め込みベクトルにノイズを加えてデータ拡張
  - [[paper]](https://arxiv.org/abs/2112.08679) [[code]](https://github.com/Coder-Yu/QRec)
  </details>

  <details>
  <summary>Adap-τ: Adaptively Modulating Embedding Magnitude for Recommendation (WWW 2023)</summary>

  - 対照損失で用いるハイパーパラメータ$\tau$の値をスコアから自動的に決定する
  - [[paper]](https://arxiv.org/abs/2302.04775) [[code]](https://github.com/junkangwu/Adap_tau)
  </details>

  <details>
  <summary>Multisample-Based Contrastive Loss for Top-K Recommendation (IEEE 2021)</summary>

  - [[paper]](https://ieeexplore.ieee.org/document/9609670) [[code]](https://github.com/haotangxjtu/MSCL)
  </details>

  <details>
  <summary>Ranking-based contrastive loss for recommendation systems( Knowledge-Based Systems 2023)</summary>

  - [[paper]](https://www.sciencedirect.com/science/article/pii/S095070512201276X) [[code]](https://github.com/haotangxjtu/RCL)
  </details>

  <details>
  <summary>Investigating Accuracy-Novelty Performance for Graph-based Collaborative Filtering (SIGIR 2022)</summary>

  - 正規化係数の値を変える
  - より高次の要素を取り込んだ埋め込みを得られ、新規性向上
  - [[paper]](https://arxiv.org/abs/2204.12326)
  </details>


  <details>
  <summary>LightGCL: Simple Yet Effective Graph Contrastive Learning for Recommendation (ICLR 2023)</summary>

  - [[paper]](https://arxiv.org/abs/2302.08191) [[code]](https://github.com/HKUDS/LightGCL)
  </details>

  <details>
  <summary>Incorporating Bias-aware Margins into Contrastive Loss for Collaborative Filtering (NeurIPS 2022)</summary>

  - インタラクション数のみを考慮した推薦でマージンを取る
  - [[paper]](https://arxiv.org/abs/2210.11054) [[code]](https://github.com/anzhang314/BC-Loss)
  </details>

  <details>
  <summary>Invariant Collaborative Filtering to Popularity Distribution Shift (WWW 2023)</summary>

  - 推薦の要因を人気による要因とアイテムそのものによる要因に分割
  - [[paper]](https://arxiv.org/abs/2302.05328) [[code]](https://github.com/anzhang314/InvCF)
  </details>

  <details>
  <summary>Self-supervised Contrastive Learning for Implicit Collaborative Filtering</summary>

  - [[paper]](https://arxiv.org/pdf/2403.07265)
  </details>

+ ## Robust Recommendation / Denoising Recommendation 
  <details>
  <summary>Denoising Implicit Feedback for Recommendation (WSDM 2021)</summary>

  - 1つ目は損失によってしきい値を調整．イテレーションが大きくなるにつれてしきい値を徐々に小さくするように調整．2つ目は予測が困難な(予測スコアが低い)サンプルの重要度を下げるように重みづけ． 
  - [[paper]](https://arxiv.org/abs/2006.04153) [[code]](https://github.com/WenjieWWJ/DenoisingRec)
  </details>

  <details>
  <summary>Self-Guided Learning to Denoise for Robust Recommendation (SIGIR 2022)</summary>

  - [[paper]](https://arxiv.org/abs/2204.06832) [[code]](https://github.com/ZJU-DAILY/SGDL)
  </details>

  <details>
  <summary>Learning Robust Recommenders through Cross-Model Agreement (WWW 2022)</summary>

  - [[paper]](https://arxiv.org/abs/2105.09605) [[code]](https://github.com/wangyu-ustc/DeCA)
  </details>

  <details>
  <summary>Learning to Denoise Unreliable Interactions for Graph Collaborative Filtering (SIGIR 2022)</summary>

  - 1回畳み込んだ後のユーザとアイテムのスコアが低い場合ノイズとしてエッジを削除
  - 多様性を維持するためにユーザと未観測のアイテム間のエッジを追加
  - [[paper]](https://dl.acm.org/doi/abs/10.1145/3477495.3531889) [[code]](https://github.com/ChangxinTian/RGCF)
  </details>

  <details>
  <summary>Towards Robust Neural Graph Collaborative Filtering via Structure Denoising and Embedding Perturbation</summary>

  - 埋め込みベクトルにノイズを与える際に自分以外の埋め込みベクトルを使用
  - [[paper]](https://dl.acm.org/doi/10.1145/3568396)
  </details>

  <details>
  <summary>Efficient Bi-Level Optimization for Recommendation Denoising (KDD 2023)</summary>

  - [[paper]](https://arxiv.org/abs/2210.10321) [[code]](https://github.com/CoderWZW/BOD)
  </details>

  <details>
  <summary>Plug-In Diffusion Model for Embedding Denoising in Recommendation System</summary>

  - [[paper]](https://arxiv.org/abs/2401.06982)
  </details>

  <details>
  <summary>MADM: A Model-agnostic Denoising Module for Graph-based Social Recommendation (WSDM 2024)</summary>

  - [[paper]](https://dl.acm.org/doi/10.1145/3616855.3635784)
  </details>

  <details>
  <summary>Knowledge-refined Denoising Network for Robust Recommendation (SIGIR 2023)</summary>

  - [[paper]](https://arxiv.org/abs/2304.14987) [[code]](https://github.com/xj-zhu98/KRDN)
  </details>

  <details>
  <summary>Co-Training-Teaching: A Robust Semi-Supervised Framework for Review-Aware Rating Regression</summary>
  
  - レーティングに基づいた回帰問題に対してCo-TrainingとCo-Teachingの考え方を利用
  - [[paper]](https://dl.acm.org/doi/10.1145/3625391) [[code]](https://github.com/PennykkLu/CoT2)
  </details>


  <details>
  <summary>Stdfed: A Self-Training Dual-Network Denoising Framework for Federated Recommendation</summary>
  
  - グローバルモデルとローカルモデルの連合学習によるノイズ除去
  - [[paper]](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4743671) [[code]](https://github.com/lgxccc/STDFed)
  </details>

+ ## Others
  <details>
  <summary>Towards Representation Alignment and Uniformity in Collaborative Filtering</summary>

  - AlignmentとUniformityを直接最適化する損失関数を提案
  - [[paper]](https://arxiv.org/abs/2206.12811) [[code]](https://github.com/THUwangcy/DirectAU)
  </details>

  <details>
  <summary>Robust Training of Graph Neural Networks via Noise Governance (WSDM 2023)</summary>

  - [[paper]](https://arxiv.org/abs/2211.06614) [[code]](https://github.com/GhostQ99/RobustTrainingGNN)
  </details>


  <details>
  <summary>LLMRec: Large Language Models with Graph Augmentation for Recommendation (WSDM 2024)</summary>

  - [[paper]](https://arxiv.org/abs/2311.00423) [[code]](https://github.com/HKUDS/LLMRec)
  </details>

<!-- --------[template]

<details>
<summary></summary>

- [[paper]]() [[code]]()
</details>

-------- -->
