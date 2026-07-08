## LLM，言語学
**文献一覧：**

<details><summary>R. Kang et al., *Is CLIP ideal? No. Can we fix it? Yes!*, ICCV 2025.</summary><div>
CLIPの埋め込み空間について，言語核の視点を踏まえて複雑な位置関係や否定関係を表すことが不可能と数学的にあらわし証明．パッチとテキストのコサイン類似度を総当たりでマップを作成し，マップを用いたスコアリング手法を提案．著者が作成したデータセットで評価．全体の精度が低下してしまっている．
</div></details>
 
<details><summary>G. Nikolaou et al., *Language Models are Injective and Hence Invertible*, preprint, 2025.</summary><div>
LLMが単射であることを証明し，その主張から埋め込み表現から入力が復元可能であることを数学的に証明．実用的な時間での入力復元アルゴリズムの提案．トークンごとに復元し，総当たりで復元してくと時間がかかるので勾配からありえそうなトークンから確かめることで復元時間の短縮を達成． </div></details>
 
<details><summary>T Luo, J Lei, F Lei, W Liu, S He, J Zhao, K Liu, MoELoRA: Contrastive Learning Guided Mixture of Experts on Parameter-Efficient Fine-Tuning for Large Language Models</sammary></div>複数のLoRAまたはAdapterでアンサンブルしても同じような特徴表現を学習してあまり効果がない．それぞれが個別の重要な特徴表現を得るように学習．CleanとNoiseのAdapterに分割してCleanの汚染を避けられるかも．
</div></details>
 ---

