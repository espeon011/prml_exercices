この演習問題では, \\( 1 \\) 変数ガウス分布に関する規格化条件 (1.48) を証明する. 
このために積分

\\[
I = \int_{-\infty}^\infty \exp \left( - \frac{1}{2 \sigma^2} x^2 \right) \mathrm{d}x
\\]

を考え, その 2 乗を

\\[
I^2 = \int_{-\infty}^\infty \int_{-\infty}^\infty \exp \left( - \frac{1}{2 \sigma^2} x^2  - \frac{1}{2 \sigma^2} y^2 \right) \mathrm{d}x \mathrm{d}y
\\]

の形で書いて評価する. 
直交座標系 \\( (x, y) \\) から極座標 \\( (r, \theta) \\) に変換し, \\( u = r^2 \\) を代入する. 
\\( \theta \\) と \\( u \\) に関する積分を実行し, 両辺の平方根を取ることにより, 

\\[
I = \left( 2 \pi \sigma^2 \right)^\frac{1}{2}
\\]

が得られることを示せ. 
最後にこの結果からガウス分布 \\( \mathcal{N} (x \ | \ \mu, \sigma^2) \\) が規格化されていることを示せ. 