A **graph** $G$ is an ordered triple $(V, E, \psi)$ consisting of a set $V$ of **vertices**, a set $E$ of **edges**, and an **incidence function** $\psi : E \rightarrow (V \times V)/{\sim}$ where $(a,b) \sim (c,d)$ if and only if $(a,b)=(d,c)$ or $(a,b)=(c,d)$ and that $V \cap E = \emptyset$.

If $e$ is an edge and $\psi(e) = uv$, then $e$ is said to **join** $u$ and $v$, and the vertices are called the **ends** of $e$.

The **order** of a graph $G$ is the number of vertices $\nu(G)$.

The **size** of a graph $G$ is the number of edges $\epsilon(G)$.

The ends of an edge are said to be **incident** with the edge, and vice versa.

Two vertices which are incident with a common edge are **adjacent**.

Two edges which are incident with a common vertex are **adjacent**.

Two distinct adjacent vertices are **neighbors**.

The set of neighbors of $v$ in $G$ is denoted by $N_G(v)$.

A **loop** is an edge with identical ends.

A **link** is an edge with distinct ends.

**Parallel edges** are two or more links with the same pair of ends.

A graph is **finite** if both $V$ and $E$ are finite.

The graph with no vertices is the **null graph**.

A graph with one vertex is a **trivial graph**.

A **nontrivial** graph is one that is nonnull and not trivial.

A **simple** graph is one that has no loops or parallel edges.

A **complete** graph is a simple graph where any two vertices are adjacent.

An **empty** graph is a graph which no two vertices are adjacent. Equivalently, it has no edges.

A **bipartite** graph is a graph such that its vertex set can be partitioned into $X$ and $Y$ such that every edge has one end in $X$ and the other in $Y$. Such partition $(X, Y)$ is a **bipartition** of the graph, and $X$ and $Y$ are called its **parts**. Denote the graph by $G[X, Y]$.

If $G[X, Y]$ is simple and every vertex in $X$ is joined with every vertex in $Y$, it is called the **complete bipartite graph**.

A **star** is a complete bipartite graph $G[X, Y]$ with $|X| = 1$ or $|Y| = 1$.

A **path** is a simple graph whose vertices can be arranged in a linear sequence such that two vertices are adjacent iff they are consecutive in the sequence.

A **cycle** on 3 or more vertices is a simple graph whose vertices can be arranged in a cyclic sequence such that two vertices are adjacent iff they are consecutive in the sequence. A cycle on one vertex consists of a vertex and a loop. A cycle on two vertices consists of two vertices joined by a pair of parallel edges.

The **length** of a path or a cycle is the number of edges.

A **k-path** is a path with length $k$.

A **k-cycle** is a cycle with length $k$.

A graph is **connected** if for every partition of its vertex into nonempty sets $X$ and $Y$, there is always an edge with the ends in $X$ and $Y$.

A graph is **disconnected** if it's not connected.

The **incidence matrix** of a graph $G$ is the $\epsilon\times \nu$ matrix $\mathbf{M}_{G}=(m_{ve})$, where $m_{ve}=0,1,2$ is the number of times $v$ and $e$ are incident.

The **adjacency matrix** of a graph $G$ is the $\nu\times \nu$ matrix $\mathbf{A}_{G}=(a_{uv})$, where $a_{uv}$ is the number of edges joining $u$ and $v$. Loops are counted as two edges.

The **degree** of $v$ in $G$ is the number $d_{G}(v)$ (or just $d(v)$ if $G$ is known from context) of edges in $G$ incident with $v$. Loops are counted as two edges.

A vertex $v$ is **isolated** if $d(v)=0$.

The numbers $\delta(G)=\min d(V)$ and $\Delta(G)=\max d(V)$ are called the **minimum degree** and the **maximum degree** of $G$ respectively.

A graph is **k-regular** if $d(v)=k$ for all vertices $v$.

A graph is **regular** if it is k-regular for some $k\in \mathbb{N}$.

A **cubic graph** is a 3-regular graph.

Two graphs $G$ and $H$ are **identical**, denoted as $G=H$, if $V(G)=V(H)$, $E(G)=E(H)$, and $\psi_{G}=\psi_{H}$.

Two graphs $G$ and $H$ are **isomorphic**, denoted as $G\cong H$, if there is a pair of bijections $(\theta:V(G)\to V(H),\phi:E(G)\to E(H))$ such that $\psi_{G}(e)=uv$ if and only if $\psi_{H}(\phi(e))=\theta(u)\theta(v)$. Such a pair is called an **isomorphism** between $G$ and $H$.

Two simple graphs $G$ and $H$ are **isomorphic** if there is a bijection $\theta:V(G)\to V(H)$ such that $u$ and $v$ are adjacent in $G$ if and only if $\theta(u)$ and $\theta(v)$ are adjacent in $H$.

A **graph automorphism** on $G$ is a graph isomorphism from $G$ to itself.

The complete graph with $n$ vertices, up to isomorphism, is denoted as $K_{n}$.

The complete bipartite graph with parts of sizes $m$ and $n$, up to isomorphism, is denoted as $K_{m,n}$.

The path on $n$ vertices, up to isomorphism, is denoted as $P_{n}$.

The cycle on $n$ vertices, up to isomorphism, is denoted as $C_{n}$.

The **components** of a graph $G$ is the pairwise disjoint connected graphs $G_{i}$ with $\bigcup G_{i}=G$.

A graph $S$ is a **subgraph** of a graph $G$, denoted as $S\subseteq G$, if $V(S)\subseteq V(G)$, $E(S)\subseteq E(G)$, and $\psi_{S}$ is the restriction of $\psi_{G}$ to $E(S)$.

An **edge-deleted** subgraph of $G$ is a subgraph of $G$ obtained by deleting an edge $e$ from $E$. This subgraph is denoted as $G\setminus e$.

A **vertex-deleted** subgraph of $G$ is a subgraph of $G$ obtained by deleting a vertex $v$ from $V$ and all the edges incident to $v$ in $E$. This subgraph is denoted as $G-v$.

A subgraph $S$ of $G$ in a family $\mathcal{F}$ of subgraphs of $G$ is **maximal** if for all subgraphs $H$ of $G$ such that $S\subseteq H$, $S=H$.

The length of a longest cycle in a graph $G$ is called its **circumference**.

The length of a shortest cycle in a graph $G$ is called its **girth**.

A graph is **acyclic** if it does not contain a cycle.

A **spanning subgraph** of $G$ is a subgraph obtained by edge deletions only, equivalently, it is a subgraph whose vertex set is the same as $G$. If $S$ is the set of deleted edges, the subgraph is denoted as $G\setminus S$.

The **underlying simple graph** of $G$ is obtained by deleting all of the loops and all but one parallel edges of $G$.

An **induced subgraph** of $G$ is as subgraph of $G$ obtained by vertex deletion only. If $X$ is the set of deleted vertices, the subgraph is denoted as $G - X$. Further, if $Y = V \setminus X$,  then $G[Y]$ is the **subgraph of $G$ induced by $Y$**.

If $S$ is a set of edges in $G$, then $G[S]$ is an **edge-induced subgraph** of $G$, that is a subgraph of $G$ whose edge set is $S$ and vertex set consists of all ends of the edges in $S$.

A **weighted graph** is a graph $G$ equipped with a function $w : E \to \mathbb{R}$ which assigns each edge to a **weight**. The value $w(e)$ is called the weight of $e$. If $F$ is a subgraph of $G$, then $w(F)$ is the weight of $F$ defined by $\sum_{e \in E(F)} w(e)$.

If $X$ and $Y$ are sets of vertices, then $E[X, Y]$ is the set of edges in $G$ with one end in $X$ and the other end in $Y$. If $Y = V \setminus X$, then $E[X, Y]$ is called the **edge cut** of $G$ associated with $X$, or the **coboundary** of $X$, denoted by $\partial(X)$.

An edge cut $\partial(v)$ associated with a single vertex $v$ is a **trivial edge cut**, which is simply the set of all links incident with $v$.

A **bond** of a graph is a minimal nonempty edge cut.

A **walk** in a graph $G$ is a sequence $W = v_0 e_1 v_1 \dots v_{l-1}e_lv_l$, whose terms are alternately vertices and edges of $G$ (not neccessarily distinct) such that $v_{i-1}$ and $v_i$ are the ends of $e_i$. If $v_0 = x$ and $v_l = y$, we say that $W$ **connects** $x$ to $y$, and $W$ is an **$xy$-walk**. The vertices $x$ and $y$ are called the **ends** of the walk, $x$ being the **initial vertex** and $y$ **terminal vertex**, the vertices $v_1, v_2, \dots, v_{l-1}$ are its **internal vertices**. The integer $l$ is the **length** of the walk.

An **$x$-walk** is a walk with initial vertex $x$.

If $u$ and $v$ are two vertices of a walk $W$, where $u$ precedes $v$ on $W$, the subsequence of $W$ starting with $u$ and ending with $v$ is denoted by $uWv$ and called the **segment** of $W$ from $u$ to $v$.

In a simple graph a walk is determined by its vertices.

A walk in a graph is **closed** if its initial and terminal vertices are identical, and it is a **trail** if all its edge terms are distinct. 

A **path** can be seen as walks whose vertices and edges are distinct.

A closed trail of positive length whose initial and internal vertices are distinct is the sequence of vertices and edges of a cycle.

The length of the shortest $xy$-path is the **distance** between $x$ and $y$ denoted by $d_G(x, y)$. If there is no path between $x$ and $y$ we set $d_G(x, y) = \infty$.

If $X$ and $Y$ are sets of vertices, then an $(X, Y)$-**path** is a path which starts at a vertex of $X$, ends at a vertex of $Y$, and whose internal vertices belong to neither $X$ nor $Y$.

A **cut edge** of $G$ is an edge $e$ such that $c(G \setminus e) = c(G) + 1$. Cut edges are also bonds of size one. Another characterization, $e$ is a cut edge iff $e$ belongs to no cycle.

A **tree** is an acyclic connected graph.

A **forest** is an acyclic graph.

A **leaf** of a tree is a vertex with degree one.

A **subtree** is a subgraph which is a tree.

A **spanning tree** is a spanning subgraph which is a tree.

The complement $E \setminus T$ of a spanning tree $T$ is called a **cotree** denoted by $\bar{T}$.



