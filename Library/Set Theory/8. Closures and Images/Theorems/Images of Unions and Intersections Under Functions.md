**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Suppose $F:I\to\mathcal{P}(A)$ is a family of subsets of $A$. Then, $$f\left[\bigcup_{\alpha\in I}F_{\alpha}\right]=\bigcup_{\alpha\in I}f[F_{\alpha}]$$and $$f\left[\bigcap_{\alpha\in I}F_{\alpha}\right]\subseteq \bigcap_{\alpha\in I}f[F_{\alpha}].$$

**Proof of First Statement.** First suppose $x\in f[\bigcup_{\alpha\in I}F_{\alpha}]$. Then, there is $a\in\bigcup_{\alpha\in I}F_{\alpha}$ such that $x=f(a)$. Since $a\in \bigcup_{\alpha\in I}F_{\alpha}$, there is $\alpha\in I$ such that $a\in F_{\alpha}$. Since $x=f(a)$ and $a\in F_{\alpha}$, by definition $x\in f[F_{\alpha}]$. Therefore, $x\in\bigcup_{\alpha\in I}f[F_{\alpha}]$.

Next suppose $x\in\bigcup_{\alpha\in I}f[F_{\alpha}]$. Then, there is $\alpha\in I$ such that $x\in f[F_{\alpha}]$. By definition, this means there is $a\in F_{\alpha}$ such that $x=f(a)$. Since $a\in F_{\alpha}$, we have $a\in\bigcup_{\alpha\in I}F_{\alpha}$. Therefore, since $x=f(a)$, we have $x\in f[\bigcup_{\alpha\in I}F_{\alpha}]$. $\blacksquare$

**Proof of Second Statement.** Suppose $x\in f[\bigcap_{\alpha\in I}F_{\alpha}]$. Then, there is $a\in\bigcap_{\alpha\in I}F_{\alpha}$ such that $x=f(a)$. Since $a\in\bigcap_{\alpha\in I}F_{\alpha}$, for all $\alpha\in I$ we have $a\in F_{\alpha}$. Therefore, since $x=f(a)$, we can conclude that for all $\alpha\in I$ we have $x\in f[F_{\alpha}]$, so $x\in\bigcap_{\alpha\in I}f[F_{\alpha}]$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Function]]
- [[Image of Subset]]
- [[Family of Subsets]]
- [[Union of Family of Sets]]
- [[Intersection of Family of Sets]]