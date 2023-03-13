二乗和誤差関数 (1.2) は以下だった. 

\\[
E(\boldsymbol{w}) = \frac{1}{2} \sum_{n = 1}^{N} \left( y(x_n, \boldsymbol{w}) - t_n \right)^2
, \qquad \left( \text{ここで } y(x, \boldsymbol{w}) = \sum_{j = 0}^M w_j x^j \right). 
\\]

\\( E(\boldsymbol{w}) \\) を最小にする \\( \boldsymbol{w} \\) は下記を満たす. 

\\[
\frac{\partial E}{\partial w_i}(\boldsymbol{w}) = 0 \qquad \left( \text{for all } i \right). \ 
\\]

よって \\( i = 0, \dots, M \\) に対して

\begin{align}
0 &= \frac{\partial E}{\partial w_i}(\boldsymbol{w}) \\\\
  &= \sum_{n = 1}^N \frac{\partial \left( y(x_n, \boldsymbol{w}) -t_n \right)}{\partial w_i} \left( y(x_n, \boldsymbol{w}) - t_n \right) \\\\
  &= \sum_{n = 1}^N x_n^i \left( y(x_n, \boldsymbol{w}) - t_n \right) \\\\
  &= \sum_{n = 1}^N \sum_{j = 0}^M w_j x_n^{i + j} - \sum_{n = 1}^N x_n^i t_n \\\\
  &= \sum_{j = 0}^M w_j \sum_{n = 1}^N x_n^{i + j} - T_i \\\\
  &= \sum_{j = 0}^M A_{ij} w_j - T_i. 
\end{align}

従って各 \\( i = 0, \dots, M \\) に対して

\\[
\sum_{j = 0}^{M} A_{ij} w_j = T_i
\\]

が成り立つ. \\( \Box \\)
