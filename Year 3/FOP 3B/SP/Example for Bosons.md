Recall that in the ground state the number of rearrangements of indistinguishable particles is 1, hence we have a 0 entropy fluid.
![[Pasted image 20241205113343.png]]
Consider Helium-4, with two protons, two neutrons and two electrons - [[Compound Bosons]].
![[Pasted image 20241205114010.png]]
Consider photons and phonons, as we have $\mu= 0$, we have the [[Bose-Einstein Distribution]]
$$f_{BE}(\varepsilon)=\frac{1}{e^{\beta\varepsilon}-1}.$$
Vibrations have an energy of $\varepsilon=\hbar \omega$. Given that the average energy per photon/phonon is the product of the average number of particles per state and the energy of that state, we get
$$\frac{U}{N}=f_{BE}(\varepsilon)\hbar \omega=\hbar \frac{\omega}{e^{\beta \hbar \omega}-1}.$$
If we have $n$ oscillators then $\varepsilon_{n}=n\hbar \omega$ if they are in the same state. If we have one oscillator with frequency $n\omega$ then we also have $\varepsilon=n\hbar \omega$. This shows that $n$ oscillators with frequency $\omega\equiv$ one oscillator with frequency $n\omega$.

The photon spectral density - energy in range $\omega\to \omega+d\omega$.
$$U(\omega)d\omega=g(\omega)d\omega f_{BE}(\varepsilon)\hbar \omega.$$
In k-space
$$g(k)=\frac{V}{(2\pi)^3}4\pi k^2dk\times{2}.$$
The multiplication by $2$ is due to the polarisation of photons.
Change of variables $k=\frac{\omega}{c}$.
$$\hbar \omega g(\omega)d\omega f(\omega)=\hbar \omega  \frac{V}{(2\pi)^3}4\pi\left( \frac{\omega}{c} \right)^2 \frac{d\omega}{c}f(\omega)\times 2.$$
The total energy is 
$$U=\int_{-\infty}^{\infty}U(\omega)d\omega=\frac{8\pi k_{B}^4}{15c^3h^3}T^{4}.$$
This is the Stephan-Boltzmann law.

Calculating the number density of phonons.
$$g(\nu)d\nu f(\nu)=\frac{8\pi}{c^3}d\nu  \frac{1}{e^{\beta h\nu}-1}.$$
Integrating over this gives
$$N\approx \frac{60.42k_{B}^3}{c^3h^3}T^3.$$
We this for photons but it isn't exactly the same for phonons. We can run through the same calculation, getting almost identical results except polarisation. Phonons have 3 polarisations instead of 2.