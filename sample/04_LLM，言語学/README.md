## LLM，言語学
**文献一覧：**

<details><summary>R. Kang et al., *Is CLIP ideal? No. Can we fix it? Yes!*, ICCV 2025.</summary><div>
CLIPの埋め込み空間について，言語核の視点を踏まえて複雑な位置関係や否定関係を表すことが不可能と数学的にあらわし証明．パッチとテキストのコサイン類似度を総当たりでマップを作成し，マップを用いたスコアリング手法を提案．著者が作成したデータセットで評価．全体の精度が低下してしまっている．
</div></details>
 
<details><summary>G. Nikolaou et al., *Language Models are Injective and Hence Invertible*, preprint, 2025.</summary><div>
LLMが単射であることを証明し，その主張から埋め込み表現から入力が復元可能であることを数学的に証明．実用的な時間での入力復元アルゴリズムの提案．トークンごとに復元し，総当たりで復元してくと時間がかかるので勾配からありえそうなトークンから確かめることで復元時間の短縮を達成． </div></details>
 
<details><summary>T Luo, J Lei, F Lei, W Liu, S He, J Zhao, K Liu, MoELoRA: Contrastive Learning Guided Mixture of Experts on Parameter-Efficient Fine-Tuning for Large Language Models</sammary></div>複数のLoRAまたはAdapterでアンサンブルしても同じような特徴表現を学習してあまり効果がない．それぞれが個別の重要な特徴表現を得るように学習．CleanとNoiseのAdapterに分割してCleanの汚染を避けられるかも．
</div></details>

<details><summary>J Fang, H Jiang, K Wng, Y Ma, ALPHAEDIT: NULL-SPACE CONSTRAINED
KNOWLEDGE EDITING FOR LANGUAGE MODELS</sammary></div>LLMにおいてRAGを用いずに知識を更新していくKnowledge Editingという研究分野．既存知識が存在しない次元をSVDから算出し，その空間に新規知識の更新を加えていく．具体的には，固有値の小さい固有ベクトルを選択するため厳密には零空間にはならない．後述のAlphaEdit+, BetaEditで多数後続研究が存在．
</div></details>

 ---

