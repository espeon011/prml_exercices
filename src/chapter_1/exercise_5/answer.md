\\( \mathbb{E}\[ f(x) \] \\) は定数なので \\( \mu \\) とおくと (1.38) より

\begin{align}
\mathrm{var} \[ f \] &= \mathbb{E} \left\[ \left( f(x) - \mu \right)^2 \right\] \\\\
&= \int_{-\infty}^{\infty} \left( f(x)^2 - 2 \mu f(x) + \mu^2 \right) p(x) \mathrm{d}x \\\\
&= \int_{-\infty}^{\infty} f(x)^2 p(x) \mathrm{d}x - 2 \mu \int_{-\infty}^{\infty} f(x) p(x) \mathrm{d}x + \mu^2 \int_{-\infty}^{\infty} p(x) \mathrm{d}x \\\\
&= \mathbb{E} \left\[ f(x)^2 \right\]  - 2 \mu^2 + \mu^2 \\\\
&= \mathbb{E} \left\[ f(x)^2 \right\]  - \mu^2 \\\\
&= \mathbb{E} \left\[ f(x)^2 \right\] - \mathbb{E} \left\[ f(x) \right\]^2. \ \Box
\end{align}