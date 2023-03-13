\\( x \\), \\( y \\) を独立とする. 
このとき \\( p(x, y) = p(x) p(y) \\) である. 
よって

\begin{align}
\mathrm{cov} \left\[ x,y \right\] &= \mathbb{E} \[ x y \] - \mathbb{E} \[ x \] \mathbb{E} \left\[ y \right\] \\\\
&= \iint_{\mathbb{R}^2} xy p(x, y) \mathrm{d}x \mathrm{d}y - \mathbb{E} \[ x \] \mathbb{E} \[ y \] \\\\
&= \int_{-\infty}^\infty x p(x) \mathrm{d}x \int_{-\infty}^\infty y p(y) \mathrm{d}y - \mathbb{E} \[ x \] \mathbb{E} \[ y \] \\\\
&= \mathbb{E} \[ x \] \mathbb{E} \[ y \] - \mathbb{E} \[ x \] \mathbb{E} \[ y \] = 0. \ \Box
\end{align}
