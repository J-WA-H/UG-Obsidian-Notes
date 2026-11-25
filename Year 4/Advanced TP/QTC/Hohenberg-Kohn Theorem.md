DFT aims to obtain properties (not just density and energy) of the ground state of an interacting electronic system without solving Schrodinger's equation. The key quantity in DFT is $\rho(\vec{r})$.
$$\rho(\vec{r})=N\sum_{\sigma_{1},\dots,\sigma_{N}}\int d^3r_{2}\dots \int d^3r_{N}|\Psi(\vec{r}_{1},\sigma_{1}; \vec{r}_{2},\sigma_{2};\dots;\vec{r}_{N},\sigma_{N})|^2\tag{7.1} .$$
Hohenberg-Kohn theorem states that there is a 1-1 mapping between potentials and density in the ground state.
![[Pasted image 20260130144014.png]]
Different potentials have a different N-electron ground state densities. Shifting a potential does not affect the properties of a system.
![[Pasted image 20260130144106.png]]
$V(\vec{r})-V'(\vec{r})=const$ does not give a unique density and does not affect the properties of the system.

Hohenberg-Kohn theorem guarantees that the mapping between $\{ V(\vec{r}) \}$ and $\{ \rho(\vec{r}) \}$ is 1-1/ Different potentials $V(\vec{r})\neq V'(\vec{r})$ means $V,V'$differ by more than a constant.

We can prove the Hohenberg-Kohn theorem in 2 lemmas:
- Lemma 1: Different potentials $V\neq V'$ lead to different ground state N-electron wavefunctions $\psi\neq \psi'$,
$$\begin{matrix}
\left( T+V_{ee}+\sum_{i}V(\vec{r}_{i}) \right)\psi=E\psi \\
\left( T+V_{ee}+\sum_{i}V'(\vec{r}_{i}) \right)\psi=E'\psi
\end{matrix}\tag{7.2} .$$
	Assuming the opposite arrives at something absurd.
	![[Pasted image 20260204113648.png]]
	Taking the difference between the two equations in $(7.2)$
$$\sum_{i}[V(\vec{r}_{i})-V'(\vec{r}_{i})]\psi(\vec{r}_{1},\vec{r}_{2},\dots,\vec{r}_{N})=(E-E')\psi(\vec{r}_{1},\vec{r}_{2},\dots,\vec{r}_{N})\tag{7.3} $$
	Since there is no kinetic energy term, $\psi$ is a delta function but it must have a finite kinetic energy operator. Divide through by $\psi$,
$$\sum_{i}[V(\vec{r}_{i})-V'(\vec{r}_{i})]=E-E'=const\tag{7.4} .$$
	This contradicts the assumption that $V,V'$ differ by more than a constant so they are the same potential. This means $V,\psi$ are 1-1.

Lemma 2: Different ground state wavefunctions $\psi\neq \psi'$ gives different densities $\rho\neq \rho'$. $\psi$ is a ground state wavefunction of $V(\vec{r})$,
$$\begin{matrix}
\left( T+V_{ee}+\sum_{i}V(\vec{r}_{i}) \right)\psi=E\psi \\
\left( T+V_{ee}+\sum_{i}V'(\vec{r}_{i}) \right)\psi'=E'\psi'
\end{matrix}\tag{7.5}$$
Assuming no degeneracy, use [Rayleigh-Ritz](Review%20of%20QM.md),
$$\begin{matrix}
\bra{\psi} T+V_{ee}+V\ket{\psi} <\bra{\psi'} T+V_{ee}+V\ket{\psi'} \\
\bra{\psi'} T+V_{ee}+V'\ket{\psi'} <\bra{\psi} T+V_{ee}+V'\ket{\psi} 
\end{matrix}\tag{7.6}. $$
These are from the fact that $\psi,\psi$ are the ground state wavefunctions are of their respective potential. Add these two together.
$$\cancel{\bra{\psi} T+V_{ee}\ket{\psi} }+\underbrace{ \bra{\psi} V\ket{\psi} }_{ =\int d^3r\rho(\vec{r})V(\vec{r}) } +\cancel{\bra{\psi'} T+V_{ee}\ket{\psi'} }+\bra{\psi'} V'\ket{\psi'} <\cancel{\bra{\psi'} T+V_{ee}\ket{\psi'} }+\bra{\psi'}V \ket{\psi'}+\cancel{\bra{\psi} T+V_{ee}\ket{\psi} }+\bra{\psi}V'\ket{\psi}  \tag{7.7}   .$$
$$\int d^3r\rho(\vec{r})V(\vec{r})+\int d^3r\rho'(\vec{r})V'(\vec{r})-\int d^3r\rho'(\vec{r})V(\vec{r})-\int d^3r\rho(\vec{r})V'(\vec{r})<0\tag{7.8}. $$
$$\implies \int d^3r\rho'(\vec{r})[V'(\vec{r})-V(\vec{r})]+\int d^3r\rho(\vec{r})[V(\vec{r})-V'(\vec{r})]<0\implies \int d^3r[V'(\vec{r})-V(\vec{r})][\rho(\vec{r})-\rho'(\vec{r})]\tag{7.9} $$
If $\psi\neq \psi'$ gives $\rho=\rho'$ then $\rho'(\vec{r})-\rho(\vec{r})=0\implies 0<0$ which is false, so by contradiction $\psi$ and $\rho$ are 1-1. This then proves Hohenberg-Kohn theorem, as combining both lemmas gives $V,\rho$ are 1-1.
