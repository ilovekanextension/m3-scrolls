**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$. Suppose $F:I\to\mathcal{P}(B)$ is a family of subsets of $B$. Then, $$f^{-1}\left[\bigcup_{\alpha\in I}F_{\alpha}\right]=\bigcup_{\alpha\in I}f^{-1}[F_{\alpha}]$$and $$f^{-1}\left[\bigcap_{\alpha\in I}F_{\alpha}\right]=\bigcap_{\alpha\in I}f^{-1}[F_{\alpha}].$$

**Proof of First Statement.** First suppose $x\in f^{-1}[\bigcup_{\alpha\in I}F_{\alpha}]$. Then, $f(x)\in\bigcup_{\alpha\in I}F_{\alpha}$, so we can choose $\alpha\in I$ such that $f(x)\in F_{\alpha}$. This means $x\in f^{-1}[F_{\alpha}]$, so $x\in\bigcup_{\alpha\in I}f^{-1}[F_{\alpha}]$.

Next suppose $x\in\bigcup_{\alpha\in I}f^{-1}[F_{\alpha}]$. Then, we can choose $\alpha\in I$ such that $x\in f^{-1}[F_{\alpha}]$. By definition, this means $f(x)\in F_{\alpha}$, so$f(x)\in\bigcup_{\alpha\in I}F_{\alpha}$. Therefore, $x\in f^{-1}[\bigcup_{\alpha\in I}F_{\alpha}]$. $\blacksquare$

**Proof of Second Statement.** First suppose $x\in f^{-1}[\bigcap_{\alpha\in I}F_{\alpha}]$. Then, $f(x)\in\bigcap_{\alpha\in I}F_{\alpha}$, so for all $\alpha\in I$ we have $f(x)\in F_{\alpha}$. Thus, for all $\alpha\in I$ we have $x\in f^{-1}[F_{\alpha}]$, so $x\in\bigcap_{\alpha\in I}f^{-1}[F_{\alpha}]$.

Next suppose $x\in\bigcap_{\alpha\in I}f^{-1}[F_{\alpha}]$. Then, for all $\alpha\in I$ we have $x\in f^{-1}[F_{\alpha}]$. Thus, for all $\alpha\in I$ we have $f(x)\in F_{\alpha}$, so $f(x)\in\bigcap_{\alpha\in I}F_{\alpha}$. Therefore, $x\in f^{-1}[\bigcap_{\alpha\in I}F_{\alpha}]$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Function]]
- [[Preimage of Subset]]
- [[Family of Subsets]]
- [[Union of Family of Sets]]
- [[Intersection of Family of Sets]]

