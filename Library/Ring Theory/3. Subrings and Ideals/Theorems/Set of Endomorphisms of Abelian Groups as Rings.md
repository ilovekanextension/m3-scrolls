**Theorem.** Let $G=(G,0,+,-(-))$ be an abelian group. Let $S$ be the set of all group homomorphisms $G\to G$.
1. Suppose $\phi:G\to G$ and $\eta:G\to G$ are group homomorphisms. Then, the function $\pi:G\to G$ defined as $$\pi(a)=\phi(a)+\eta(a)$$is a group homomorphism. We can therefore construct an operation $+:S\times S\to S$ defined as $$(\phi+\eta)(a)=\phi(a)+\eta(a).$$
2. Suppose $\phi:G\to G$ is a group homomorphism. Then, the function $\pi:G\to G$ defined as $$\pi(a)=-\phi(a)$$is a group homomorphism. We can therefore construct a function $-(-):S\to S$ defined as $$(-\phi)(a)=-\phi(a).$$
3. The set $S$ together with the group homomorphism $0_{S}:G\to G$ defined as $$0_{S}(a)=0,$$the identity group homomorphism $\text{id}_{G}$, the operation $+:S\to S$ defined on the first statement, the composition operation $\circ$, and the function $-(-):S\to S$ defined on the second statement is a ring.

**Proof of First Statement.** Suppose $a,b\in G$. We have
$$\begin{align}
\pi(a+b) & =\phi(a+b)+\eta(a+b) \\
 & =\phi(a)+\phi(b)+\eta(a)+\eta(b) \\
 & =\phi(a)+\eta(a)+\phi(b)+\eta(b) \\
 & =\pi(a)+\pi(b).\blacksquare
\end{align}$$

**Proof of Second Statement.** Suppose $a,b\in G$. By [[Inverses of Group Compositions]], 
$$\begin{align}
\pi(a+b) & =-\phi(a+b) \\
 & =-\phi(a)+(-\phi(b)) \\
 & =\pi(a)+\pi(b).\blacksquare
\end{align}$$

**Proof of Third Statement.** We first show that $(S,+,0_{S},-(-))$ is a group.
- **Associativity.** Suppose $\phi,\eta,$ and $\pi$ are group homomorphisms $G\to G$. For all $a\in G$, $$\begin{align}
((\phi+\eta)+\pi)(a) & =(\phi+\eta)(a)+\pi(a) \\
 & =(\phi(a)+\eta(a))+\pi(a) \\
 & = \phi(a)+(\eta(a)+\pi(a)) \\
 & =\phi(a)+(\eta+\pi)(a) \\
 & =(\phi+(\eta+\pi))(a),
\end{align}$$so by [[Extensionality of Functions]] $(\phi+\eta)+\pi=\phi+(\eta+\pi)$.
- **Existence of Identity.** Suppose $\phi:G\to G$ is a group homomorphism. For all $a\in G$, $$\begin{align}
(\phi+0_{S})(a) & =\phi(a)+0_{S}(a) \\
 & =\phi(a)+0 \\
 & =\phi (a)
\end{align}$$and $$\begin{align}
(0_{S}+\phi)(a) & =0_{S}(a)+\phi(a) \\
 & =0+\phi(a) \\
 & =\phi(a),
\end{align}$$so by [[Extensionality of Functions]] $\phi+0_{S}=0_{S}+\phi=\phi$.
- **Existence of Inverses.** Suppose $\phi:G\to G$ is a group homomorphism. For all $a\in G$, $$\begin{align}
(\phi+(-\phi))(a) & =\phi(a)+(-\phi)(a) \\
 & =\phi(a)+(-\phi(a)) \\
 & =0 \\
 & =0_{S}(a)
\end{align}$$and $$\begin{align}
(-\phi+\phi)(a) & =(-\phi)(a)+\phi(a) \\
 & =(-\phi(a))+\phi(a) \\
 & =0 \\
 & =0_{S}(a),
\end{align}$$so by [[Extensionality of Functions]] $\phi+(-\phi)=-\phi+\phi=0_{S}$.

Next we show that $(S,\circ,1)$ is a monoid.
- **Associativity.** This follows by [[Associativity of Relation Composition]].
- **Existence of Identity.** This follows by [[Compositions with Identity Functions]].

Finally, we show that $\circ$ distributes over $+$. Suppose $\phi,\eta,$ and $\pi$ are group homomorphisms $G\to G$. By [[Evaluations of Composite Functions]]. for all $a\in G$ we have
$$\begin{align}
(\phi\circ(\eta+\pi))(a) & =\phi((\eta+\pi)(a)) \\
 & =\phi(\eta(a)+\pi(a)) \\
 & =\phi(\eta(a))+\phi(\pi(a)) \\
 & =\phi\circ\eta(a)+\phi\circ\pi(a) \\
 & =(\phi\circ \eta+\phi\circ\pi)(a)
\end{align}$$
and
$$\begin{align}
((\phi+\eta)\circ\pi)(a) & =(\phi+\eta)(\pi(a)) \\
 & =\phi(\pi(a))+\eta(\pi(a)) \\
 & =\phi\circ\pi(a)+\eta\circ\pi(a) \\
 & =(\phi\circ\pi+\eta\circ\pi)(a),
\end{align}$$
so by [[Extensionality of Functions]] $\phi\circ(\eta+\pi)=\phi\circ\eta+\phi\circ\pi$ and $(\phi+\eta)\circ\pi=\phi\circ\pi+\eta\circ\pi$. $\blacksquare$
***
Definitions used:
- [[Ring]]
- [[Group]]
- [[Abelian Group]]
- [[Group Homomorphism]]
- [[Monoid]]
- [[Function]]
- [[Composition of Functions]]

Theorems used:
- [[Associativity of Relation Composition]]
- [[Extensionality of Functions]]
- [[Evaluations of Composite Functions]]
- [[Compositions with Identity Functions]]
- [[Inverses of Group Compositions]]