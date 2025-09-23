*Theorem.* Let $A$ be a set. Let $2$ be the set $\{0,1\}$. Then, the Cartesian Product $A\times 2$ is isomorphic to the disjoint union $A+A$. That is, $$A\times 2\cong A+A.$$
*Proof.* Define a function $f:A\times 2\to A+A$ as follows: $$f(a,n)=\begin{cases}
(a,x_{A_{1}}), & n=0, \\
(a,x_{A_{2}}), & n=1.
\end{cases}$$We will show that $f$ is bijective; the statement in the theorem follows immediately.
- *Injectivity.* Suppose $(a,m)\in A\times 2$ and $(b,n)\in A\times 2$, and suppose that $f(a,m)=f(b,n)$. Then, $m=0$ or $m=1$. We proceed by cases; in each case we will show that $(a,m)=(b,n)$.
	- *Case* $m=0$. By definition of $f$, we have $(a,x_{A_{1}})=f(b,n)$. Since $x_{A_{1}}$ and $x_{A_{2}}$ are distinct, we must have $n=0$, so $(a,x_{A_{1}})=(b,x_{A_{1}})$. This means $a=b$, so $(a,0)=(b,0)$ and thus $(a,m)=(b,n)$.
	- *Case* $m=1$. By definition of $f$, we have $(a,x_{A_{2}})=f(b,n)$. Since $x_{A_{1}}$ and $x_{A_{2}}$ are distinct, we must have $n=1$, so $(a,x_{A_{2}})=(b,x_{A_{2}})$. This means $a=b$, so $(a,1)=(b,1)$ and thus $(a,m)=(b,n)$.
- *Surjectivity.* Suppose $(a,x)\in A+A$. Then, $(a,x)\in A\times\{x_{A_{1}}\}$ or $(a,x)\in A\times\{x_{A_{2}}\}$. We proceed by cases; in each case we will show that $(a,x)=f(b,n)$ for some $b\in A$ and $n\in\{0,1\}$.
	- *Case* $(a,x)\in A\times\{x_{A_{1}}\}$. We have $a\in A$ and $x=x_{A_{1}}$. Consider $(a,0)\in A\times 2$. We have $f(a,0)=(a,x_{A_{1}})=(a,x)$.
	- *Case* $(a,x)\in A\times\{x_{A_{2}}\}$. We have $a\in A$ and $x=x_{A_{2}}$. Consider $(a,1)\in A\times 2$. We have $f(a,1)=(a,x_{A_{2}})=(a,x)$. $\blacksquare$