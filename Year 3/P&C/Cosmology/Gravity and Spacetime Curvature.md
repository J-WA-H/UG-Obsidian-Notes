Test bodies move along the shortest trajectory. Gravity is of a geometric nature. This is the universality of spacetime.

Matter tells space how to curve, and space tells matter how to move.

In normal flat spacetime, the separation between two events is given by the [Minkowski norm](Lorentz%20Transforms.md),
$$ds^2=-c^2dt^2+dx^2+dy^2+dz^2.$$
This norm is given by the [metric](Index%20and%20Tensor%20Notation.md)
$$g_{\mu \nu}=\begin{bmatrix}
-1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}.$$
$$ds^2=g_{\mu \nu} dx^{\mu}dx^{\nu}=\begin{bmatrix}
cdt & dx & dy & dz
\end{bmatrix}\begin{bmatrix}
-1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}\begin{bmatrix}
cdt \\
dx \\
dy \\
dz
\end{bmatrix}.$$
$g_{\mu \nu}$ is the metric of a static universe. For an expanding universe, the metric is deformed to
$$g_{\mu \nu}(x^{\alpha})=\begin{bmatrix}
-1 & 0 & 0 & 0 \\
0 & a^2 & 0 & 0 \\
0 & 0 & a^2 & 0 \\
0 & 0 & 0 & a^2
\end{bmatrix}.$$
Here the separation is
$$ds^2=-c^2dt^2+a^2(dx^2+dy^2+dz^2).$$
This gives the Ricci curvature tensor
$$R_{\mu \nu}=\frac{\partial}{\partial x^{\alpha}} \frac{\partial}{\partial x^{\beta}}g_{\mu \nu}(x).$$
Einstein's equation is
$$R_{\mu \nu}-\frac{1}{2}g_{\mu \nu}R=\frac{8\pi G}{c^4}T_{\mu \nu}+\Lambda g_{\mu \nu}$$
where $T_{\mu \nu}=\text{diag}(\rho c^2,P,P,P)$.
This equations give:
$$\left( \frac{\dot{a}}{a} \right)^2+\frac{kc^2}{a^2}=\frac{8\pi G\rho(t)}{3}+\frac{\Lambda}{3}$$
$$2\left( \frac{\ddot{a}}{a} \right)+\left( \frac{\dot{a}}{a} \right)+\frac{kc^2}{a^2}=-\frac{8\pi GP(t)}{c^2}+\Lambda.$$
