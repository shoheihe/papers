# papers
# 文献分類

---

## ① ノイズデータ学習・ロバスト学習（Learning with Noisy or Web Data）

**<details><summary>概要</summary><div>**
Webデータや誤ラベルを含むノイズデータから学習するためのロバスト手法。弱教師あり学習、損失補正、データ選別、ノイズモデル化などを扱う。Crowdsourcingやマルチアノテータ学習も含む。
**</div></details>**

**文献一覧：**
<details>
  <summary>
    P. Welinder et al., *The multidimensional wisdom of crowds*, NIPS, 2010. 
  </summary>
  <div>
    crowdでデータ集める手法について
  </div>
</details>
[2] Y. Yan et al., *Learning from multiple annotators*, JMLR, 2014.  
[3] X. Chen et al., *NEIL: Extracting visual knowledge from web data*, ICCV, 2013.  
[4] F. Schroff et al., *Harvesting image databases from the web*, TPAMI, 2011.  
[5] L. Niu et al., *Visual recognition by learning from web data*, CVPR, 2015.  
[6] T. Xiao et al., *Learning from massive noisy labeled data*, CVPR, 2015.  
[7] W. Li et al., *WebVision database*, arXiv, 2017.  
[8] H. Song et al., *SELFIE*, ICML, 2019.  
[9] S. Guo et al., *CurriculumNet*, ECCV, 2018.  
[14] D. Ortego et al., *Multi-objective interpolation training*, CVPR, 2021.  
[15] J. Li et al., *Learning from noisy data with robust representation learning*, ICCV, 2021.  
[19] Z. Huang et al., *Twin Contrastive Learning with Noisy Labels*, CVPR, 2023.  
[20] R. Fukunaga et al., *Enhancing Robustness to Noisy Labels...*, ITE, 2024.  
[21] S. Li et al., *Selective-Supervised Contrastive Learning with Noisy Labels*, CVPR, 2022.  
[24] J. Li et al., *DivideMix*, arXiv, 2020.  
[25] E. Arazo et al., *Unsupervised label noise modeling and loss correction*, ICML, 2019.  
[30] 杉浦 一瑳ほか, *ミスラベルデータの忘却による学習済みモデルの汎化性能の向上手法の提案*, DEIM, 2024.  
[32] B. V. Rooyen et al., *Learning with symmetric label noise*, NIPS, 2015.  
[33] G. Patrini et al., *Making DNNs robust to label noise*, CVPR, 2017.  

---

## ② 表現学習・一般化・自己教師あり学習（Representation & Generalization Learning）

**<details><summary>概要</summary><div>**
深層表現の一般化や、ラベルに依存しない自己教師あり学習（SimCLR, SimSiam等）、およびコントラスト学習やmixupを用いた表現ロバスト化に関する研究。
**</div></details>**

**文献一覧：**
[10] C. Zhang et al., *Understanding deep learning requires rethinking generalization*, ICLR, 2017.  
[11] D. Arpit et al., *A closer look at memorization in deep networks*, ICML, 2017.  
[12] T. Chen et al., *A Simple Framework for Contrastive Learning (SimCLR)*, ICML, 2020.  
[13] X. Chen & K. He, *Exploring Simple Siamese Representation Learning (SimSiam)*, CVPR, 2021.  
[22] T. Yan et al., *Negative Correlation-Steered Latent Contrastive Learning*, CVPR, 2022.  
[23] H. Zhang et al., *mixup: Beyond empirical risk minimization*, arXiv, 2017.  
[31] L. van der Maaten & G. Hinton, *Visualizing data using t-SNE*, JMLR, 2008.  

---

## ③ 機械的忘却・プライバシー保護（Machine Unlearning & Data Privacy）

**<details><summary>概要</summary><div>**
学習済みモデルから特定データを削除する「機械的忘却（Machine Unlearning）」や、データ保護法（GDPR, CCPAなど）に基づくモデルのプライバシー保証に関する研究。
**</div></details>**

**文献一覧：**
[16] E. Triantafillou et al., *NeurIPS 2023 - Machine Unlearning Competition*, 2023.  
[17] A. Mantelero, *The EU proposal for a general data protection regulation*, CLSR, 2013.  
[18] M. Kurmanji et al., *Towards unbounded machine unlearning*, arXiv, 2023.  
[26] California State Legislature, *Bill AB-375 (California Consumer Privacy Act)*, 2017.  
[27] Office of the Privacy Commissioner of Canada, *Announcement on online reputation*, 2018.  
[28] S. Shastri et al., *The seven sins of personal-data processing systems under GDPR*, USENIX HotCloud, 2019.  

---

## ④ 知識蒸留・知識転移（Knowledge Distillation & Transfer）

**<details><summary>概要</summary><div>**
大規模モデルの知識を小規模モデルに転移する技術。ノイズ耐性・一般化・忘却学習との関連も議論される。
**</div></details>**

**文献一覧：**
[29] J. Gou et al., *Knowledge distillation: a survey*, IJCV, 2021.  
