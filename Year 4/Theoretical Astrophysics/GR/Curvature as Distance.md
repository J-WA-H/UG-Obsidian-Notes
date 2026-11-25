We aim to use tensor algebra to describe curvature - hence defining gravity. One way to consider curvature is distance, shown below as the two lines start and end at the two points, but the curved line has a much larger distance.
![[Pasted image 20260115115936.png]]
In cartesian and spherical coordinates, distance is defined by Pythagoras' theorem,
$$ds^2=dx^2+dy^2+dz^2=dr^2+r^2d\theta^2+r^2\sin^2\theta d\phi^2\tag{1.1}. $$
This distance between points defines the metric, which in spacetime is
$$ds^2=c^2dt^2-dx^2-dy^2-dz^2=cdt^2-dr^2-r^2d\theta^2-r^2\sin^2\theta d\phi^2\tag{1.2}. $$
This defines the spacetime interval. Distance is fundamental to the shape of the space. It is defined on a coordinate system that is not fundamental.

To define notation, consider the position $\vec{r}=x\vec{i}+y\vec{j}+z\vec{k}$. Instead use indices
$$\vec{r}=\begin{bmatrix}
x^1 \\
x^2 \\
x^3
\end{bmatrix}\tag{1.3} $$
and the basis $\vec{e}_{1},\vec{e}_{2},\vec{e}_{3}$. This gives
$$\vec{r}=x^1\vec{e}_{1}+x^2\vec{e}_{2}+x^3\vec{e}_{3}=\sum_{i=1}^3x^i\vec{e}_{i}=x^i\vec{e}_{i}\tag{1.4} $$which makes use of Einstein's summation convention. We also use the convention that $i,j,k$ represents 3D space, $a,b,c,\dots$ gives a general $N$-dimensional space, $A,B,C$ denotes 2D space, and $\alpha,\beta,\gamma$ denotes 4D spacetime.

To denote a change of frame, use $\bar{x}$ instead of $x'$,
$$\bar{x}=x^\bar{1}=\gamma\left( x^1-\frac{v}{c}x^0 \right)=\gamma(x^1-\beta x^0).\tag{1.5} $$
![[Pasted image 20260115123700.png]]
The coordinates of $P$ is $\vec{r}(P)=x^a(P)\vec{e}_{a}$ and for $Q$ $\vec{r}(Q)=x^a(Q)\vec{e}_{a}$. The distance between these points is $$\Delta \vec{r}=[x^a(Q)-x^a(Q)]\vec{e}_{a}=\Delta x^a\vec{e}_{a}\tag{1.6}. $$From the position vector $\vec{r}=x^1\vec{e}_{1}+x^2\vec{e}_{2}+x^3\vec{e}_{3}$, the basis vector becomes
$$\vec{e}_{i}=\frac{\partial \vec{r}}{\partial x^i}\tag{1.7}. $$
Consider new coordinates $x^\bar{b}$ from $x^a$,
$$x^\bar{a}=x^\bar{a}(x^b)\tag{1.8} .$$The new coordinates are defined on the old coordinate system. This expands to $N^2$ equations,
$$\begin{matrix}
\Delta x^\bar{1}=\Delta x^{\bar{1}}(x^1,x^2,\dots,x^N) \\
\Delta x^\bar{2}=\Delta x^\bar{2}(x^1,x^2,\dots ,x^N) \\
\vdots \\
\Delta x^\bar{N}=\Delta x^\bar{N}(x^1,x^2,\dots,x^N)
\end{matrix}.\tag{1.9} $$
Consider the function $f(x^1,x^2,\dots,x^N)$, its full derivative is defined as
$$\Delta f=\frac{{\partial f}}{\partial x^1}\Delta x^1+\dots \frac{\partial f}{\partial x^N}\Delta x^N\tag{1.10} $$which yields
$$dx^\bar{b}=\frac{\partial x^\bar{b}}{\partial x^a}dx^a.\tag{1.11} $$
$$\vec{e}_{\bar{b}}=\frac{\partial x^c}{\partial x^\bar{b}}\vec{e}_{c}\tag{1.12}. $$the form of the equation is unchanged $\Delta x^\bar{b}\vec{e}_{\bar{b}}=\Delta x^a\vec{e}_{a}$.
