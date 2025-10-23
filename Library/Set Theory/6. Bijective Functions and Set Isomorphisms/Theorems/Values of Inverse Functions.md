**Theorem.** Let $A$ and $B$ be sets. Let $f:A\to B$ be bijective. Suppose $a\in A$ and $b\in B$. Then, $f(a)=b$ if and only if $f^{-1}(b)=a$.

**Proof of Forward Implication.** By definition, we have $(b,f^{-1}(b))\in f^{-1}$. Also, since $f(a)=b$, we have $(a,b)\in f$, so $(b,a)\in f^{-1}$. This means $f^{-1}(b)=a$. $\blacksquare$

**Proof of Backward Implication.** By definition, we have $(a,f(a))\in f$. Also, since $f^{-1}(b)=a$, we have $(b,a)\in f^{-1}$, so $(a,b)\in f$. This means $f(a)=b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Inverse of Relation]]
- [[Function]]
- [[Bijective Function]]
- [[Inverse of Bijective Function]]