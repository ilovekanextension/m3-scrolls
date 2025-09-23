**Theorem.** Let $A$ be a set. Then, $$A\cup\varnothing=A.$$
**Proof.** We will show that $A\cup \varnothing\subseteq A$ and $A\subseteq A\cup \varnothing$.
- **First Statement.** Suppose $x\in A\cup\varnothing$. Then, $x\in A$ or $x\in \varnothing$. We proceed by cases; in each case we show that $x\in A$.
	- **Case** $x\in A$. This is precisely what we wanted to show.
	- **Case** $x\in\varnothing$. By [[Empty Set as Subset of Any Set]], we have $\varnothing\subseteq A$, so $x\in A$. $\blacksquare$
- **Second Statement.** Suppose $x\in A$. Then, $x\in A$ or $x\in \varnothing$, so $x\in A\cup\varnothing$. $\blacksquare$

***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Empty Set]]
- [[Union of Two Sets]]

Theorems used:
- [[Empty Set as Subset of Any Set]]