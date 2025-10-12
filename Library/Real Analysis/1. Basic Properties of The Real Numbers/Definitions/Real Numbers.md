**Definition.** We axiomatically define the mathematical structure of **real numbers** as a structure consisting of
- a set $\mathbb{R}$ of **real numbers**,
- objects $0\in \mathbb{R}$ and $1\in \mathbb{R}$ called **zero** and **one** respectively,
- two operations $+:\mathbb{R}\times \mathbb{R}\to \mathbb{R}$ and $\cdot:\mathbb{R}\times \mathbb{R}\to \mathbb{R}$ called **addition** and **multiplication** respectively,
- a function $-(-):\mathbb{R}\times \mathbb{R}\to \mathbb{R}$ mapping a real number to its **additive inverse**, and
- a strict total order $<$ on $\mathbb{R}$ inducing a total order $\leq$ (see [[Induced Orders From Strict Orders]]) on $\mathbb{R}$

satisfying the following properties.
1. **Algebraic Property.** The structure $(\mathbb{R},+,\cdot,0,1,-(-))$ is a field.
2. **Order Property.** We have the following properties:
	- For all $a,b,c\in \mathbb{R}$, if $a<b$, then $a+c<b+c$.
	- For all $a,b,c\in \mathbb{R}$, if $a<b$ and $0<c$, then $a\cdot c<b\cdot c$.
3. **Completeness Property.** For all nonempty subsets $S$ of $\mathbb{R}$, if $S$ is bounded above by $\leq$, then the supremum of $S$ under $\leq$ exists. That is, there is $s\in \mathbb{R}$ such that $s=\sup(S)$.

The duals of $<$ and $\leq$ are denoted by $>$ and $\geq$ respectively. Thus, for all $a,b\in \mathbb{R}$, $$b>a\iff a<b$$and $$b\geq a\iff a\leq b.$$
The notation $a<x<b$ means $a<x\wedge x<b$. Similar notations also have similar meaning (for example, $a<x\leq b$ means $a<x\wedge x\leq b$).
***
Definitions used:
- [[Set]]
- [[Function]]
- [[Subtraction Notation on Rings]]
- [[Field]]
- [[Division Notation on Fields]]
- [[Total Order]]
- [[Dual Order]]
- [[Supremum]]
- [[Strict Total Order]]

Theorems used:
- [[Induced Orders From Strict Orders]]