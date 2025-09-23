**Theorem.** Let $G$ be a group. Let $S$ be a subgroup of $G$. Suppose $g,h\in G$.
1. $g\circ S=h\circ S$ if and only if $g^{-1}\circ h\in S$.
2. $S\circ g=S\circ h$ if and only if $g\circ h^{-1}\in S$.

**Proof of First Statement.**
- **Forward Implication.** Suppose $g\circ S=h\circ S$. Since $S$ is a subgroup, $1\in S$, so $h=h\circ 1\in h\circ S$. This means $h\in g\circ S$, so there is $s\in S$ such that $h=g\circ s$. We then have $g^{-1}\circ h=s\in S$. $\blacksquare$
- **Backward Implication.** Suppose $g^{-1}\circ h\in S$. Then, there is $s\in S$ such that $g^{-1}\circ h=s$. This means $h=g\circ s$.
  
  First suppose $x\in g\circ S$. Then, there is $t\in S$ such that $x=g\circ t$. This means $$x=h\circ s^{-1}\circ t=h\circ(s^{-1}\circ t)\in h\circ S.$$Next suppose $x\in h\circ S$. Then, there is $t\in S$ such that $x=h\circ t$. This means $$x=g\circ s\circ t=g\circ(s\circ t)\in g\circ S.\blacksquare$$

**Proof of Second Statement.**
- **Forward Implication.** Suppose $S\circ g=S\circ h$. Since $S$ is a subgroup, $1\in S$, so $g=1\circ g\in S\circ g$. This means $g\in S\circ h$, so there is $s\in S$ such that $g=s\circ h$. We then have $g\circ h^{-1}=s\in S$. $\blacksquare$
- **Backward Implication.** Suppose $g\circ h^{-1}\in S$. Then, there is $s\in S$ such that $g\circ h^{-1}=s$. This means $g=s\circ h$.
  
  First suppose $x\in S\circ g$. Then, there is $t\in S$ such that $x=t\circ g$. This means $$x=t\circ s\circ h=(t\circ s)\circ h\in S\circ h.$$Next suppose $x\in S\circ h$. Then, there is $t\in S$ such that $x=t\circ h$. This means $$x=t\circ s^{-1}\circ g=(t\circ s^{-1})\circ g\in S\circ g.\blacksquare$$

***
Definitions used:
- [[Group]]
- [[Subgroup]]
- [[Left and Right Coset]]