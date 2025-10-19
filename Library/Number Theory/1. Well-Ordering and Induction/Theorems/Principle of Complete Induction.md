**Theorem.** Let $\varphi$ be a proposition on $\mathbb{N}$. Suppose that
- $\varphi(0)$ is true and
- for all $n\in \mathbb{N}$, if $\varphi(m)$ is true for all $m\in \mathbb{N}$ satisfying $m\leq n$, then $\varphi(n+1)$ is also true.

Then, $\varphi(n)$ is true for all $n\in \mathbb{N}$.

This is called the **Principle of Complete Induction**.

**Proof.** Define a proposition $\theta$ on $\mathbb{N}$ as $$\theta(n):\equiv \forall m\in \mathbb{N} \ (m\leq n\Rightarrow \varphi(m)).$$We will first show by [[Principle of Mathematical Induction]] that $\theta(n)$ is true for all $n\in \mathbb{N}$.
- **Base Case.** Suppose $m\in \mathbb{N}$, and suppose that $m\leq 0$. Then, by [[Zero as Minimal Natural Number]] $m=0$. By definition, $\varphi(0)$ is true, so $\varphi(m)$ is true. Therefore, $\theta(0)$ is true.
- **Induction Step.** Suppose $n\in \mathbb{N}$, and suppose that $\theta(n)$ is true. Suppose $m\in \mathbb{N}$, and suppose that $m\leq n+1$. Then, by definition $m=n+1$ or $m<n+1$. We proceed by cases; in each case we will show that $\varphi(m)$ is true.
	- **Case** $m=n+1$. Since $\theta(n)$ is true, for all $x\in \mathbb{N}$ with $x\leq n$ we have that $\varphi(x)$ is true. By definition of $\varphi$, this means $\varphi(n+1)$ is true, so $\varphi(m)$ is true.
	- **Case** $m<n+1$. By [[Discreteness of Natural Numbers]], this means $m\leq n$. Since $\theta(n)$ is true and $m\leq n$, this means $\varphi(m)$ is true.

Now suppose $n\in \mathbb{N}$. Then, by the previous observation $\theta(n)$ is true, so for all $m\in \mathbb{N}$ satisfying $m\leq n$ we have that $\varphi(m)$ is true. In particular, since $\leq$ is reflexive and $n\in \mathbb{N}$, we have $n\leq n$, so $\varphi(n)$ is true. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Zero as Minimal Natural Number]]
- [[Discreteness of Natural Numbers]]