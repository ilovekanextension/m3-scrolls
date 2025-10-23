**Theorem.** Let $A$ be a set. Let $F:A\to\mathcal{P}(A)$ be defined as $F_{x}=\{x\}$. Then, $$A=\bigcup_{x\in A}F_{x.}$$
**Proof.** First suppose $a\in A$. By definition, $F_{a}=\{a\}$. Since $a\in\{a\}$, we have $a\in F_{a}$, so $a\in\bigcup_{x\in A}F_{x}$. Next suppose $a\in\bigcup_{x\in A}F_{x}$. Then, there is $x\in A$ such that $a\in F_{x}$. By definition, $F_{x}=\{x\}$, so $a\in\{x\}$. This means $a=x$, so since $x\in A$ we have $a\in A$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Subset]]
- [[Singleton]]
- [[Function]]
- [[Family of Subsets]]
- [[Union of Family of Sets]]