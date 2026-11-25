 The [Dirac equation](Dirac%20Equation%20Derivation.md) is [Lorentz invariant](Dirac%20Equation%20Lorentz%20Invariance.md) and has a positive [probability density](Dirac%20Continuity%20Equation.md), but the negative energy solutions, like the [[Klein-Gordon Equation]], still remain but the Dirac equation allows us to reinterpret our understanding spin.

Consider the plane wave solution of the Dirac equation,
$$\psi(\underline{x},t)=Au(p)\exp\left[ \frac{i}{\hbar}(\underline{p}\cdot \underline{x}-Et) \right]=Au(p)\exp\left[ -\frac{i}{\hbar}p^{\mu}x_{\mu} \right].$$
$u(p)$ is a 4-component spinor which is dependent on momentum $p^{\mu}$ instead of $x^{\mu}$ and $A\in \mathbb{C}$.

Use the Dirac equation to find $u(p)$,
$$i\hbar \frac{\partial \psi}{\partial t}=(-ic\hbar\alpha^{k}\nabla_{k}+\beta mc^2)\psi(\underline{x},t).$$
$$Eu(p)\cancel{A}\cancel{e^{ -ip^{\mu} x_{\mu}/\hbar} }=(c\alpha^{k}p_{k}+\beta mc^2)\cancel{A}u(p)\cancel{e^{-ip^{\mu}x_{\mu}/\hbar}}.$$
Start in the particles rest frame, $p^{\mu}=\begin{bmatrix}mc \\ \underline{0}\end{bmatrix}$,
$$E\begin{bmatrix}
u_{1} \\
u_{2} \\
u_{3} \\
u_{4}
\end{bmatrix}=mc^2\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{bmatrix}\begin{bmatrix}
u_{1} \\
u_{2} \\
u_{3} \\
u_{4}
\end{bmatrix}.$$
There are two types of solutions,
$$E=mc^2;\;\begin{cases}
u_{1},u_{2}\neq 0 \\
u_{3},u_{4}=0
\end{cases}$$
$$E=-mc^2;\;\begin{cases}
u_{1},u_{2}=0 \\
u_{3},u_{4}\neq 0
\end{cases}.$$
This gives a basis of 4 spinor,- 
$$\{ u_{1}=\begin{bmatrix}
1 \\
0 \\
0 \\
0
\end{bmatrix},u_{2}=\begin{bmatrix}
0 \\
1 \\
0 \\
0
\end{bmatrix},u_{3}=\begin{bmatrix}
0 \\
0 \\
1 \\
0
\end{bmatrix}, u_{4}=\begin{bmatrix}
0 \\
0 \\
0 \\
1
\end{bmatrix} \}.$$
The first two states represent the positive energy, particle, and the last two represent negative energy, antiparticle.

For the general solution, the momentum is non-zero.
$$\psi(\underline{x},t)=Au(p)e^{-ip^{\mu}x_{\mu}/\hbar}.$$
One way is to boost the solutions from the rest frame but it is easier to calculate directly.
$$Eu(p)=(c\alpha^{k}p_{k}+\beta mc^2)u(p).$$
Brake $u$ down into two two-component spinors.
$$E\begin{bmatrix}
u_{A} \\
u_{B}
\end{bmatrix}=\begin{bmatrix}
mc^2\mathbb{I}_{2} & c\underline{\sigma}\cdot \underline{p} \\
c\underline{\sigma}\cdot \underline{p} & -mc^2\mathbb{I}_{2}
\end{bmatrix}\begin{bmatrix}
u_{A} \\
u_{B}
\end{bmatrix}.$$
Expanding this out gives
$$Eu_{A}=mc^2u_{A}+c\underline{\sigma}\cdot \underline{p}u_{B}$$
$$\implies u_{A}=\frac{c\underline{\sigma}\cdot\underline{p}}{E-mc^2}u_{B}.$$
$$Eu_{B}=c\underline{\sigma}\cdot \underline{p}u_{A}-mc^2u_{B}$$$$\implies u_{B}=\frac{{c\underline{\sigma} \cdot \underline{p}}}{E+mc^2}u_{A}$$
$$\therefore u_{A}=\frac{{c\underline{\sigma}\cdot \underline{p}}}{E-mc^2} \frac{{c\underline{\sigma}\cdot \underline{p}}}{E+mc^2}u_{A}=\frac{c^2(\underline{\sigma}\cdot \underline{p})^2}{(E-mc^2)(E+mc^2)}u_{A}.$$
Aside:
$$(\underline{\sigma}\cdot \underline{a})(\underline{\sigma}\cdot \underline{b})=\sigma_{i}\sigma_{j}a_{i}b_{j}=\frac{1}{2}(\sigma_{i}\sigma_{j}+\sigma_{j}\sigma_{i})a_{i}b_{j}+\frac{1}{2}(\sigma_{i}\sigma_{j}-\sigma_{j}\sigma_{i})a_{i}b_{j}$$
$$=\frac{1}{2}\{ \sigma_{i},\sigma_{j} \}a_{i}b_{j}+\frac{1}{2}[\sigma_{i},\sigma_{j}]=\delta_{ij}a_{i}b_{j}+i\epsilon_{ijk}a_{i}b_{j}\sigma_{k}=\underline{a}\cdot \underline{b}+i(\underline{a}\times \underline{b})\cdot\sigma_{k}.$$
$$(\underline{\sigma}\cdot \underline{a})(\underline{\sigma}\cdot \underline{b})=\underline{a}\cdot \underline{b}+i(\underline{a}\times \underline{b})\cdot\sigma_{k}.$$
Applying this to the solutions,
$$(\underline{\sigma}\cdot \underline{p})^2=\underline{p}\cdot \underline{p}+i(\underline{p}\times \underline{p})\cdot\sigma_{k}=\underline{p}\cdot \underline{p}=|\underline{p}|^2.$$
$$u_{A}=\frac{c^2p^2}{E^2-m^2c^4}u_{A}\implies(E^2-m^2c^4=p^2c^2)u_{A}=0.$$
This gives 4 eigenvalues,
$$E_{+}=(m^2c^4+p^2c^2)^{1/2}$$
$$E_{-}=-(m^2c^4+p^2c^2)^{1/2}.$$
In terms of spinors,
$$u_1=\begin{bmatrix}
\alpha \\
\frac{{c\underline{\sigma}\cdot \underline{p}}}{E+mc^2}\alpha
\end{bmatrix};\;u_{2}=\begin{bmatrix}
\beta \\
\frac{{c\underline{\sigma}\cdot \underline{p}}}{E+mc^2}\beta
\end{bmatrix}$$
$$u_{3}=\begin{bmatrix}
\frac{{c\underline{\sigma}\cdot \underline{p}}}{E-mc^2}\alpha \\
\alpha
\end{bmatrix};\;u_{4}=\begin{bmatrix}
\frac{{c\underline{\sigma}\cdot \underline{p}}}{E-mc^2}\beta \\
\beta
\end{bmatrix}.$$
