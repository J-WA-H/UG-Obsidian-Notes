The contravariant vector is defined by
$$x^\mu=\begin{bmatrix}
x^0 \\
x^1 \\
x^2 \\
x^3
\end{bmatrix}=\begin{bmatrix}
ct \\
x \\
y \\
z
\end{bmatrix} \rightarrow\text{Contravariant vector}$$
In index notation, the [Lorentz transformation matrix](4-Vectors.md) is given by 
$$\Lambda^\mu_{\;\nu}=\frac{\partial x'^\mu}{\partial x^\nu}$$
A contravariant vector is a vector that can transform under a Lorentz transform
$$x'^\mu=\Lambda^\mu_{\;\nu}x^\nu$$
A covariant vector flips the sign of the spatial dimensions and is denoted by $x_{\nu}$
$$x_{\nu}=\begin{bmatrix}
x_{0} \\
x_{1} \\
x_{2} \\
x_{3}
\end{bmatrix}=\begin{bmatrix}
x^0 \\
-x^1 \\
-x^2 \\
-x^3
\end{bmatrix}=\begin{bmatrix}
ct \\
-x \\
-y \\
-z
\end{bmatrix}.$$
A metric can transform a contravariant vector into a covariant vector
$$g^{\mu \nu}=g_{\mu \nu}=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & -1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{bmatrix}.$$
$$q_{\mu}=g_{\mu \nu}q^\nu$$
Product of two metrics:
$$g^\mu_{\;\nu}=g^{\mu \rho}g_{\rho \nu}=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}=\delta^\mu_{\;\nu}.$$
 A covariant 4-vector transforms as:
 $$x'_{\mu}=g_{\mu \nu}x'^\nu=g_{\mu \nu}\Lambda^\nu_{\;\rho}x^\rho=g_{\mu \nu}\Lambda^\nu_{{\;\rho}}g^{\rho \sigma}x_{\sigma}=\Lambda_{\mu}^{\;\sigma}x_{\sigma}.$$
