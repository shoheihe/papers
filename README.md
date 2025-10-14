# 読んだ論文まとめ

## ① ノイズデータ学習

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

---

## ② 表現学習

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

## ③ アンラーニング

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

---

## ④ 知識蒸留

**文献一覧：**

<details><summary>J. Gou et al., *Knowledge distillation: a survey*, IJCV, 2021.</summary><div>
大規模モデルの知識を小規模モデルに転移する技術を体系的に整理し、分類と課題をまとめた総説。
</div></details>
