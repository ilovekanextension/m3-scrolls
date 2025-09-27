> Given $X\subseteq \Omega$, we define $X^c=\Omega-X$.
> Define $\overline{\mathbb{R}}$ as the extended real line number system.

A $\sigma$-**field** over a set $\Omega$ is a set $\mathcal{F}$ of subsets of $\Omega$ satisfying the following properties.
- $\Omega\in\mathcal{F}$ and $\varnothing\in\mathcal{F}$.
- If $X\in\mathcal{F}$ and $Y\in\mathcal{F}$, then $X\cap Y\in\mathcal{F}$.
- If $X\in\mathcal{F}$, then $X^c\in\mathcal{F}$.

As a direct consequence, if $X\in\mathcal{F}$ and $Y\in\mathcal{F}$, then $X\cup Y\in\mathcal{F}$.

A **measurable space** $(\Omega,\mathcal{F})$ consists of a set $\Omega$ and a $\sigma$-field $\mathcal{F}$ over $\Omega$.

A **measure** over a measurable space $(\Omega,\mathcal{F})$ is a function $\mu:\mathcal{F}\to \overline{\mathbb{R}}$ satisfying the following properties.
- **Non-negativity.** For all $X\in\mathcal{F}$, $\mu(X)\geq 0$.
- $\mu(\varnothing)=0$.
- **Countable Additivity.** For all countable families $\{X_{n}\}$ of pairwise disjoint sets in $\mathcal{F}$, $$\mu\left(\bigcup_{n=1}^\infty X_{n}\right)=\sum_{n=1}^\infty \mu(X_{n}).$$

A **measure space** $(\Omega,\mathcal{F},\mu)$ consists of a set $\Omega$, a $\sigma$-field $\mathcal{F}$ over $\Omega$, and a measure $\mu$ over $(\Omega,\mathcal{F})$.

A measure $\mathbb{P}$ over a measurable space $(\Omega,\mathcal{F})$ is called a **probability measure** if $\mathbb{P}(\Omega)=1$.

A measure space $(\Omega,\mathcal{F},\mathbb{P})$ in which $\mathbb{P}$ is a probability measure is called a **probability space**.
___
**Theorem.** Let $(\Omega,\mathcal{F},\mathbb{P})$ be a measure space.
1. **Complementary Events.** For all $X\in\mathcal{F}$, $$\mathbb{P}(X^c)=1-\mathbb{P}(X).$$
2. **Monotonicity.** For all $X,Y\in\mathcal{F}$, if $X\subseteq Y$, then $\mathbb{P}(X)\leq\mathbb{P}(Y)$.
3. **Boundedness.** For all $X\in\mathcal{F}$, $$\mathbb{P}(X)\in[0,1].$$
4. **Difference of Events.** For all $X,Y\in\mathcal{F}$, $$\mathbb{P}(X-Y)=\mathbb{P}(X)-\mathbb{P}(X\cap Y).$$
5. **Inclusion-Exclusion Principle.** For all $X,Y\in\mathcal{F}$, $$\mathbb{P}(X\cup Y)=\mathbb{P}(X)+\mathbb{P}(Y)-\mathbb{P}(X\cap Y).$$

*Proof.*
1. Suppose $X\in\mathcal{F}$. We have $X^c\cup X=\Omega$. Since $X^c$ and $X$ are pairwise disjoint, by countable additivity $$1=\mathbb{P}(\Omega)=\mathbb{P}(X^c\cup X)=\mathbb{P}(X^c)+\mathbb{P}(X).$$
2. Suppose $X,Y\in\mathcal{F}$. Suppose $X\subseteq Y$. Then, $X$ and $Y-X$ are pairwise disjoint. Since $X\cup(Y-X)=Y$, by countable additivity $$\mathbb{P}(Y)=\mathbb{P}(X\cup(Y-X))=\mathbb{P}(X)+\mathbb{P}(Y-X).$$By non-negativity, $\mathbb{P}(Y-X)\geq 0$. Therefore, $\mathbb{P}(Y)\geq\mathbb{P}(X)$.
3. Suppose $X\in\mathcal{F}$. Since $\varnothing\subseteq X\subseteq \Omega$, by monotonicity $$0=\mathbb{P}(\varnothing)\leq\mathbb{P}(X)\leq\mathbb{P}(\Omega)=1.$$
4. Suppose $X,Y\in\mathcal{F}$. Since $(X-Y)\cup(X\cap Y)=X$ and $(X-Y)\cap(X\cap Y)=\varnothing$, by countable additivity $$\mathbb{P}(X)=\mathbb{P}((X-Y)\cup(X\cap Y))=\mathbb{P}(X-Y)+\mathbb{P}(X\cap Y).$$
5. Suppose $X,Y\in\mathcal{F}$. $$\mathbb{P}((X\cup Y)-Y)=\mathbb{P}(X\cup Y)-\mathbb{P}((X\cup Y)\cap Y)$$

