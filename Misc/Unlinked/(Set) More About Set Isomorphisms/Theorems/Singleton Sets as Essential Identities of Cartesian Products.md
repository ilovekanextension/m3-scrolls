*Theorem.* Let $A$ be a set. Let $1$ be a singleton set $\{*\}$. Then, $A$ is isomorphic to the Cartesian Product $A\times 1$. That is, $$A\cong A\times 1.$$
*Proof.* Define a function $f:A\to A\times 1$ as follows: $$f(a)=(a,*).$$We will show that $f$ is bijective; the statement in the theorem follows immediately.
- *Injectivity.* Suppose $a,b\in A$, and suppose that $f(a)=f(b)$. Then, by definition of $f$, we have $(a,*)=(b,*)$, so $a=b$.
- *Surjectivity.* Suppose $(a,*)\in A\times 1$. We have $f(a)=(a,*)$. $\blacksquare$