**Theorem.** Let $A$ be a set. Let $\sim$ and $\simeq$ be equivalence relations on $A$. Suppose $A/{\sim}=A/{\simeq}$. Then, $\sim$ is equal to $\simeq$.

**Proof.** Without loss of explanation, suppose $a\sim b$. Then, $a\in[b]_{\sim}$. Since $A/{\sim}=A/{\simeq}$, there is $x\in A$ such that $[b]_{\sim}=[x]_{\simeq}$. By [[Properties of Membership and Equality of Equivalence Classes]], $b\in[b]_{\sim}$, so $b\in[x]_{\simeq}$. Thus, $b\simeq x$, so $[b]_{\simeq}=[x]_{\simeq}$. We therefore have $[b]_{\sim}=[b]_{\simeq}$. Since $a\in[b]_{\sim}$, $a\in[b]_{\simeq}$, so $a\simeq b$. $\blacksquare$
***
Definitions used:
- [[Set]]
- [[Equivalence Relation]]
- [[Equivalence Class]]
- [[Quotient Set]]

Theorems used:
- [[Properties of Membership and Equality of Equivalence Classes]]