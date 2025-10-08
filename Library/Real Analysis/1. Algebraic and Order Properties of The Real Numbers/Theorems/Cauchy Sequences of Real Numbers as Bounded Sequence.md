**Theorem.** A cauchy sequence of real numbers are bounded.

**Proof**. Let $(x_{n})$ be a cauchy sequence. Then, for $\varepsilon = 1$, we have $N$ such that for all $m, n \ge N, |x_{n}-x_{m}|< 1$. Therefore we have for all $n \ge N, |x_{n}-x_{N}| < 1$. Then, by the triangle inequality, we have that $|x_n| \le |x_{n}-x_{N}| + |x_{N}| < 1 + |x_N|$ for all $n \ge N$. Therefore, we have the bound $M = \sup \{ |x_{1}|, |x_{2}|, \dots, |x_{N-1}|, 1 + |x_{n}|\}$, and thus $(x_n)$ is bounded.

---
Definitions used:

Theorems used:

