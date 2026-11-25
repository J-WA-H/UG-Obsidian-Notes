The [[Klein-Gordon Equation]] was obtained by applying the correspondence principle to the relativistic energy.

Dirac said that the [inconsistencies](Interpreting%20Klein-Gordon%20Solutions.md) were due to the second order time derivative. This lead to a consistent first order wave equation.

Ansatz: The wavefunction obeys
$$i\hbar \frac{ \partial \psi }{ \partial t }=H_{D}\psi(\underline{x},t) $$
where $H_{D}$ is the Dirac Hamiltonian,
$$H_{D}=-i\hbar c\sum_{k=1}^{3}\alpha^{k} \frac{ \partial }{ \partial x^{k} }+\beta mc^2.$$
The coefficients are such that $\alpha,\beta$ are dimensionless.

This is the most general form with a combination of spatial derivatives (momentum operators) and constant term proportional to the rest mass.
$$H_{D}=\underline{\alpha}\cdot \underline{p}+\beta mc^2$$
where $\underline{p}=-i\hbar \underline{\nabla}$.
Any relativistic particle obeys the energy/momentum relation
$$E^2\psi(\underline{x},t)=(p^2c^2+m^2c^4)\psi(\underline{x},t)$$
$$\implies H_{D}^2\psi(\underline{x},t)=(-\hbar^2c^2\nabla^2+m^2c^4)\psi(\underline{x},t)$$
Using Einstein notation,
$$H_{D}^2=(-i\hbar c\alpha^{j}\partial_{j}+\beta mc^2)(-i\hbar c\alpha^{k}\partial_{k}+\beta mc^2)$$
$$=-\hbar^2c^2\alpha^{j}\alpha^{k}\partial_{j}\partial_{k}-im\hbar c^3\alpha^{j}\beta \partial_{j}-i\hbar c^3m\beta\alpha^{k}\partial_{k}+\beta^2m^2c^4.$$
Define the anticommutator:
$$\{ A,B \}=AB+BA.$$
This is zero if the matrices are anticommutative, $AB=-BA$ - like swapping fermions in a wavefunction.

Consider $$\alpha^{j}\alpha^{k}\partial_{j}\partial_{k}=\frac{1}{2}(\alpha^{j}\alpha^{k}\partial_{j}\partial_{k}+\alpha^{j}\alpha^{k}\partial_{k}\partial_{j}).$$
Since the two 4-gradiants don't act on each other, their order can be swapped around for the second term. Now swap the $j$ and $k$ indices in the second term,
$$\alpha^{j}\alpha^{k}\partial_{j}\partial_{k}=\frac{1}{2}(\alpha^{j}\alpha^{k}+\alpha^{k}\alpha^{j})\partial_{j}\partial_{k}=\frac{1}{2}\{ \alpha^{j},\alpha^{k} \}\partial_{j}\partial_{k}.$$
$$\therefore H_{D}^2=-\frac{1}{2}\hbar^2c^2\{ \alpha^{j},\alpha^{k} \}\partial_{j}\partial_{k}-im\hbar c^3\{ \alpha^{j},\beta \}\partial_{j}+\frac{1}{2}mc^2c^4\{ \beta,\beta \}.$$
From relativistic energy this expression must be equal to $-\hbar^2c^2\partial_{j}\partial_{j}+m^2c^4$ where $\partial_{j}\partial_{j}=\nabla^2$.
Equating like terms gives
$$-\frac{1}{2}\hbar^2c^2\{ \alpha^{j},\alpha^{k} \}=-\hbar^2c^2\delta_{jk}$$
$$\implies \{ \alpha^{j},\alpha^{k} \}=2\delta_{jk}.$$
$$-i\hbar c^3m\{ \alpha^{j},\beta \}=0$$
$$\implies \{ \alpha^{j},\beta \}=0.$$
$$\frac{1}{2}m^2c^4\{ \beta,\beta \}=m^2c^4$$
$$\implies \{ \beta,\beta \}=2.$$
This defines Dirac algebra,
$$\{ \alpha^{j},\alpha^{k} \}=2\delta_{jk} $$
$$\{ \alpha^{j},\beta \}=0$$
$$\{ \beta,\beta \}=2.$$
Any matrices that satisfy Dirac algebra are called Dirac matrices.
We will use
$$\alpha^{k}=\begin{bmatrix}
0 & \sigma^{k} \\
\sigma^{k} & 0
\end{bmatrix};\;\beta=\begin{bmatrix}
\mathbb{I}_{2} & 0 \\
0 & -\mathbb{I}_{2}
\end{bmatrix}$$
where $\sigma^{k}$ is the $k^{th}$ Pauli matrix.
This gives 4x4 matrices, for example
$$\alpha^{1}=\begin{bmatrix}
0 & 0 & 0 & 1 \\
0 & 0 & 1 & 0 \\
0 & 1 & 0 & 0 \\
1 & 0 & 0 & 0
\end{bmatrix};\;\beta=\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{bmatrix}.$$
Consider $\{ \beta,\beta \}=2$, as the product of two 4x4 matrices is a matrix, saying it equals 2 means it equals $2\mathbb{I}_{4}$.

Properties:
- Must be at least 4x4 matrices to satisfy Dirac algebra
- Hamiltonian must be Hermitian $\implies\alpha^{k},\beta^{k}$ must also be Hermitian.
- Representation is not unique,
	e.g. $\tilde{\alpha}^{k}=Ma^{k}M^{-1}$, $\tilde{\beta}=M\beta M^{-1}$ also satisfies Dirac algebra.
	These new matrices must be Hermitian 
	$$\tilde{\beta}^{\dagger}=(M\beta M^{-1})^{\dagger}=(M^{-1})^{\dagger}\beta M^{\dagger}=\tilde{\beta}=M\beta M^{-1}$$
	$$\implies M^{-1}=M^{\dagger}.$$
	To satisfy Dirac algebra $\alpha^{k},\beta$ can undergo any [unitary transform](Unitary%20and%20Orthogonal%20Operators.md).

- As $\alpha^{k}, \beta$ are 4x4 matrices, $\psi$ has 4 components.
$$\psi=\begin{bmatrix}
\psi_{1} \\
\psi_{2} \\
\psi_{3} \\
\psi_{4}
\end{bmatrix}.$$
This is the Dirac spinor.
The evolution of the components is coupled by the Dirac equation.