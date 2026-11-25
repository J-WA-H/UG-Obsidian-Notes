Electrons in an atom respond to an EM field by transitioning energy levels.

Take the E-field experienced by an atom to be
$$\underline{E}=E_{0}\cos(\omega t)\underline{\hat{z}}.$$
From this we can see the potential from this E-field is
$$V(z,t)=-q\int E(z,t)dz=-qzE_{0}\cos(\omega t).$$
$$\therefore H'(t)=-qzE_{0}\cos(\omega t)$$
We will use the dipole approximation, which assumes the wavelength of the E field is much larger than the extent of the electrons wavefunction.
![[Pasted image 20241102165128.png]]
In this regime we can call the z-component of the electric dipole $p_{z}=qz$, so the perturbation becomes
$$H'(\underline{r},t)=-p_{z}\cos(\omega t).$$
This gives
$$H'_{ba}=\bra{\psi_{b}}H'(z,t)\ket{\psi_{a}}=-(p_{z})_{ba}E_{0}\cos(\omega t).$$
For excitation, the electron starts in state $\psi_{a}$ and is excited by the E field to state $\psi_{b}$, so the probability of this excitation is given by the norm squared of the [probability amplitude for state b](Sinusoidal%20Perturbation.md):
$$P_{b\to a}=\lvert c_{b}^{(1)}(t) \rvert^2 = \frac{\lvert V_{ba}\rvert^2}{\hbar^2} \frac{\sin^2\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{(\omega_{0}-\omega)^2}=\frac{\lvert(p_{z})_{ba}\rvert^2E_{0}^2}{\hbar^2}\frac{\sin^2\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{(\omega_{0}-\omega)^2}$$
As time tends to $\infty$,
$$\lim_{ t \to \infty }\frac{\sin^2\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{(\omega_{0}-\omega)^2}=\frac{\pi t}{2}\delta(\omega-\omega_{0})$$
This gives a probability of excitation:
$$P_{a\to b}=\frac{\lvert(p_{z})_{ba}\rvert^2E_{0}^2}{\hbar^2} \frac{\pi t}{2}\delta(\omega-\omega_{0}).$$
Now for de-excitation, the electron is initially in state $\psi_{b}$ and moves down to state $\psi_{a}$, emitting a photon. As the wavefunction is initially in state b, we swap the a and b indices in the [total wavefunction](Perturbation%20Theory.md):
$$\Psi(t)=\psi_{b}e^{-iE_{b}t/\hbar}-\frac{i}{\hbar}\psi_{a}e^{-iE_{a}t/\hbar}\int_{0}^tdt'\hat{H}'_{ab}(t')e^{-i\omega_{0}t}$$
A similar process can be done to evaluate the integral for $c_{a}^{(1)}(t)$, which yields
$$P_{b\to a}=\lvert c_{a}^{(1)}(t) \rvert^2= \frac{\lvert(p_{z})_{ab}\rvert^2E_{0}^2}{\hbar^2}\frac{\sin^2\left[ \frac{(\omega-\omega_{0})t}{2} \right]}{(\omega-\omega_{0})^2}.$$
From this we can see $P_{a\to b}=P_{b\to a}$, indicating symmetry in the emission and absorption probabilities. 