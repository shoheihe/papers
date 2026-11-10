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

<details><summary>S. Ahn, S. Kim, J. Ko, S. Yun, Fine-tuning Pre-trained Models for Robustness under Noisy Labels, IJCAI, 2024</summary><div>事前学習モデルを利用したNLL．Fine Tuningの有効性がノイズ率によって有効性が異なるかことを実験的に確認．線形分類器だけを学習し，GMMによるclean-dataでFFTを行い高精度を実現．
</div></details>


---

