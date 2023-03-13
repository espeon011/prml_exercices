以下の変換によって \\( (x, y) \\) から \\( (r, \theta) \\) へ変数変換し, \\( I^2 \\) を評価する. 

\begin{align}
x &= r \cos \theta \\\\
y &= r \sin \theta
\end{align}

変数変換のヤコビアン \\( J \\) は

\begin{align}
J &= \det \begin{pmatrix}
            \displaystyle\frac{\partial x}{\partial r} & \displaystyle\frac{\partial x}{\partial \theta} \\\\
            \displaystyle\frac{\partial y}{\partial r} & \displaystyle\frac{\partial y}{\partial \theta}
          \end{pmatrix} \\\\
  &= \det \begin{pmatrix}
            \cos \theta & -r \sin \theta \\\\
            \sin \theta & r \cos \theta
          \end{pmatrix} \\\\
  &= r
\end{align}

となる. よって \\( I^2 \\) は

\begin{align}
I^2 &= \int_{-\infty}^\infty \int_{-\infty}^\infty r \exp \left( - \frac{1}{2 \sigma^2} x^2  - \frac{1}{2 \sigma^2} y^2 \right) \mathrm{d}x \mathrm{d}y \\\\
&= \int_0^\infty \int_0^{2\pi} r \exp \left( - \frac{r^2}{2 \sigma^2} \right) \mathrm{d}\theta \mathrm{d}r
\end{align}

ここで \\( u = r^2 \\) と変換すれば変数変換のヤコビアンは \\( \frac{1}{2 \sqrt{u}} \\) であるから
\begin{align}
I^2 &= \int_0^\infty \int_0^{2\pi} \frac{1}{2} \exp \left( - \frac{u}{2 \sigma^2} \right) \mathrm{d}\theta \mathrm{d}u \\\\
&= 2 \pi \int_0^\infty \frac{1}{2} \exp \left( - \frac{u}{2 \sigma^2} \right) \mathrm{d}u \\\\
&= 2 \pi \left\[ - \sigma^2 \exp \left( - \frac{u}{2 \sigma^2} \right) \right\]_0^\infty \\\\
&= 2 \pi \sigma^2. \ 
\end{align}

よって

\\[
I = \sqrt{2 \pi \sigma^2}
\\]

が得られた. 

ガウス分布が規格化されていることは \\( z = x - \mu \\) と変数変換することで次のように計算できる. 

\begin{align}
\int_{-\infty}^{\infty} \mathcal{N} (x \ | \ \mu, \sigma^2) \mathrm{d} x &= \frac{1}{\sqrt{2 \pi \sigma^2}} \int_{-\infty}^{\infty} \exp \left( - \frac{1}{2 \sigma^2} (x - \mu)^2 \right) \mathrm{d}x \\\\
&= \frac{1}{\sqrt{2 \pi \sigma^2}} \int_{-\infty}^{\infty} \exp \left( - \frac{1}{2 \sigma^2} z^2 \right) \mathrm{d}z \\\\
&= \frac{I}{\sqrt{2 \pi \sigma^2}} = 1. \ \Box
\end{align}