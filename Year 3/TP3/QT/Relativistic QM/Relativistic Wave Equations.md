There are 2 important relativistic wave equations:
- Klein-Gordan equation - spin 0
- Dirac equation - spin $\frac{1}{2}$

Understanding these tells us about spin. It includes particles and anti-particles. The normal way to derive these is using [[4-Vectors]].

Recall [4-position](Index%20and%20Tensor%20Notation.md):
$$x^{\mu}=\begin{bmatrix}
ct \\
x \\
y \\
z
\end{bmatrix};\;x_{\mu}=\begin{bmatrix}
ct & -x & -y & -z
\end{bmatrix}.$$
The metric is given by
$$g^{\mu \nu}=g_{\mu \nu}=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & -1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{bmatrix}.$$
The metric raises and lowers indices.

The [[Lorentz Transforms]] between 2 inertial frames is given by
$$x'^{\mu}=\Lambda^{\mu}_{\;\nu}x^{\nu}.$$
Any quantity that transforms this way is a 4-vector.
[[4-Momentum]]:
$$p^{\mu}=\begin{bmatrix}
\frac{E}{c} \\
p_{x} \\
p_{y} \\
p_{z}
\end{bmatrix}.$$
The scalar product is defined as $a^{\mu}b_{\mu}=g_{\mu \nu}a^{\mu}b^{\nu}$ and is conserved between frames.
$$a^{\mu}b_{\mu}=a'^{\mu}b'_{\mu}=g_{\mu \nu}a'^{\mu}b'^{\nu}=g_{\mu \nu}\Lambda^{\mu}_{\;\alpha}a^{\alpha}\Lambda^{\nu}_{\;\beta}a^{\alpha}b^{\beta}=g_{\mu \nu}\Lambda^{\mu}_{\;\alpha}\Lambda^{\nu}_{\;\beta}a^{\alpha}b^{\beta}$$
$$\implies g_{\mu \nu}\Lambda^{\mu}_{\;\alpha}\Lambda^{\nu}_{\;\beta}=g_{\alpha\beta}.$$
There are 2 main types of Lorentz transforms:
1. [[Rotations]], e.g. angle of $\phi$ about $z$ axis
	$$R=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & \cos \phi & \sin \phi & 0 \\
0 & -\sin \phi & \cos \phi & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
1. Boosts, e.g. along $x$ axis
	$$L_{0}=\begin{bmatrix}
\cosh \eta & -\sinh \eta & 0 & 0 \\
-\sinh \eta  & \cosh \eta  & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
There are also discrete transforms:
1. Spatial inversion - [parity](Symmetries%20and%20Parity.md) 
	$$\underline{x}\to-\underline{x}$$
2. Time reversal
	$$t\to-t.$$
Both are valid Lorentz transforms.

Properties of Lorentz transforms:
$$\det(\Lambda)=\pm 1;\;|\Lambda^{0}_{\;0}|\geq{1}$$
This gives the types of transformations:
$$\det\Lambda=+1;\;\Lambda^{0}_{\;0}\geq{1}\text{ Proper orthochronous}$$
$$\det\Lambda=+1;\;\Lambda^{0}_{\;0}\leq -1\text{ Proper nonorthochronous}$$
$$\det\Lambda=-1;\;\Lambda^{0}_{\;0}\geq 1 \text{ Improper orthochronous}$$
$$\det\Lambda=-1;\;\Lambda^{0}_{\;0}\leq -1\text{ Improper nonorthochronous}.$$
Proper and improper are linked by parity
Orthochronous and nonorthochronous are linked by a time reversal.

We will only consider proper orthochronous transformations - only rotations and boosts.

Recall 4-gradient:
$$\partial_{\mu}=\frac{\partial}{\partial x^{\mu}}=\begin{bmatrix}
\frac{1}{c} \frac{\partial}{\partial t} & \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
\end{bmatrix}$$
$$\partial^{\mu}=\frac{\partial}{\partial x_{\mu}}=\begin{bmatrix}
\frac{1}{c} \frac{\partial}{\partial t} \\
-\frac{\partial}{\partial x} \\
-\frac{\partial}{\partial y} \\
-\frac{\partial}{\partial z}
\end{bmatrix}.$$
This gives a differential operator which transforms a 4-vector and is Lorentz invariant.
$$\square=\partial^{\mu}\partial_{\mu}.$$
