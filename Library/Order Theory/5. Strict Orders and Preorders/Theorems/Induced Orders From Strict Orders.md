**Theorem.** Let $A$ be a set. Let $<$ be a strict order on $A$.
1. The relation $\leq$ on $A$ defined as $$a\leq b\iff a<b\vee a=b$$is a partial order on $A$.
2. Suppose that $<$ is a strict total order. Then, the relation $\leq$ on $A$ defined on the first statement is a total order.

**Proof of First Statement.**
- **Reflexivity.** Suppose $a\in A$. Then, by reflexivity $a=a$, so $a=a$ or $a<a$. By definition, this means $a\leq a$.
- **Antisymmetry.** Suppose $a,b\in A$, and suppose that $a\leq b$ and $b\leq a$. Then, $a<b$ or $a=b$, and $b<a$ or $b=a$. We proceed by cases on the first disjunction; in each case we will show that $a=b$.
	- **Case** $a<b$. We will first show that $\neg(b<a)$. Assume for the sake of negation that $b<a$. Then, $a<b$ and $b<a$. Since $<$ is a strict order, it is transitive, so $a<a$. This contradicts the fact that $<$ is irreflexive. Therefore, the assumption that $b<a$ is false, so $\neg(b<a)$. Now, by the second disjunction, $b<a$ or $b=a$, so we must have $b=a$.
	- **Case** $a=b$. This is precisely what we wanted to show.
- **Transitivity.** Suppose $a,b,c\in A$, and suppose that $a\leq b$ and $b\leq c$. Then, $a<b$ or $a=b$, and $b<c$ or $b=c$. We proceed by cases on the first disjunction; in each case we will show that $a\leq c$.
	- **Case** $a<b$. By the second disjunction, $b<c$ or $b=c$. If $b<c$, then by transitivity of $<$ we have $a<c$. This means $a<c$ or $a=c$, so by definition $a\leq c$. If $b=c$, then since $a<b$ we must have $a<c$. This means $a<c$ or $a=c$, so $a\leq c$.
	- **Case** $a=b$. By the second disjunction, $b<c$ or $b=c$. If $b<c$, then since $a=b$ we have $a<c$. This means $a<c$ or $a=c$, so $a\leq c$. If $b=c$, then by transitivity $a=c$, so $a<c$ or $a=c$, which means $a\leq c$. $\blacksquare$

**Proof of Second Statement.** By the first statement, $\leq$ is already a partial order. We will show that $\leq$ is also connected.

Suppose $a,b\in A$. Since $<$ is a strict total order, we have $a<b$ or $b<a$ or $a=b$. We proceed by cases; in each case we will show that $a\leq b$ or $b\leq a$.
- **Case** $a<b$. This means $a<b$ or $a=b$, so $a\leq b$.
- **Case** $b<a$. This means $b<a$ or $b=a$, so $b\leq a$.
- **Case** $a=b$. This means $a<b$ or $a=b$, so $a\leq b$. $\blacksquare$

***
Definitions used:
- [[Partial Order]]
- [[Total Order]]
- [[Strict Order]]
- [[Strict Total Order]]
- [[Set]]