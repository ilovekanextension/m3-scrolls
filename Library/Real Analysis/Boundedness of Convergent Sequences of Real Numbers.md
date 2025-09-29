**Theorem**. Let $(x_n)$ be a sequence of real numbers that is convergent to $x$. Then, $(x_n)$ is bounded.

**Proof**. Let $n \in \mathbb{N}$. Since $x_n \to x$, there exists $K \in \mathbb{N}$ such that for all $n \ge K$, $|x_{n}-x|<1$. Notice that for all $n \ge K$, $|x_{n}| \le |x_{n} - x| + |x| < 1 + |x|$. Choose $M = \max\{|x_{1}|, |x_{2}|, \dots, |x_{K-1}|, 1+|x|\}$. Therefore $|x_n| \leq M$. $\blacksquare$ 

---
Definitions used:
- [[Sequence of Real Numbers]]
- [[Convergent Sequence of Real Numbers]]
- [[Bounded Sequence of Real Numbers]]

Theorems used:

