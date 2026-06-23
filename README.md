# 読んだ論文まとめ

## ノイズデータ学習

**文献一覧：**

<details><summary>P. Welinder et al., *The multidimensional wisdom of crowds*, NIPS, 2010.</summary><div>
クラウドソーシングで収集されたアノテーションを信頼度に基づいて統合し、個々のアノテータの精度を推定する手法を提案。
</div></details>

<details><summary>Y. Yan et al., *Learning from multiple annotators*, JMLR, 2014.</summary><div>
複数アノテータの信頼性を考慮して真のラベルを推定する生成モデルを構築し、誤ラベルの影響を軽減。
</div></details>

<details><summary>X. Chen et al., *NEIL: Extracting visual knowledge from web data*, ICCV, 2013.</summary><div>
Web画像を自動収集し、関係性や概念を抽出して視覚知識ベースを構築する自己教師ありシステムを提案。
</div></details>

<details><summary>F. Schroff et al., *Harvesting image databases from the web*, TPAMI, 2011.</summary><div>
Web画像から信頼性の高いデータセットを自動生成する手法を提案。クラスタリングと外れ値除去によりノイズを軽減。
</div></details>

<details><summary>L. Niu et al., *Visual recognition by learning from web data*, CVPR, 2015.</summary><div>
Webデータを利用した弱教師あり学習によってドメイン一般化を実現する手法を提案。
</div></details>

<details><summary>T. Xiao et al., *Learning from massive noisy labeled data*, CVPR, 2015.</summary><div>
大量のノイズラベルデータから信頼度に基づきサンプルを選別し、ロバストに学習する手法を導入。
</div></details>

<details><summary>W. Li et al., *WebVision database*, arXiv, 2017.</summary><div>
ImageNetと対応する大規模Web画像データセット「WebVision」を公開し、ノイズ環境下での学習を検証。
</div></details>

<details><summary>H. Song et al., *SELFIE*, ICML, 2019.</summary><div>
信頼度の低いサンプルを修正・再利用するノイズ耐性手法を提案。誤ラベルを完全に除去せず再学習に活用。
</div></details>

<details><summary>S. Guo et al., *CurriculumNet*, ECCV, 2018.</summary><div>
サンプルの難易度に基づいて学習順序を制御するカリキュラム学習により、ノイズデータの影響を低減。
</div></details>

<details><summary>D. Ortego et al., *Multi-objective interpolation training*, CVPR, 2021.</summary><div>
複数の目的関数を組み合わせることでラベルノイズに対して頑健な補間学習手法を提案。
</div></details>

<details><summary>J. Li et al., *Learning from noisy data with robust representation learning*, ICCV, 2021.</summary><div>
ノイズデータ下でのロバスト表現獲得を目的とし、特徴空間でのクラスタ構造を利用して誤ラベルを検出。
</div></details>

<details><summary>Z. Huang et al., *Twin Contrastive Learning with Noisy Labels*, CVPR, 2023.</summary><div>
2つのネットワークを対比的に学習させることでノイズラベルを識別し、信頼度の高い表現を抽出する手法を提案。
</div></details>

<details><summary>R. Fukunaga et al., *Enhancing Robustness to Noisy Labels...*, ITE, 2024.</summary><div>
特徴空間で類似クラスを分離することでラベルノイズの影響を抑制する手法を提案。
</div></details>

<details><summary>S. Li et al., *Selective-Supervised Contrastive Learning with Noisy Labels*, CVPR, 2022.</summary><div>
信頼できるサンプルのみを用いた選択的コントラスト学習により、ノイズデータ環境下での精度を向上。
</div></details>

<details><summary>J. Li et al., *DivideMix*, arXiv, 2020.</summary><div>
データをクリーン・ノイズに分割し、半教師あり学習的に同時最適化するノイズ学習の代表的手法。
</div></details>

<details><summary>E. Arazo et al., *Unsupervised label noise modeling and loss correction*, ICML, 2019.</summary><div>
ラベルノイズの分布をモデル化し、損失関数の補正によりロバスト学習を実現。
</div></details>

<details><summary>杉浦 一瑳ほか, *ミスラベルデータの忘却による学習済みモデルの汎化性能の向上手法の提案*, DEIM, 2024.</summary><div>
誤ラベルデータの影響を忘却させることで既存モデルの汎化性能を向上させる手法を提案。
</div></details>

<details><summary>B. V. Rooyen et al., *Learning with symmetric label noise*, NIPS, 2015.</summary><div>
対称ノイズ環境で安定する損失関数「Unhinged Loss」を提案し、理論的なロバスト性を解析。
</div></details>

<details><summary>G. Patrini et al., *Making DNNs robust to label noise*, CVPR, 2017.</summary><div>
ノイズ遷移行列を推定して損失補正を行うことで、ディープネットワークのノイズ耐性を実現。
</div></details>

<details><summary>Haochen Han and Alex Jinpeng Wang and Peijun Ye and Fangming Liu, *Unlearning the Noisy Correspondence Makes CLIP More Robust*, ICCV, 2025</summary><div>マルチモーダルにおける画像分類モデルのCLIPにおいて，2つのノイズを考慮したunlearningを行いZero-Shot精度を向上させる手法．2つのノイズは(1)imageとtextの不一致，(2)似通ったサンプルが特徴空間上で分離される．否定textの特徴量を扱い適切な位置となる損失関数を提案．
</div></details>

<details><summary>S. Ahn, S. Kim, J. Ko, S. Yun, Fine-tuning Pre-trained Models for Robustness under Noisy Labels, IJCAI, 2024</summary><div>
</div></details>




---

## 特徴表現学習

**文献一覧：**

<details><summary>C. Zhang et al., *Understanding deep learning requires rethinking generalization*, ICLR, 2017.</summary><div>
ディープネットがノイズデータを完全に記憶できることを示し、一般化の理論的課題を提示。
</div></details>

<details><summary>D. Arpit et al., *A closer look at memorization in deep networks*, ICML, 2017.</summary><div>
ニューラルネットの記憶挙動を解析し、ノイズサンプルが学習過程に与える影響を詳細に調査。
</div></details>

<details><summary>T. Chen et al., *SimCLR*, ICML, 2020.</summary><div>
データ拡張とコントラスト学習を組み合わせたシンプルな自己教師あり学習枠組みを提案。
</div></details>

<details><summary>X. Chen & K. He, *SimSiam*, CVPR, 2021.</summary><div>
自己教師あり表現学習において、負例を使わずとも安定学習が可能であることを示すシンプルなSiamese構造を導入。
</div></details>

<details><summary>T. Yan et al., *Negative Correlation-Steered Latent Contrastive Learning*, CVPR, 2022.</summary><div>
潜在空間での負相関制約により、ノイズを抑制しながら識別的特徴を強調するコントラスト学習法を提案。
</div></details>

<details><summary>H. Zhang et al., *mixup*, arXiv, 2017.</summary><div>
異なるサンプルの線形補間で学習を安定化させ、過学習とノイズの影響を軽減するデータ拡張手法。
</div></details>

<details><summary>L. van der Maaten & G. Hinton, *t-SNE*, JMLR, 2008.</summary><div>
高次元データを低次元に可視化する手法を提案し、表現空間の構造理解に広く利用される。
</div></details>

---

## アンラーニング

**文献一覧：**

<details><summary>E. Triantafillou et al., *NeurIPS 2023 - Machine Unlearning Competition*, 2023.</summary><div>
モデルから特定データを削除するアルゴリズムを比較する国際競技会を開催し、評価基準を提示。
</div></details>

<details><summary>A. Mantelero, *The EU proposal for a general data protection regulation*, CLSR, 2013.</summary><div>
GDPRの背景と目的を論じ、個人データの制御権をユーザに返す理念を整理。
</div></details>

<details><summary>M. Kurmanji et al., *Towards unbounded machine unlearning*, arXiv, 2023.</summary><div>
無制限に削除要求へ対応可能な機械的忘却手法を提案し、効率と正確性の両立を目指す。
</div></details>

<details><summary>California State Legislature, *Bill AB-375 (CCPA)*, 2017.</summary><div>
カリフォルニア消費者プライバシー法（CCPA）の制定文書。データ削除権の法的基盤を提供。
</div></details>

<details><summary>Office of the Privacy Commissioner of Canada, *Announcement on online reputation*, 2018.</summary><div>
カナダにおけるオンライン上の個人情報削除権に関する法的見解を公表。
</div></details>

<details><summary>S. Shastri et al., *The seven sins of personal-data processing systems under GDPR*, USENIX, 2019.</summary><div>
GDPR違反の典型例を7つに分類し、プライバシー準拠設計の重要性を論じる。
</div></details>


<details><summary>Y. Kuwana, Y. Goto, T. Shibata, G. Irie, Black-Box Forgetting, Advances in Neural Information Processing Systems (NeurIPS), 2024.</summary><div>
汎用的な大規模モデル（CLIP）から，モデルの中身がわからないBalck-Box環境で，特定のタスクに特化するモデルを作成するのが目的．任意のクラスを忘却することで目的を達成．適切な入力プロンプトの学習を行う．トークン間の共有特徴をまとめて学習パラメータの削減．Whiter-Boxと比肩する性能を達成．
</div></details>



---


## LLM，言語学
**文献一覧：**

<details><summary>R. Kang et al., *Is CLIP ideal? No. Can we fix it? Yes!*, ICCV 2025.</summary><div>
CLIPの埋め込み空間について，言語核の視点を踏まえて複雑な位置関係や否定関係を表すことが不可能と数学的にあらわし証明．パッチとテキストのコサイン類似度を総当たりでマップを作成し，マップを用いたスコアリング手法を提案．著者が作成したデータセットで評価．全体の精度が低下してしまっている．
</div></details>
 
<details><summary>G. Nikolaou et al., *Language Models are Injective and Hence Invertible*, preprint, 2025.</summary><div>
LLMが単射であることを証明し，その主張から埋め込み表現から入力が復元可能であることを数学的に証明．実用的な時間での入力復元アルゴリズムの提案．トークンごとに復元し，総当たりで復元してくと時間がかかるので勾配からありえそうなトークンから確かめることで復元時間の短縮を達成． </div></details>
 
 ---

## 知識蒸留

**文献一覧：**

<details><summary>J. Gou et al., *Knowledge distillation: a survey*, IJCV, 2021.</summary><div>
知識蒸留は計算コスト・時間コストの観点から大規模モデルの知識を小規模モデルに転移する研究．そのsurvey論文．
</div></details>

---

## Incremental-Lerning

**文献一覧：**

<details><summary>G. M. van de Ven, T. Tuytelaars, A. S. Tolias, Three types of incremental learning, Nature Machine Intelligence, 2022.</summary><div>
散見されたIncremental-Learningの実験方式を①Domain Incremental Learning, ②Task Incremental Learning, ③Class Incremental Learningの3つに大別している．
</div></details>

<details><summary>Modular Memory is the Key to Continual Learning Agents, arxiv, 2026</summary><div>
AIエージェントにおける継続学習の知識保持方法の提案．一般的な知識を保持する事前に学習されたコアモデル，これまでのユーザの入力特徴からなる長期記憶，現在のタスクに関する入力特徴からなる作業記憶の3点を用いる．推論時，長期記憶から検索し，その情報を活用しコアモデルが出力．長期記憶内の有用な情報を定期的に整理しコアモデルに反映．
</div></details>

### ・Class Incremental Learning

<details><summary>D.-W. Zhou, H.-L. Sun, H.-J. Ye, D.-C. Zhan, Expandable Subspace Ensemble for Pre-Trained Model-Based Class-Incremental Learning, CVPR, 2024.</summary><div>
Pre-Trained ModelとAdapterを使用した，特徴空間上のクラス重心を更新する手法．データ学習後に過去データで学習したadapter上のクラス重心との類似度から学習データのないクラスでも疑似補完．分類器は，クラス重心との類似度のマックス．データごとにAdapterを追加するためにメモリコスト懸念．
</div></details>

<details><summary>M. D. McDonnell, D. Gong, A. Parveneh, E. Abbasnejad, A. van den Hengel, RanPAC: Random Projections and Pre-trained Models for Continual Learning, NeurIPS, 2023.</summary><div>Pre-trained ModelをFrreze, 特徴量を使用しAdapterを学習．ここでRandom Pojectionを利用することで，特徴空間の分離性を高める．頻繁に比較手法で用いられる．DIL, CILで高精度．
</div></details>

<details><summary>X. Yang, G. Lai, D. Meng, X. M. Cao, X. Yang, RACE: Robust adaptive and clustering elimination for noisy labels in continual learning, Knowledge-Based Systems, 2025.</summary><div>CILにノイジーラベルを導入したもの．D^1の学習、Parameter-Efficient Transfer Learning(PETL)において，の維持らーべる学習に適した損失関数の提案．加えてBIRCHを利用したクラスタリングにより，多数決による疑似ラベルの付与．おそらくRanpacの拡張の認識．Real world Datasetでも検証．CILでは最良．DIvideMixなどのNLL手法とnon-countinual設定では精度が高いものの勝つことは厳しい．
</div></details>

<details><summary>T. Tomilin, L. Boogaard, S. Garcin, B. Grooten, M. Fang, Y. Du, M. Pechenizkiy,  MEAL: A Benchmark for Continual Multi-Agent
Reinforcement Learning, ICML, 2026.</summary><div>Agentが複数存在する環境で，Incrementalでタスクが振られたときに強化学習を行う設定における，実験ベンチマークの作成論文．
実世界での想定環境は，複数走行している自動運転のエージェントの新しい規則や標識が追加されるような状況．

新規性：強化学習における継続学習，マルチエージェントにおける強化学習ではベンチマークが作成されているが，それらを組み合わせた環境では適したベンチマークが存在しない．
工夫：OverCookedというゲームの設定を活用．他ベンチマークでも存在する性質を確認することで有効性を検証．
</div></details>

---