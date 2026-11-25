Consider two elements of abelian group $U_{i},U_{j}\in G$. The order we apply these groups does not matter, $U_{i}U_{j}=U_{j}U_{i}$. An example of these are spatial translations.
![[Pasted image 20260205142125.png]]
For non-abelian groups, the order in general does matter, $U_{i}U_{j}\neq U_{j}U_{i}$, for example rotations
![[Pasted image 20260205142933.png]]
Groups can be shown by their representations. Consider the group of rotations on the vector $\vec{x}\to U\vec{x}$ where $$U=U_{z}(\theta_{z})U_{x}(\theta_{x})U_{y}(\theta_{y})\tag{1.1} .$$For example, about the $z$-axis
$$U_{z}(\theta_{z})=\begin{bmatrix}
\cos \theta_{z} & -\sin \theta_{z} & 0 \\
\sin \theta_{z} & \cos \theta_{z} & 0 \\
0 & 0 & 1
\end{bmatrix}.\tag{1.2} $$
The rotation group is defined by the properties:
- $UU^T=U^TU=1$
- $\det(U)=1$.

$\vec{x}=\begin{bmatrix}x & y & z \end{bmatrix}^T$ is the vector representation $\mathbf{3}$. Defining $\vec{p}=(p_{x},p_{y},p_{z})^T$, we get $M_{ij}=x_{i}p_{j}$ such that $M\to UMU^T$. We can decompose $M$ to the sum of the identity, and symmetric and antisymmetric parts
$$M=I+S+A=\frac{\mathrm{Tr}(M)}{3}\mathbb{I}+\frac{{M+M^T}}{2}-I + \frac{{M-M^T}}{2}\tag{1.3}. $$
The identity is defined such that
$$I\to UIU^T\propto I\tag{1.4}.$$
Define the representation
$$\omega=\begin{bmatrix}
\underbrace{ \vec{x}\cdot \vec{p} }_{ \mathbf{1} } & \underbrace{ x_{i}p_{j}-x_{j}p_{i}, \frac{yp_{y}+xp_{x}-2zp_{z}}{\sqrt{ 3 }},x_{i}p_{j}+x_{j}p_{i} }_{ \mathbf{5} }
\end{bmatrix} \tag{1.5} $$
Then
$$\omega\to \begin{bmatrix}
1 & 0 & 0 \\
0 & U^A_{3\times 3} & 0 \\
0 & 0 & U^S_{5\times 5}
\end{bmatrix}.\tag{1.6} $$This then gives
$$\begin{matrix}
\mathbf{3}\otimes \mathbf{3}=\mathbf{1}\oplus \mathbf{3}\oplus \mathbf{5} \\
1\otimes 1=0\oplus 1\oplus 2
\end{matrix}\tag{1.7} .$$This is similar to combining 2 spin-1 states. Consider the representation $R\to UR$ with $U=\exp[i\theta_{B}T_{B}]$ where $\theta_{B}$ is a parameter and $T_{B}$ is the generator. $B$ runs over the dimensions of the group. This is a Lie group

Assume the generators are Hermitian, $T_{B}^{\dagger}=T_{B}$. For $SO(3)$, 
$$\exp[i\theta_{B}T_{B}]=1+\begin{bmatrix}
0 & -\theta_{z} & \theta_{y} \\
\theta_{z} & 0 & -\theta_{x} \\
-\theta_{y} & \theta_{x} & 0
\end{bmatrix}+\mathcal{O}(\theta^2)\tag{1.8}.$$
This gives the generators
$$T_{1}=\begin{bmatrix}
0 & 0 & 0 \\
0 & 0 & i \\
0 & -i & 0
\end{bmatrix};\;T_{2}=\begin{bmatrix}
0 & 0 & -i \\
0 & 0 & 0 \\
i & 0 & 0
\end{bmatrix};\;T_{3}=\begin{bmatrix}
0 & i & 0 \\
-i & 0 & 0 \\
0 & 0 & 0
\end{bmatrix}.\tag{1.9} $$
Different representations of the same group have different generators.
$$e^{ i\theta_{B}T_{B} }e^{ i\theta_{C}T_{C} }-e^{ i\theta_{C}T_{C} }e^{ i\theta_{B}T_{B} }=-\theta_{B}\theta_{C}[T_{B},T_{C}]+\mathcal{O}(\theta^3).\tag{1.10} $$
The commutator is
$$[T_{B},T_{C}]=i\sum_{D}f_{BCD}T_{D}\tag{1.11} .$$$f_{BCD}$ are structure constants, which equal zero for abelian groups and non-zero for non-abelian groups.
$A=A_{B}T_{B}$ with $$A\to UAU^{-1}=UAU^{-1}UU^{\dagger}=UAU^{\dagger}=A+i\theta_{C}[T_{C},T_{B}]+\mathcal{O}(\theta^2)=(A_{D}+\theta_{C}f_{CBD}A_{B})T_{D}+\mathcal{O}(\theta^2).\tag{1.12} $$
Structure constants themselves act as generators. This is the adjoint representation of the group. 

Important groups are
- $SO(d)$
- $SU(d)$, $U^{\dagger}U=1=e^{ -i\theta T }e^{ i\theta T }=1+i\theta(T-T^{\dagger})\implies T=T^{\dagger}$.
	- $\det(e^{ i\theta T })=1=e^{ i\theta \mathrm{Tr}(T) }\implies \mathrm{Tr}(T)=0$.

The generators that define $SU(d)$ must satisfy $T=T^{\dagger}$ and $\mathrm{Tr}(T)$.

Groups act on fields in a representation.
- Trivial representation ($\mathrm{dim}=1$) $\iff$ fields are uncharged since they are unchanged.
- Fundamental representation ($SU(n),\mathrm{dim}=N$) $\iff$ matter fields, e.g. quarks $\mathbf{3}$
	- Anti-fundamental representation $\iff$ anti matter fields e.g. anti-quarks $\mathbf{\bar{3}}$.
- Adjoint representation $(T^A)^{BC}=if^{ABC}$ $\iff$ gauge bosons e.g. $SU(3):\mathbf{8}$, $SU(2):\mathbf{3}$.

Note $\mathrm{dim}(SU(N))=N^2-1$.

Group dimension is the number of generators, different from representation dimension which is the dimension of the vector space. They are only equal in the adjoint representation.