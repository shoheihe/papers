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

<details><summary>Z Xie, Y Shi, D Zhou, AREA: Attribute Extraction and Aggregation for CLIP-Based Class-Incremental Learning, ICML 2026</summary><div>CLIP-basedなCIL．CLIPの予測が属性抽出と属性集約からなることを仮定．超球面上の主成分分析により，各クラスの属性の上位K個を保存．それらの集約により予測．タスク選択に，属性の分布比較による最適輸送を用いる．
新規性：CLIPの属性に着目（これは他にもありそう）．CILでの属性を利用した枠組みの提案．
数学的議論多．根本の知識が違いすぎる．
</div></details>

<details><summary>Z Xie, J Tang, Y Shi, H Ye, D Zhan, D zhou, SAME: Stabilized Mixture-of-Experts for
Multimodal Continual Instruction Tuning, ICML 2026</summary><div>

AREAと同じ著者，南京大学LAMDAのM3．
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
