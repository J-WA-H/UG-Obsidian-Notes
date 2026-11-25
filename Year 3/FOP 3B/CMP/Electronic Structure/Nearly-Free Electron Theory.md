As we are treating the electron wavefunctions as plane waves, they undergo constructive interference at the Bragg condition
$$\lambda=2d\sin \theta$$
$$\implies k^2=(\underline{k}+\underline{G})^2$$
where $\underline{G}$ is the reciprocal vector.
Constructive interference occurs at
$$\underline{k}=\pm \frac{\underline{G}}{2}$$i.e. the Brillouin zone boundaries.

Consider a 1D chain of atoms with periodic spacing $a$
![[Pasted image 20250117115248.png]]
At the Brillouin zone boundary, the possible wavefunctions are $\psi_{BZ}=e^{i\pi x/a},e^{-i\pi x/a}$. These two wavefunctions interfere be either adding or subtracting from one another
$$\psi^{+}=e^{i\pi x/a}+e^{-i\pi x/a}=2\cos\left( \frac{\pi}{a}x \right)$$
$$\psi^{-}=e^{i\pi x/a}-e^{-i\pi x/a}=2i\sin\left( \frac{\pi}{a}x \right).$$
![[Pasted image 20250117122207.png]]
The probability distributions for $|\psi^{+}|^2,|\psi^{-}|^2$ are out of phase with each other.
$\psi^{+}$ peaks at lower distances so is the lower energy solution.
$\psi^{-}$ peaks at higher distances so is the higher energy solution.

At the Brillouin zone boundary, the energy states are non-degenerate.

![[Pasted image 20250117122757.png]]

The wavefunction can be denoted as a ket vector
$$\ket{\underline{k}}=e^{i\underline{k}\cdot \underline{r}} $$
where
$$H_{0}\ket{\underline{k}}=E_{0}\ket{\underline{k}}.$$
$H_{0}$ is the unperturbed Hamiltonian, and $E_{0}$ is the unperturbed energy.

In the nearly free electron model we treat the ionic interactions, $V_{ion}(\underline{r})$ as a perturbation.
$$H_{0}\to H_{0}+V_{ion}(\underline{r}).$$
Applying 2nd order non-degenerate perturbation theory gives an energy level
$$E(\underline{k})=E_{0}(\underline{k})+\bra{\underline{k}}V_{ion}\ket{\underline{k}}+\sum_{\underline{k}'\neq \underline{k}} \frac{\bra{\underline{k}'}V_{ion}\ket{\underline{k}}}{E_{0}(\underline{k})-E_{0}(\underline{k}')}$$
where 
$$\bra{\underline{k}'}V_{ion}\ket{\underline{k}}=\int \psi_{k'}^{*}V_{ion}\psi_{k}d^3r=\int e^{i(\underline{k}-\underline{k}')\cdot \underline{r}}V_{ion}d^3r.$$
This gives a Fourier transform.

$\bra{\underline{k}}V_{ion}\ket{\underline{k}}=V_{\underline{0}}$ which we will set to zero.

Consider case close to the origin.
![[Pasted image 20250117125303.png]]
There is a large difference between $E_{0}(\underline{k})$ and $E_{0}(\underline{k}')$ so the denominator in the second term is small so $k\to 0$ does not perturb the Hamiltonian.

For the case close to the Brillouin zone boundary.
![[Pasted image 20250117125453.png]]
Here $E_{0}(\underline{k})\approx E_{0}(\underline{k}')$ so there is a large contribution to the second term, and the Brillouin zone boundary is degenerate.

This can be modelled using degenerate perturbation theory.

Near the Brillouin zone the mixing of $\ket{\underline{k}},\ket{\underline{k}'}$ gives a new wavefunction, with $\underline{k}=\underline{k}'-\underline{G}$
$$\ket{\psi}=\alpha \ket{\underline{k}}+\beta \ket{\underline{k}'}.$$
$\alpha,\beta$ are given by
$$\begin{bmatrix}
H_{11} & H_{12} \\
H_{21} & H_{22}
\end{bmatrix}\begin{bmatrix}
\alpha \\
\beta
\end{bmatrix}=E\begin{bmatrix}
\alpha \\
\beta
\end{bmatrix}.$$
$$H_{11}=\bra{\underline{k}}H\ket{\underline{k}}=\bra{\underline{k}}H_{0}+V_{ion}\ket{\underline{k}}=\bra{\underline{k}}H_{0}\ket{\underline{k}}+\cancelto{0}{\bra{\underline{k}}V_{ion}\ket{\underline{k}}  }=E_{0}  $$
$$H_{22}=E_{0}$$
$$H_{12}=\bra{\underline{k}}H_{0}+V_{ion}\ket{\underline{k}'}=\bra{\underline{k}}H_{0}\ket{\underline{k}'}+\bra{\underline{k}}V_{ion}\ket{\underline{k}'}=V_{\underline{k}-\underline{k}'}=V_{\underline{G}}$$
$$H_{21}=V_{-\underline{G}}=V_{\underline{G}}^{*}.$$
This gives non-trivial solutions of $E=E_{0}\pm V_{G}$ $\alpha=\pm \beta$
$$\psi=\frac{1}{\sqrt{ 2 }}(\ket{\underline{k}}\pm \ket{\underline{k}'}  ).$$
This produces band gaps of $2\lvert V_{G} \rvert$.
![[Pasted image 20250117143127.png]]
