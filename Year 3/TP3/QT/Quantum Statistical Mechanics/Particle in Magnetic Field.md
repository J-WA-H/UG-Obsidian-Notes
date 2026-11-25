Consider a spin-$\frac{1}{2}$ particle in a magnetic field.
It has [magnetic dipole](Magnetic%20Dipoles.md):
$$\underline{\mu}=-\frac{\mu_{B}\underline{S}}{\hbar}.$$
The Hamiltonian of the system is
$$H=-g\underline{\mu}\cdot \underline{B}.$$
Take the $B$ field to be along the $z$ axis,
$$H=\frac{g\mu_{B}B\sigma_{z}}{2}$$
where $\sigma_{z}=\begin{bmatrix}1 & 0 \\ 0 & -1\end{bmatrix}$.
Using the [[Canonical Ensemble]], the [[Density Operator]] is 
$$\rho=\frac{\exp(-\beta H)}{\mathrm{Tr}(\exp(-\beta H))}=\frac{1}{\mathrm{Tr}(\exp(-\beta H))}\begin{bmatrix}
\exp\left[ {-\frac{\beta g\mu_{B}B}{2}} \right] & 0 \\
0 & \exp\left[ -\frac{\beta g\mu_{B}B}{2} \right]
\end{bmatrix}$$
$$=\frac{1}{\exp\left[ -\frac{\beta g\mu_{B}B}{2} \right]+\exp\left[\frac{\beta g\mu_{B}B}{2} \right]}\begin{bmatrix}
\exp\left[ -\frac{\beta g\mu_{B}B}{2} \right] & 0 \\
0 & \exp\left[ \frac{\beta g\mu_{B}B}{2} \right]
\end{bmatrix}.$$
Compute $\langle S_{z} \rangle$:
$$\langle S_{z} \rangle =\mathrm{Tr}(\rho S_{z})=\frac{\hbar}{2}\mathrm{Tr}(\rho\sigma_{z})=\frac{\hbar}{2} \frac{1}{\exp\left[ -\frac{\beta g\mu_{B}B}{2} \right]+\exp\left[ \frac{\beta g\mu_{B}B}{2} \right]}\left( \exp\left[ -\frac{\beta g\mu_{B}B}{2} \right]-\exp\left[ \frac{\beta g\mu_{B}B}{2} \right] \right)$$
$$=-\frac{\hbar}{2}\tanh\left( \frac{\beta g\mu_{B}B}{2} \right).$$
The average energy of a particle in a box is
$$E_{n}=\frac{\hbar^2}{2\mu}\left( \frac{\pi}{L} \right)^2(n_{x}^2+n_{y}^2+n_{z}^2).$$
The partition function is
$$Q=\sum_{n_{x},n_{y},n_{z}}\exp[-\beta E_{n}].$$
For a large box, the sum becomes an integral
$$Q=\int_{0}^{\infty}n_{x}\int_{0}^{\infty}n_{y}\int_{0}^{\infty}n_{z}e^{-\beta E_{n}}$$
$$\implies Q=L^3\left( \frac{\mu}{2\pi \hbar^2\beta} \right)^{3/2}.$$
Using the relation between energy and the partition function,
$$E=-\frac{d\ln Q}{d\beta}=-\frac{d}{d\beta}\ln\left[ \frac{L^2\mu}{2\pi \hbar^2\beta} \right]^{3/2}=-\frac{3}{2} \frac{d}{d\beta} \left( \ln\left( \frac{L^2\mu}{2\pi \hbar^2} \right)-\ln\beta \right)$$
$$=\frac{3}{2} \frac{d\ln\beta}{d\beta}=\frac{3}{2} \frac{1}{\beta}=\frac{3}{2}k_{B}T.$$
This is the expected energy from equipartition of energy.