$D=\sum(y_{i}-(a_{0}+a_{1}x_{i}))^2=\sum y_{i}^2-2y_{i}(a_{0}+a_{1}x_{i})+(a_{0}+a_{1}x_{i})^2$.

$$\begin{align}
&& \frac{\partial D}{\partial a_{0}} &=0 &  \\
\Rightarrow &&\sum(-2y_{i}+2(a_{0}+a_{1}x_{i})) & =0 \\
\Rightarrow &&\sum(-y_{i}+a_{0}+a_{1}x_{i}) & =0 \\
\Rightarrow &&\sum(-y_{i})+\sum(a_{0})+\sum (a_{1}x_{i}) & =0 \\
\Rightarrow &&n\cdot a_{0} +\sum(a_{1}x_{i})& =\sum y_{i} \\
\Rightarrow &&n\cdot a_{0}+a_{1}\sum x_{i} & =\sum y_{i}
\end{align}$$

$$\begin{align}
&& \frac{\partial D}{\partial a_{1}} & =0 \\
\Rightarrow && \sum(-2y_{i}x_{i})+2x_{i}(a_{0}+a_{1}x_{i}) & =0 \\
\Rightarrow && \sum(-y_{i}x_{i}+x_{i}(a_{0}+a_{1}x_{i})) & =0 \\
\Rightarrow && \sum(a_{0}x_{i})+\sum a_{1}x_{i}^2 & = \sum y_{i}x_{i} \\
\Rightarrow && a_{0}\sum x_{i}+a_{1}\sum x_{i}^2 & =\sum y_{i}x_{i}
\end{align}$$


| data         |     |     |     |     |      |     |      | sum |
| ------------ | --- | --- | --- | --- | ---- | --- | ---- | --- |
| $x_{i}$      | 1   | 2   | 3   | 4   | 5    | 6   | 7    | 28  |
| $y_{i}$      | 0.5 | 2.5 | 2   | 4   | 3.5  | 6   | 5.5  |     |
| $x_{i}y_{i}$ | 0.5 | 5   | 6   | 16  | 17.5 | 36  | 38.5 |     |
