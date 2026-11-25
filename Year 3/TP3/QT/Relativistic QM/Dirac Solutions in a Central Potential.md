Central potentials are common in many physical situations, like [scattering](Potential%20Scattering.md) and the hydrogen atom.

One important calculation is the energy levels of an atomic system, which for hydrogen is
$$E_{n}=-\frac{R_{y}}{n^2}$$where $R_{y}=-13.6\text{ eV}$.
After adding relativistic effects like spin using perturbation theory this gives reasonable agreement with the atomic spectra.

However, if we solve the Dirac for a central potential, all relativistic effects are included.

Start with coupling the [Dirac equation](Dirac%20Equation%20Derivation.md) to an EM field,
$$i\hbar \frac{{\partial \psi}}{\partial t}=(c\alpha^{k}p_{k}+\beta mc^2+e\phi)\psi(\underline{r}).$$
Take $\underline{A}=\underline{0}$, so no magnetic field is present, and the scalar potential $e\phi=V(r)$.
We want stationary solutions
$$\psi(\underline{r},t)=\exp\left[ -\frac{iEt}{\hbar} \right]\psi(\underline{r}).$$
$$\implies E\psi(\underline{r})=[c\alpha^{k}p_{k}+\beta mc^2+V(r)]\psi(\underline{r}).$$
As with the Schrodinger equation, we want to separate the solutions. To do this first consider the angular momentum.
In the non-relativistic case, $\hat{L}^2$ and $\hat{L}_{z}$ commute with the Hamiltonian
$$[\hat{L}^2,H]=[\hat{L}_{z},H]=0.$$
These have conserved quantum numbers and the same eigenvectors.

In the relativistic case, we aim to calculate these commutators with the Dirac Hamiltonian,
$$H_{D}=c\alpha^{k}p_{k}+\beta mc^2+V(r).$$
Look at the commutator of this Hamiltonian with the $m^{th}$ component of orbital angular momentum,
$$[H_{D},L_{m}]=c\alpha^{k}[p_{k},(\underline{r}\times \underline{p})_{m}]+[\beta mc^2,(\underline{r}\times \underline{p})_{m}]+[V(r),(\underline{r}\times \underline{p})_{m}].$$
Calculate 1st term:
$$c\alpha^{k}[p_{k},(\underline{r}\times \underline{p})_{m}]=c\epsilon_{ijm}\alpha^{k}[p_{k},r_{i}p_{j}]=c\epsilon_{ijm}\alpha^{k}(p_{k}r_{i}p_{j}-r_{i}p_{j}p_{k})$$
$$=c\epsilon_{ijm}\alpha^{k}((p_{k}r_{i}-r_{i}p_{k})p_{j}+r_{i}(p_{k}p_{j}-p_{j}p_{k}))=c\epsilon_{ijm}\alpha^{k}([p_{i},r_{i}]p_{j}+r_{i}\cancelto{0}{[p_{k},p_{j}]})$$
$$=-i\hbar c\epsilon_{ijm}a^{i}p_{j}=-i\hbar c(\underline{\alpha}\times \underline{p})_{m}.$$
2nd term: $[\beta mc^2,(\underline{r}\times \underline{p})_{m}]=0$ as $\beta$ is not in space-time or momentum space, but in spinor space.

3rd term:
$$[V(r),(\underline{r}\times \underline{p})_{m}]=\epsilon_{ijm}[V(r),r_{i}p_{j}]=\epsilon_{ijm}r_{i}[V(r),p_{j}]=-i\hbar\epsilon_{ijm}r_{i}\left( V(r) \frac{\partial}{\partial r^{j}}-\frac{\partial}{\partial r^{j}}V(r) \right)$$
$$=-i\hbar\epsilon_{ijm}r_{i}\left( V(r) \frac{\partial}{\partial r^j}-V(r) \frac{\partial}{\partial r^j}-\frac{\partial V(r)}{\partial r^{j}} \right)=-i\hbar(\underline{r}\times \underline{\nabla}V)_{m}.$$
For a central potential, the gradient points radially so $\underline{r}\times \underline{\nabla}V=9$.

This gives the total commutator of
$$[H_{D},L_{m}]=-i\hbar c(\underline{\alpha}\times \underline{p})_{m}\neq{0}.$$
This makes sense as orbital angular momentum may not necessarily be conserved, but total angular momentum must be conserved.
$$\underline{J}=\underline{L}+\underline{S};\;\underline{S}=\frac{\hbar}{2}\underline{\Sigma}$$
where
$$\underline{\Sigma}=\begin{bmatrix}
\sigma_{k} & 0 \\
0 & \sigma_{k}
\end{bmatrix}.$$
For spin, $[H_{D},\underline{S}]=i\hbar c(\underline{\alpha}\times \underline{p})$
$$\therefore [H_{D},\underline{J}]=[H_{D},\underline{L}]+[H_{D},\underline{S}]=-i\hbar c(\underline{\alpha}\times \underline{p})+i\hbar c(\underline{\alpha}\times \underline{p})=0.$$
As $[H_{D},\underline{J}]=0$, we can describe energy states in terms of the total angular momentum $J^2,J_{z}$.

We can rewrite the Dirac Hamiltonian as
$$H_{D}=c\alpha_{r}p_{r}+\frac{i\hbar c}{r}\alpha_{r}\beta \kappa+\beta mc^2+V(r)$$
where
$$p_{r}=-i\hbar \frac{1}{r} \frac{\partial}{\partial r}r;\;\alpha_{r}=\frac{{\underline{\alpha}\cdot \underline{r}}}{r};\;\kappa=\frac{\beta}{\hbar^2}\left[ J^2-L^2+\frac{\hbar^2}{4} \right].$$
Use the trial solution
$$\psi^{\ell}_{jm_{j}}=\frac{1}{r} \begin{bmatrix}
G_{\ell j}(r)\phi^{\ell}_{jm_{j}}(\theta,\phi) \\
-iF_{\ell j}(r) \frac{{\underline{\sigma}\cdot \underline{r}}}{r}\phi^{\ell}_{jm_{j}}(\theta,\phi)
\end{bmatrix}.$$
where
$$\phi^{\ell}_{jm_{j}}=\begin{cases}
\phi^{+}_{jm_{j}} & j=\ell+\frac{1}{2} \\
\phi^-_{jm_{j}} & j=\ell-\frac{1}{2}
\end{cases}$$
where $\phi^\pm_{j_{m_{j}}}$ are 2-component spinors defined by
$$\phi^+_{jm_{j}}(\theta,\phi)=\begin{bmatrix}
\sqrt{ \frac{{\ell+m_{j}+\frac{1}{2}}}{2\ell+1} }Y_{\ell,m_{j}-\frac{1}{2}}(\theta,\phi) \\
\sqrt{ \frac{{\ell-m_{j}+\frac{1}{2}}}{2\ell+1} }Y_{\ell,m_{j}+\frac{1}{2}}(\theta,\phi)
\end{bmatrix}$$
$$\phi^-_{jm_{j}}(\theta,\phi)=\begin{bmatrix}
\sqrt{ \frac{{\ell-m_{j}+\frac{1}{2}}}{2\ell+1} }Y_{\ell,m_{j}-\frac{1}{2}}(\theta,\phi) \\
-\sqrt{ \frac{{\ell+m_{j}+\frac{1}{2}}}{2\ell+1} }Y_{\ell,m_{j}+\frac{1}{2}}(\theta,\phi)
\end{bmatrix}.$$
$$\frac{{\underline{\sigma}\cdot \underline{r}}}{r}\phi^{\pm}=\phi^{\mp}.$$
Looking at the Dirac equation,
$$E\psi=H_{D}\psi \implies(H_{D}-E)\psi=0.$$
$$-i\hbar c \frac{{\underline{\alpha}\cdot \underline{r}}}{r} \frac{1}{r} \frac{\partial}{\partial r}(r\psi)+\frac{{i\hbar c}}{r} \frac{{\underline{\alpha}\cdot \underline{r}}}{r} \frac{1}{\hbar^2}\left( J^2-L^2+\frac{\hbar^2}{4} \right)\psi+\beta mc^2\psi+V(r)\psi-E\psi=0$$
As a matrix equation this becomes$$\begin{bmatrix}
(mc^2+V(r)-E)\mathbb{I}_{2} & -\frac{{i\hbar c}}{r} \frac{{\underline{\sigma}\cdot \underline{r}}}{r} \frac{1}{r} \frac{\partial}{\partial r}(r)+i\hbar \frac{c}{r} \frac{{\underline{\sigma}\cdot \underline{r}}}{\hbar^2r}\left( J^2-L^2+\frac{\hbar^2}{4} \right) \\
-\frac{{i\hbar c}}{r} \frac{{\underline{\sigma}\cdot \underline{r}}}{r}\frac{1}{r} \frac{\partial}{\partial r}(r)+i\hbar \frac{c}{r} \frac{{\underline{\sigma}\cdot \underline{r}}}{\hbar^2r}\left( J^2-L^2+\frac{\hbar^2}{4} \right) & (-mc^2+V(r)-E)\mathbb{I}_{2}
\end{bmatrix}$$$$\frac{1}{r}\begin{bmatrix}
G_{\ell j}\phi^{\pm} \\
-iF_{\ell j}\phi^\pm
\end{bmatrix}=0.$$
Expanding the first row gives
$$(mc^2+V(r)-E) \frac{G_{\ell j}(r)}{r}\phi^{\pm}(\theta,\phi)+\frac{\hbar c}{r} \frac{{\underline{\sigma}\cdot \underline{r}}}{r}\left( \mp\left( j+\frac{1}{2} \right) \right) \frac{F_{\ell j}(r)}{r}\phi^{\mp}$$
$$\implies(E-V(r)-mc^2)G_{\ell j}(r)\cancel{\phi^{\pm}}=-\hbar c \frac{\partial F_{\ell j}}{\partial r}\cancel{\phi^{\pm}}\mp \frac{\hbar c}{r}\left( j+\frac{1}{2} \right)F_{\ell j}\phi^{\pm}$$
$$\therefore \frac{{E-mc^2-V(r)}}{\hbar c}G_{\ell j}(r)=\frac{dF_{\ell j}}{dr}\mp\left( j+\frac{1}{2} \right) \frac{F_{\ell j}(r)}{r}.$$
For the second row,
$$\frac{E+mc^2-V(r)}{\hbar c}F_{\ell j}(r)=\frac{dG_{\ell j}}{dr}\mp\left( j+\frac{1}{2} \right)F_{\ell j}(r).$$
This gives a pair of coupled differential equations.
For the hydrogen atom
$$V(r)=\frac{Z\alpha}{r}.$$
Solving these can be done similar to the NR hydrogen atom, setting $\rho=vr$ where
$$v=\frac{mc}{\hbar}\left( 1-\frac{E^2}{m^2c^4} \right)^{1/2}.$$
This gives two differential equations.
Looking at the high-radius behaviour,
$$G\to a_{1}e^{-\rho}$$
$$F\to a_{2}e^{-\rho}$$
$$\implies \frac{a_{1}}{a_{2}}=-\left( \frac{{1+\frac{E}{mc^2}}}{1-\frac{E}{mc^2}} \right)^{1/2}$$
$$\therefore G=N\left( 1+\frac{E}{mc^2} \right)^{1/2}e^{-\rho}g(\rho)$$
$$F=N\left( 1-\frac{E}{mc^2} \right)^{1/2}e^{-\rho}f(\rho).$$
$g(\rho),f(\rho)$ can be found using a power series.
$$g(\rho)=\rho^{5}\sum_{k=0}^{\infty}c_{k}\rho^{k};\;f(\rho)=\rho^{5}\sum_{k=0}^{\infty}d_{k}\rho^{k}.$$
Find a recurrence relation with a termination condition gives the energy levels
$$E_{nj}=\frac{mc^2}{\sqrt{ 1+\left( \frac{Z\alpha}{n-\left( j+\frac{1}{2} \right)+\sqrt{ \left( j+\frac{1}{2} \right)^2-(Z\alpha)^2 }} \right)^2 }}.$$
This predicts degenerate energy levels for the same $n$ and $j$ but different for $J_{z}$, $L^2$.
To gain insight, Taylor expand the energy levels.
$$E_{nj}\approx mc^2\left( 1-\frac{Z^2\alpha^2}{2n^2}-\frac{Z^4\alpha^{4}}{2n^3}\left( \frac{1}{j+\frac{1}{2}} -\frac{3}{4n}\right)+\mathcal{O}(Z^6\alpha^{6}) \right).$$
The first time is the rest mass energy, the second term is the non-relativistic energy and the third term is the relativistic correction. This naturally gives the spin and relativistic corrections.

There is a further splitting from the Lamb shift that needs quantum field theory to evaluate.

