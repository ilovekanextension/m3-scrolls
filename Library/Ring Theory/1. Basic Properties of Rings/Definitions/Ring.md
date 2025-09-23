**Definition.** A **ring** consists of
- a set $R$,
- objects $0,1\in R$,
- operations $+:R\times R\to R$ and $\cdot:R\times R\to R$, and
- a function $-(-):R\to R$

satisfying the following properties.
1. $(R,+,0,-(-))$ is an abelian group.
2. $(R,\cdot,1)$ is a monoid.
3. **Left Distributivity.** For all $a,b,c\in R$, $$a\cdot(b+c)=a\cdot b+a\cdot c.$$
4. **Right Distributivity.** For all $a,b,c\in R$, $$(a+b)\cdot c=a\cdot c+b\cdot c.$$

By [[Commutativity of Additive Groups of Rings]], the abelian property of $(R,+)$ can be deduced from the other properties. Therefore, it is enough to mention $(R,+)$ as a group.

The objects $0$ and $1$ are called **zero** and **one** respectively. An object $a\in R$ with $a\neq 0$ is called a **nonzero** object.
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Group]]
- [[Abelian Group]]
- [[Monoid]]