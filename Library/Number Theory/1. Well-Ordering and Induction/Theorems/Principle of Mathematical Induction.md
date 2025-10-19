**Theorem.** Let $\varphi$ be a proposition on $\mathbb{N}$. Suppose that
- $\varphi(0)$ is true and
- for all $n\in \mathbb{N}$, if $\varphi(n)$ is true, then $\varphi(n+1)$ is also true.

Then, $\varphi(n)$ is true for all $n\in \mathbb{N}$. 

This is called the **Principle of Mathematical Induction**. A proof of truth of $\varphi$ for all $n\in \mathbb{N}$ in this way is called a **proof by induction.** The proof that $\varphi(0)$ is true is called the proof of the **base case**, and the proof that $\varphi(n+1)$ is true whenever $\varphi(n)$ is true is called the proof of the **induction step**.

**Proof.** Define a set $S\subseteq \mathbb{N}$ as $$S=\{n\in \mathbb{N}\mid\varphi(n)\}.$$To show that $\varphi(n)$ is true for all $n\in \mathbb{N}$, we can show that $S=\mathbb{N}$. Since $S\subseteq \mathbb{N}$, we then only need to show that $N\subseteq S$. By definition of $\mathbb{N}$, it is therefore enough to show that
- $0\in S$ and
- for all $n\in \mathbb{N}$, if $n\in S$ then $n+1\in S$.

Using the definition of $S$, these are equivalent to
- $\varphi(0)$ is true and
- for all $n\in \mathbb{N}$, if $\varphi(n)$ is true, then $\varphi(n+1)$ is also true,

which are precisely the given assumptions. $\blacksquare$
***
Definitions used:
- [[Natural Numbers]]
- [[Set]]
- [[Subset]]
- [[Set Builder Notation]]