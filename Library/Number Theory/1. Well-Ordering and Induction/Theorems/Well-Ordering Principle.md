**Theorem.** Let $S$ be a nonempty subset of $\mathbb{N}$. Then, $S$ has a smallest object. That is, there is $n\in S$ such that for all $m\in S$ we have $n\leq m$.

This is called the **Well-Ordering Principle**.

**Proof.** For the sake of contradiction, assume that $S$ has no smallest object. Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(n):\equiv \forall m\in \mathbb{N} \ (m\leq n\Rightarrow m\notin S).$$We will first show by [[Principle of Mathematical Induction]] that $\varphi(n)$ is true for all $n\in \mathbb{N}$.
- **Base Case.** Suppose $m\in \mathbb{N}$, and suppose that $m\leq 0$. Then, by [[Zero as Minimal Natural Number]] $m=0$. We want to show that $m\notin S$. To do this, assume for the sake of negation that $m\in S$. Then, $0\in S$. By [[Zero as Smallest Natural Number]], for all $n\in \mathbb{N}$ we have $0\leq n$. Since $S\subseteq \mathbb{N}$, this means for all $n\in S$ we have $0\leq n$. Since $0\in S$, $0$ is then the smallest object of $S$, which contradicts the fact that $S$ has no smallest object. Therefore, $m\notin S$. We can conclude that $\varphi(0)$ is true.
- **Induction Step.** Suppose $n\in \mathbb{N}$, and suppose that $\varphi(n)$ is true. Suppose $m\in \mathbb{N}$, and suppose that $m\leq n+1$. Then, by definition $m=n+1$ or $m<n+1$. We proceed by cases; in each case we will show that $m\notin S$.
	- **Case** $m=n+1$. Assume for the sake of negation that $m\in S$. We will first show that $m$ is a minimal object of $S$.
	  
	  Suppose $x\in S$, and suppose that $x\leq m$. Then, $x\leq n+1$, so $x=n+1$ or $x<n+1$. We will show that $\neg(x<n+1)$; from this we have $x=n+1$, so $x=m$. Assume for the sake of negation that $x<n+1$. Then, by [[Discreteness of Natural Numbers]] $x\leq n$. Since $\varphi(n)$ is true and $x\leq n$, we have $x\notin S$. This contradicts the fact that $x\in S$.
	  
	  Since $m$ is a minimal object of $S$ and $\leq$ is a total order, by [[Minimal Objects Under Total Orders as Smallest Objects]] $m$ is the smallest object of $S$, which contradicts the fact that $S$ has no smallest object. Therefore, $m\notin S$.
	- **Case** $m<n+1$. By [[Discreteness of Natural Numbers]], this means $m\leq n$. Since $\varphi(n)$ is true and $m\leq n$, we have $m\notin S$.

Since $S$ is nonempty, there is $x\in \mathbb{N}$ such that $x\in S$. By the previous observation, $\varphi(n)$ is true for all $n\in \mathbb{N}$, so in particular $\varphi(x)$ is true. This means for all $m\in \mathbb{N}$ satisfying $m\leq x$ we have $m\notin S$. In particular, since $\leq$ is reflexive and $x\in \mathbb{N}$, we have $x\leq x$, so $x\notin S$. This contradicts the fact that $x\in S$. Therefore, the assumption that $S$ has no smallest object must be false, so $S$ has a smallest object. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]
- [[Nonempty Set]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Zero as Smallest Natural Number]]
- [[Zero as Minimal Natural Number]]
- [[Discreteness of Natural Numbers]]
- [[Minimal Objects Under Total Orders as Smallest Objects]]