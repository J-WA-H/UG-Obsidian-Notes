Consider a charged particle in a magnetic field $\underline{B}=B\underline{\hat{z}}$, we wish to solve the [Hamiltonian](Hamiltonian%20for%20Particles%20in%20EM%20field.md) of this system.
Choose [Landau gauge](Gauge%20Freedom.md) $\underline{A}=-By\hat{\underline{x}}$, $\phi=0$:
The Hamiltonian is:
$$\hat{H}=\frac{1}{2m}[-i\hbar \underline{\nabla}-q\underline{A}]^2=\frac{1}{2m}[-\hbar^2\nabla^2+2i\hbar \underline{A}\cdot \underline{\nabla}+q^2\underline{A}\cdot \underline{A}]$$
$$=\frac{1}{2m}\left[ -\hbar^2 \frac{\partial^2}{\partial x^2}-\hbar^2 \frac{\partial^2}{\partial y^2}-2i\hbar qBy \frac{\partial}{\partial x}+q^2B^2y^2 \right]$$
As there is no explicit $x$ dependence in the Hamiltonian, we can take the wavefunction $\psi(x,y)$ to be separable. For convenience choose $\psi(x,y)=e^{-ikx}\phi(y)$
Substitute this wavefunction into Schrödinger's equation, $\hat{H}\psi=E\psi$:
$$\frac{1}{2m}\left[ -\hbar^2 \frac{\partial^2}{\partial x^2}-\hbar^2 \frac{\partial^2}{\partial y^2}-2i\hbar qBy \frac{\partial}{\partial x}+q^2B^2y^2 \right]e^{-ikx}\phi(y)=Ee^{-ikx}\phi(y)$$
$$=\frac{1}{2m}\left[ \hbar^2k^2+q^2B^2y^2-2\hbar qByk-\hbar^2 \frac{d^2}{dy^2}  \right]\phi(y)=E\phi(y)$$
$$=\frac{1}{2m}\left[ -\hbar^2 \frac{\partial^2}{\partial y^2}+(\hbar k-qBy)^2 \right]\phi(y)=E\phi(y)$$
$$=-\frac{\hbar^2}{2m} \frac{d^2\phi(y)}{dy^2}+\frac{q^2B^2}{2m}\left( y-\frac{\hbar k}{qB} \right)^2\phi(y)=E\phi(y)$$
Define $y_{0}=\frac{\hbar k}{qB}$ and $\omega_{C}=\frac{qB}{m}$ - this yields
$$-\frac{\hbar^2}{2m} \frac{d^2\phi}{dy^2}+\frac{1}{2}m\omega_{C}^2(y-y_{0})^2\phi=E\phi.$$
This is the form of a harmonic oscillator of known energy levels where $y_0$ is the centre of oscillation and $\omega_{C}$ is the cyclotron frequency.
The energy levels, known as Landau levels, are hence given by
$$E=\left( n+\frac{1}{2} \right)\hbar \omega_{C}$$
where $n\in \mathbb{Z}$.