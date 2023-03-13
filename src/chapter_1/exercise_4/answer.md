まず変換が線形変換である場合に \\( \widehat{x} = g(\widehat{y}) \\) が成り立つことを示す. 
\\( x = g(y) = a y + b \\) とおく. 
このとき

\begin{align}
p_y(y) &= p_x(g(y)) \| g'(y) \| \\\\
       &= p_x( a y + b ) \| a \|. \ 
\end{align}

いま, \\( p_x(x) \\) の最大値は \\( p_x(\widehat{x}) \\) であるから, 

\\[
p_y(y) \leq p_x(\widehat{x}) \| a \|
\\]

である. 
ここで \\(\widehat{y} = g^{-1}(\widehat{x}) = \frac{\widehat{x} - b}{a} \\) とおくと \\( \widehat{x} = g(\widehat{y}) \\) の関係が成り立ち, さらに

\begin{align}
p_y(\widehat{y}) = p_x(\widehat{x}) \| a \|
\end{align}

となり, \\( \widehat{y} \\) は \\( p_y(y) \\) の最大値を与えることがわかる. \\( \Box \\)

　そして上記は一般の \\( g \\) に対しては成立しない. 
例をあげることで示す. 

確率密度 \\( p_x(x) \\) と変換関数 \\( x = g(y) \\) を以下のように定義する. 

\begin{align}
p_x(x) &= \frac{1}{\sqrt{2 \pi}} e^{ -\frac{1}{2} x^2 } \\\\
g(y) &= \cases{
  y^2 + y & \text{if \\( y \geq 0 \\)} \\\\
  -y^2 + y & \text{if \\( y < 0 \\)}
}
\end{align}

このとき (1.27) より

\begin{align}
p_y(y) &= p_x(g(y)) \| g'(y) \| \\\\
       &= \cases{
            \frac{1}{\sqrt{2 \pi}} e^{ - \frac{1}{2} \left( y^2 + y \right)^2} \| 2 y + 1 \| & \text{if \\( y \geq 0 \\)} \\\\
            \frac{1}{\sqrt{2 \pi}} e^{ - \frac{1}{2} \left( -y^2 + y \right)^2} \| -2 y + 1 \| & \text{if \\( y < 0 \\)}
          } \\\\
       &= \cases{
            \frac{2 y + 1}{\sqrt{2 \pi}} e^{ - \frac{1}{2} \left( y (y + 1) \right)^2} & \text{if \\( y \geq 0 \\)} \\\\
            \frac{-2 y + 1}{\sqrt{2 \pi}} e^{ - \frac{1}{2} \left( y (y - 1) \right)^2} & \text{if \\( y < 0 \\)}
          }
\end{align}

となる. 特に \\( p_y(y) \\) は左右対称である. 

この \\( p_y(y) \\) が問の条件を満たしていること, 
つまり \\( p_x(x) \\) を最大にする \\( \widehat{x} \\) と \\( p_y(y) \\) を最大にする \\( \widehat{y} \\) は \\( \widehat{x} = g(\widehat{y}) \\) の関係には**ない**ことを示す. 

\\( p_x(x) \\) を最大にする \\( \widehat{x} \\) は明らかに \\( 0 \\) である. 
一方で \\( p_y(y) \\) を最大にする \\( \widehat{y} \\) は \\( g^{-1}(\widehat{x}) = 0 \\) ではない. 
これを示すために \\(\lim_{y \to +0} p_y'(y) > 0 \\) を示す. 
\\( y > 0 \\) に限定して \\( p_y'(y) \\) を計算すると

\begin{align}
p_y'(y) &= \left( \frac{2 y + 1}{\sqrt{2 \pi}} e^{-\frac{1}{2} \left( y(y + 1) \right)^2} \right)' \\\\
        &= \frac{2}{\sqrt{2 \pi}} e^{-\frac{1}{2} \left( y(y + 1) \right)^2} + \frac{2 y + 1}{\sqrt{2 \pi}} e^{-\frac{1}{2} \left( y(y + 1) \right)^2} \left(-\frac{1}{2} \left( y(y + 1) \right)^2 \right)' \\\\
        &= \frac{1}{\sqrt{2 \pi}} e^{-\frac{1}{2} \left( y(y + 1) \right)^2} \left( 2 + (2 y + 1) \left( -\frac{1}{2}( 4 y^3 + 6 y^2 + 2 y) \right) \right) \\\\
        &= \frac{1}{\sqrt{2 \pi}} e^{-\frac{1}{2} \left( y(y + 1) \right)^2} \left( 2 - y (y + 1) (2 y + 1)^2 \right). \ 
\end{align}

よって 
\\[
\lim_{y \to +0} p_y'(y) = \frac{1}{\sqrt{2 \pi}} \times 2 = \sqrt{\frac{2}{\pi}} > 0. \ 
\\]

つまり \\( p_y(y) \\) は \\( y \\) を \\( 0 \\) から正の方向に少しだけ動かすと値が増加するから \\( y = 0 \\) で最大値を取らない. \\( \Box \\)
