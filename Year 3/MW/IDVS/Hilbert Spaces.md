A Hilbert space is a metric space - a complex [vector space](Vector%20Spaces.md) with an inner product whose elements look like $\sum_{n}a_{n}\ket{\phi_{n}}$, where $a_{n}\in \mathbb{C}$. This allows for superposition of states to be described.

We have a concept of distance between vectors $f,g$ between two elements which we do using the norm
$$d(f,g)=\lVert f-g \rVert =\sqrt{ (f-g,f-g) }.$$
The distance must satisfy these properties
1. $d(f,g)=d(g,f)$
2. $d(f,g)>0$. Only vanishes for $f=g$.
3. $d(f,g)\leq d(f,h)+d(h,g)$ (triangle inequality).

The normed space is complete if every convergent sequence in the space $X$ has a limit that is also in the space $X$.

The Cauchy sequence is a sequence whose elements become arbitrarily close for $f_{n}\to f$ as $n\to \infty$ i.e. if $\{ f_{n} \}\subset X\iff f\in X$.

The [pre-Hilbert space](Infinite%20Dimensional%20Spaces.md) is not necessarily complete but every pre-Hilbert space has a closure - we can add to $X$ the limit of all possible sequences in $X$.
e.g. we can add all irrationals to $\mathbb{Z}$ to get $\mathbb{R}$.

We denote the closure of $X$ as $\bar{X}$. The complete pre-Hilbert space is a Hilbert space.

Because Hilbert spaces can be infinite dimensional, we are forced to work with an infinite basis. If we have a sequence $\{ \underline{f}_{1},\underline{f}_{2},\dots,\underline{f}_{n} \}$ with $\underline{f}_{k}=\sum_{i=1}^{\infty}\underline{e}_{i}p^{i}\in H$.
The sequence converges strongly to $f$ if $\lVert \underline{f}-\underline{f}_{n} \rVert\to 0$ as $n\to \infty$.
The sequence converges weakly to $f$ if the scalar product $(\underline{g},\underline{f}_{n})\to(\underline{g},\underline{f})$ for any $\underline{g}\in H$.

Strong convergence $\implies$ weak convergence, but not the other way around.

As the Hilbert space is complete, all Cauchy-sequences converge in $H$.
The Cauchy-sequence implies $\lVert f_{n}-f_{m} \rVert\to 0;\;n,m\to 0$.
