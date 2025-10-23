**Theorem.**
1. Suppose $a,b\in \mathbb{R}$. Then, $d(a,b)\geq 0$.
2. Suppose $a,b\in \mathbb{R}$. Then, $d(a,b)=d(b,a)$.
3. Suppose $a,b,c\in \mathbb{R}$. Then, $d(a,c)\leq d(a,b)+d(b,c)$.
4. Suppose $a,b\in \mathbb{R}$. Then, $d(a,b)=0$ if and only if $a=b$.

**Proof of First Statement.** By [[Absolute Value as Norm on Real Numbers]], $|a-b|\geq 0$, so $d(a,b)\geq 0$. $\blacksquare$

**Proof of Second Statement.** By [[Inverses of Group Compositions]] and [[Involution Property on Group Inverses]], $$-(a-b)=b-a.$$By [[Absolute Value as Even Function]], $|a-b|=|{-(a-b)}|$, so $|a-b|=|b-a|$. Therefore, $d(a,b)=d(b,a)$. $\blacksquare$

**Proof of Third Statement.** We have $$a-c=a-b+b-c=(a-b)+(b-c),$$so by [[Absolute Value as Norm on Real Numbers]] $$|a-c|=|(a-b)+(b-c)|\leq|a-b|+|b-c|.$$Therefore, $d(a,c)\leq d(a,b)+d(b,c)$.

**Proof of Fourth Statement.** By [[Absolute Value as Norm on Real Numbers]], $|a-b|=0$ if and only if $a-b=0$. Since $d(a,b)=|a-b|$ and $a-b=0$ if and only if $a=b$, we have $d(a,b)=0$ if and only if $a=b$. $\blacksquare$
***
Definitions used:
- [[Real Numbers]]
- [[Absolute Value]]
- [[Distance Function on Real Numbers]]

Theorems used:
- [[Absolute Value as Norm on Real Numbers]]
- [[Absolute Value as Even Function]]
- [[Inverses of Group Compositions]]
- [[Involution Property on Group Inverses]]