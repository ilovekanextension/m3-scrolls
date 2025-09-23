**Theorem.** Let $R$ be a ring. Let $I$ be an ideal of $R$. By [[Normality of Subgroups of Abelian Groups]], $I$ is a normal subgroup of $R$, so we can consider the quotient group $R/I$. Denote the operation on the quotient group as $+$.
1. Suppose $a,b,x,y\in R$. Suppose that $a+I=x+I$ and $b+I=y+I$. Then, $(a\cdot b)+I=(x\cdot y)+I$. We can therefore construct an operation $\cdot:R/I\times R/I\to R/I$ defined as $$(a+I)\cdot(b+I)=(a\cdot b)+I.$$
2. The group $R/I$ together with $1+I$ and the function $\cdot$ defined on the first statement forms a ring.

**Proof of First Statement.** Since $a+I=x+I$, by [[Criterion for Equality of Cosets]] $x-a\in I$. Since $I$ is an ideal, we then have $$x\cdot b-a\cdot b=(x-a)\cdot b\in I.$$Likewise, since $b+I=y+I$, by [[Criterion for Equality of Cosets]] $y-b\in I$, so $$x\cdot y-x\cdot b=x\cdot(y-b)\in I$$We therefore have
$$\begin{align}
x\cdot y-a\cdot b & =x\cdot y+0-a\cdot b \\
 & =x\cdot y-x\cdot b+x\cdot b-a\cdot b \\
 & =x\cdot(y-b)+(x-a)\cdot b \\
 & \in I.
\end{align}$$
By [[Criterion for Equality of Cosets]], this means $(a\cdot b)+I=(x\cdot y)+I$. $\blacksquare$

**Proof of Second Statement.** We first show that $(R/I,\cdot,1+I)$ forms a ring.
- **Associativity.** Suppose $X,Y,Z\in R/I$. Then, there are $a,b,c\in R$ such that $X=a+I$, $Y=b+I$, and $Z=c+I$. We then have $$\begin{align}
(X\cdot Y)\cdot Z & =((a+I)\cdot(b+I))\cdot(c+I) \\
 & =((a\cdot b)+I)\cdot(c+I) \\
 & =((a\cdot b)\cdot c)+I \\
 & =(a\cdot(b\cdot c))+I \\
 & =(a+I)\cdot((b\cdot c)+I) \\
 & =(a+I)\cdot((b+I)\cdot(c+I)) \\
 & =X\cdot(Y\cdot Z).
\end{align}$$
- **Existence of Identity.** Suppose $X\in R/I$. Then, there is $a\in R$ such that $X=a+I$. We have $$X\cdot(1+I)=(a+I)\cdot(1+I)=(a\cdot 1)+I=a+I=X$$and $$(1+I)\cdot X=(1+I)\cdot(a+I)=(1\cdot a)+I=a+I=X.$$

We now show that $\cdot$ distributes over $+$. Suppose $X,Y,Z\in R/I$. Then, there are $a,b,c\in R$ such that $X=a+I$, $Y=b+I$, and $Z=c+I$. We then have
$$\begin{align}
X\cdot(Y+Z) & =(a+I)\cdot((b+I)+(c+I)) \\
 & =(a+I)\cdot((b+c)+I) \\
 & =(a\cdot(b+c))+I \\
 & =(a\cdot b+a\cdot c)+I \\
 & =((a\cdot b)+I)+((a\cdot c)+I) \\
 & =((a+I)\cdot(b+I))+((a+I)\cdot(c+I)) \\
 & =X\cdot Y+X\cdot Z
\end{align}$$
and
$$\begin{align}
(X+Y)\cdot Z & =((a+I)+(b+I))\cdot(c+I) \\
 & =((a+b)+I)\cdot(c+I) \\
 & =((a+b)\cdot c)+I \\
 & =(a\cdot c+b\cdot c)+I \\
 & =((a\cdot c)+I)+((b\cdot c)+I) \\
 & =((a+I)\cdot(c+I))+((b+I)\cdot(c+I)) \\
 & =X\cdot Z+Y\cdot Z.\blacksquare
\end{align}$$
***
Definitions used:
- [[Ring]]
- [[Subtraction Notation on Rings]]
- [[Ideal]]
- [[Left and Right Coset]]
- [[Normal Subgroup]]
- [[Quotient Group]]
- [[Function]]

Theorems used:
- [[Multiplications with Additive Inverses]]
- [[Criterion for Equality of Cosets]]
- [[Normality of Subgroups of Abelian Groups]]