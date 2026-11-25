A contravariant first order tensor $(1,0)$ is a quantity $A^a$ that are components of $\vec{A}=A^a\vec{e}_{a}=A^\bar{b}\vec{e}_{\bar{b}}$ and transforms as$$A^\bar{b}=\frac{\partial x^\bar{b}}{\partial x^a}A^a\tag{2.1}. $$Suppose we have $A^a,B^a$ that are both $(1,0)$ tensors. Consider $T^a=k(A^a+B^a)$. Take this to another [frame](Curvature%20as%20Distance.md) $x^\bar{b}=x^\bar{b}(x^a)$,
$$T^\bar{b}=k(A^\bar{b}+B^\bar{b})=k\left( \frac{\partial x^\bar{b}}{\partial x^a}A^a+\frac{\partial x^\bar{b}}{\partial x^a}B^a \right)=k \frac{\partial x^\bar{b}}{\partial x^a}(A^a+B^a)=\frac{\partial x^\bar{b}}{\partial x^a}T^a\tag{2.2} $$
This gives that $T^a$ is a $(1,0)$ tensor so contravariant tensors are linear.

Consider higher-order tensors, for example $T^{ab}=A^aB^a$, which is a $(2,0)$. This transforms as
$$T^{\bar{c}\bar{d}}=A^\bar{c}B^\bar{d}=\frac{\partial x^\bar{c}}{\partial x^a}A^a \frac{\partial x^\bar{d}}{\partial x^b}B^b=\frac{\partial x^\bar{c}}{\partial x^a} \frac{\partial x^\bar{d}}{\partial x^b}A^aB^b=\frac{\partial x^\bar{c}}{\partial x^a} \frac{\partial x^\bar{d}}{\partial x^b}T^{ab}.\tag{2.3} $$
An outer product is when multiple tensors multiply together to get higher order tensors.
Example: $A^i=(1,2,3)$ $B^j=(2,3,4)$,
$$A^iB^j=\begin{bmatrix}
A_{1}B_{1} & A_{1}B_{2} & A_{1}B_{3} \\
A_{2}B_{1} & A_{2}B_{2} & A_{2}B_{3} \\
A_{3}B_{1} & A_{3}B_{2} & A_{3}B_{3}
\end{bmatrix}=\begin{bmatrix}
2 & 3 & 4 \\
4 & 6 & 8 \\
6 & 9 & 12
\end{bmatrix}.\tag{2.4} $$
Note that in general $A^iB^j\neq A^jB^i$. 

Define a scalar field $\phi(x^i)$. For a coordinate transform $\phi$ is invariant, but $\vec{\nabla}\phi$ isn't. This vector has components $\frac{\partial \phi}{\partial x^i}$. Change coordinates to $x^\bar{j}=x^\bar{j}(x^i)$. Let $A_{i}=\frac{\partial \phi}{\partial x^i}$, this transforms as
$$A_{\bar{j}}=\frac{\partial \phi}{\partial x^\bar{j}}=\frac{\partial \phi}{\partial x^i} \frac{\partial x^i}{\partial x^\bar{j}}=\frac{\partial x^i}{\partial x^\bar{j}}A_{i}\tag{2.5} .$$
This is a covariant tensor $(0,1)$. These are also linear.

Using the generalised position vector $d\vec{r}=dx^a\vec{e}_{a}$
![[Pasted image 20260117103119.png]]
the distance between $P$ and $Q$ is
$$ds^2=d\vec{r}\cdot d\vec{r}=(dx^a\vec{e}_{a})\cdot(dx^b\vec{e}_{b})=\vec{e}_{a}\cdot \vec{e}_{b}dx^adx^b=g_{ab}dx^adx^b.\tag{2.6} $$This defines the metric tensor $g_{ab}=\vec{e}_{a}\cdot \vec{e}_{b}$. Using the definition of the basis vectors,
$$\vec{e}_{\bar{b}}=\frac{\partial \vec{r}}{\partial x^\bar{b}}=\frac{\partial \vec{r}}{\partial x^a} \frac{\partial x^a}{\partial x^\bar{b}}=\frac{\partial x^a}{\partial x^\bar{b}}\vec{e}_{a}\tag{2.7} $$
$$\therefore g_{\bar{a}\bar{b}}=\vec{e}_{\bar{a}}\cdot\vec{e}_{\bar{b}}=\frac{\partial x^a}{\partial x^\bar{a}}\vec{e}_{a}\cdot \frac{\partial x^b}{\partial x^\bar{b}}\vec{e}_{b}=\frac{\partial x^a}{\partial x^\bar{a}} \frac{\partial x^b}{\partial x^\bar{b}}g_{ab}.\tag{2.8} $$
The metric tensor is symmetric.
For 3D flat cartesian space, $\vec{e}_{1}=\vec{i}$, $\vec{e}_{2}=\vec{j}$, $\vec{e}_{3}=\vec{k}$, which gives
$$g_{ab}=\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}\tag{2.9} $$
and
$$ds^2=dx^2+dy^2+dz^2\tag{2.10} .$$
This gives Pythagoras.

For spherical coordinates, $\vec{e}_{1}=\sin \theta \cos \phi \vec{i}+\sin \theta \sin \phi \vec{j}+\cos \theta \vec{k}$, $\vec{e}_{2}=r\cos \theta \cos \phi\vec{i}+r\cos \theta \sin \phi \vec{j}-r\sin \theta \vec{k}$, $\vec{e}_{3}=-r\sin \theta \sin \phi \vec{i}+r\sin \theta \cos \phi \vec{j}$ the metric is
$$g_{ab}=\begin{bmatrix}
1 & 0 & 0 \\
0 & r^2 & 0 \\
0 & 0 & r^2\sin^2\theta
\end{bmatrix}\tag{2.11} $$
with the distance
$$ds^2=dr^2+r^2d\theta^2+r^2\sin^2\theta d\theta^2+r^2\sin^2\theta d\phi^2.\tag{2.12} $$
