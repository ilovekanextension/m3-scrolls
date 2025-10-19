**Theorem.**
1. Let $m,n\in \mathbb{N}$. Then, $m\leq n$ if and only if there is $k\in \mathbb{N}$ such that $n=m+k$.
2. Let $m,n\in \mathbb{N}$. Then, $m<n$ if and only if there is $k\in \mathbb{N}-\{0\}$ such that $n=m+k$.

**Proof of First Statement.**
- **Forward Implication.** Define a proposition $\varphi$ on $\mathbb{N}$ as $$\varphi(y):\equiv \forall x\in \mathbb{N} \ (x\leq y\Rightarrow \exists k\in \mathbb{N} \ (y=x+k)).$$To prove the forward implication, it is enough to show that $\varphi(y)$ is true when $y=n$. We will show by [[Principle of Mathematical Induction]] that $\varphi(y)$ is actually true for all $y\in \mathbb{N}$.
	- **Base Case.** Suppose $x\in \mathbb{N}$, and suppose that $x\leq 0$. Then, by [[Zero as Minimal Natural Number]] $x=0$. Picking $k=0$, we have $$0=0+0=x+k.$$Therefore, $\varphi(0)$ is true.
	- **Induction Step.** Suppose $y\in \mathbb{N}$, and suppose that $\varphi(y)$ is true. Suppose $x\in \mathbb{N}$, and suppose that $x\leq y+1$. Then, by definition $x=y+1$ or $x<y+1$. We proceed by cases; in each case we will show that $\varphi(y+1)$ is true.
		- **Case** $x=y+1$. Pick $k=0$. We have $$y+1=x=x+0=x+k.$$Therefore, $\varphi(y+1)$ is true.
		- **Case** $x<y+1$. By [[Discreteness of Natural Numbers]], this means $x\leq y$. Since $\varphi(y)$ is true and $x\leq y$, there is $k\in \mathbb{N}$ such that $y=x+k$. This means $$y+1=(x+k)+1=x+(k+1).$$Therefore, $\varphi(y+1)$ is true. $\blacksquare$
- **Backward Implication.** Suppose there is $k\in \mathbb{N}$ such that $n=m+k$. By [[Zero as Smallest Natural Number]], $0\leq k$, so by the first order property of real numbers $$m=m+0\leq m+k=n.\blacksquare$$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $m<n$. Then, $m\leq n$, so by the first statement there is $k\in \mathbb{N}$ such that $n=m+k$. To prove that there is $k\in \mathbb{N}-\{0\}$ such that $n=m+k$, it is enough to show that $k\neq 0$. To do this, assume for the sake of negation that $k=0$. Then, $m=n+0=n$. However, by assumption $m<n$. This contradicts the fact that $<$ is trichotomous. $\blacksquare$
- **Backward Implication.** Suppose there is $k\in \mathbb{N}-\{0\}$ such that $n=m+k$. Since $k\in \mathbb{N}-\{0\}$, by definition $k\in \mathbb{N}$, so by the first statement $m\leq n$. To prove that $m<n$, it is enough to show that $m\neq n$. To do this, assume for the sake of negation that $m=n$. Then, $$m+0=m=m+k,$$so by [[Cancellation Properties on Groups]] $k=0$. This contradicts the fact that $k\in \mathbb{N}-\{0\}$. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]
- [[Real Numbers]]
- [[Difference of Sets]]

Theorems used:
- [[Principle of Mathematical Induction]]
- [[Zero as Smallest Natural Number]]
- [[Zero as Minimal Natural Number]]
- [[Discreteness of Natural Numbers]]
- [[Cancellation Properties on Groups]]