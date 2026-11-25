We have followed a historical [[Dirac Equation Derivation]] but this hides its Lorentz symmetry.
Introduce an alternative notation, the covariant form, so we can see the symmetries.
The Dirac equation is
$$i\hbar  \frac{\partial \psi}{\partial t}=-i\hbar c\alpha^{k} \frac{\partial \psi}{\partial x^{k}}+\beta mc^2\psi(\underline{x},t).$$
Multiply the Dirac equation by $-\frac{\beta}{\hbar c}$,
$$-\frac{i\beta}{c} \frac{\partial \psi}{\partial t}=i\beta\alpha^{k} \frac{{\partial \psi}}{\partial x^k}-\frac{mc}{\hbar}\psi$$
$$-i\left( \frac{\beta}{c} \frac{{\partial \psi}}{\partial t}+\beta\alpha^{k} \frac{{\partial \psi}}{\partial x^{k}} \right)+\frac{mc}{\hbar}\psi=0.$$
Using the [4-gradient](Relativistic%20Wave%20Equations.md)
$$\partial_{\mu}=\begin{bmatrix}
\frac{1}{c} \frac{\partial}{\partial t} & \frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}
\end{bmatrix},$$
from observation, the Dirac equation is of a similar form. To use this - we define $\gamma$ matrices:
$$\gamma^{0}=\beta;\;\gamma^{k}=\beta \alpha^{k}.$$
These are also known as Dirac matrices.
Using these the Dirac equation then becomes
$$\left( -i\gamma^{\mu}\partial_{\mu}+\frac{mc}{\hbar} \right)\psi(\underline{x},t).$$
It must be noted that $\gamma^{0}$ is Hermitian and $\gamma^{k}$ are anti-Hermitian.

Using the $\gamma$ matrices Dirac algebra simplifies to
$$\{ \gamma^{\mu},\gamma^{\nu} \}=2g^{\mu \nu}.$$
Note there are two different sets of indices, $\mu$ and $\nu$, which denote space-time derivatives.

$\gamma^{\mu}$ are 4x4 matrices in spinor space.

With anticommutators the $\mathbb{I}_{4}$ factor is often omitted but is still there, for example the anticommutator of the gamma matrices is $\{ \gamma^{\mu},\gamma^{\nu} \}=2g^{\mu \nu}\mathbb{I}_{4}$ but is often written as $2g^{\mu \nu}$. 

Like the $\alpha^{k}$ and $\beta$ matrices, the form of the $\gamma$ matrices can be changed by a unitary transformation.
The most common form is the chiral form.
$$\gamma^{0}=\begin{bmatrix}
0 & \mathbb{I}_{2} \\
\mathbb{I}_{2} & 0
\end{bmatrix};\;\gamma^{k}=\begin{bmatrix}
0 & \sigma^{k} \\
-\sigma^{k} & 0
\end{bmatrix}.$$
To simplify the Dirac equation, Feynman slash notation is used,
$$\partial \!\!\!/=\gamma^{\mu}\partial_{\mu}.$$
For an arbitrary 4-vector $a^{\mu}$, $a\!\!\!/=\gamma^{\mu}a_{\mu}$.

In this notation the Dirac equation becomes
$$\left( i\partial \!\!\!/-\frac{mc}{\hbar} \right)\psi(\underline{x},t)=0.$$
In natural units,
$$(i\partial \!\!\!/-m)\psi(\underline{x},t)=0.$$
