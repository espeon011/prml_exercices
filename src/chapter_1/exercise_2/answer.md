式 (1.4) は以下だった. 

\\[
\widetilde{E} (\boldsymbol{w}) = \frac{1}{2} \sum_{n = 1}^N \left( y(x_n, \boldsymbol{w}) - t_n \right)^2 + \frac{\lambda}{2} \\| \boldsymbol{w} \\|^2. \ 
\\]

\\( \widetilde{E} \\) が最小値を取る時, 各 \\( i = 0, \dots, M \\) に対して下記が成り立つ. 

\\[
\frac{\partial \widetilde{E}}{\partial w_i}(\boldsymbol{w})= 0. \ 
\\]

よって

\begin{align}
0 &= \frac{\partial \widetilde{E}}{\partial w_i}(\boldsymbol{w}) \\\\
  &= \frac{\partial}{\partial w_i} \left( E(\boldsymbol{w}) + \frac{\lambda}{2} \\| \boldsymbol{w} \\|^2 \right) \\\\
  &= \sum_{j = 0}^M A_{ij} w_j -T_i + \frac{\lambda}{2} \frac{\partial}{\partial w_i} \left( w_1^2 + \dots + w_M^2 \right) \\\\
  &= \sum_{j = 0}^M A_{ij} w_j -T_i + \lambda w_i
\end{align}

が成り立つ(ここで, \\( A_{ij} \\), \\( T_i \\) は演習問題 1.1 で定めたものとする).
従って各 \\( i = 0, \dots, M \\) に対して以下が成り立つ. 

\\[
\sum_{j = 0}^M \left( A_{ij} + \lambda \delta_{ij} \right) w_j = T_i
\\]

ただしここで \\( \delta_{ij} \\) は Kronecker のデルタとする. \\( \Box \\)
