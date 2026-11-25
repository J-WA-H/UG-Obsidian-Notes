Inflation is designed to solve two problems:
- Why is the universe smooth and isotropic on large scales
- Why is the universe so spatially flat, $k\approx 0 \iff \Omega \approx 1$.

Inflation supposes that at very early times, $(t\sim 10^{-43}\text{ s})$, some initially tiny patch of the universe underwent exponential expansion $\gtrsim 10^{20}$. This gives the whole of the present-day observable universe contained inside this causally connected patch, and the the observable now looks nearly smooth on large scales. The exponential expansion flattens out the curvature so $k\approx 0$ and $\Omega \approx 1$ inside the present day observable universe.

![[Pasted image 20251127120913.png]]

The current theory behind what drives inflation is a scalar field $\phi$ with potential $V(\phi)$. Since this is a scalar field, we are dealing with spin-0 bosons. If $\phi$ is slowly varying, then its energy is dominated by $V(\phi)$ which implies
$$\rho=\frac{V(\phi)}{c^2},\;p=-\rho c^2=-V(\phi)\tag{22.1} .$$
This is similar to the [vacuum energy](Cosmological%20Expansion.md). A nearly constant $V(\phi)$ drives exponential expansion, $a\propto e^{ Ht }$. Here the Hubble's parameter is
$$H^2=\frac{8\pi G}{3} \frac{V(\phi)}{c^2}\approx\text{const.}\tag{22.2} $$
The exponential expansion carries on as long as $V(\phi)$ dominates the total energy density. 

The current favoured model of inflation is the slow-roll model.
![[Pasted image 20251127122254.png]]
The field $\phi$ starts in a false vacuum state with $V(\phi)> 0$. $\phi$ rolls slowly downhill towards the true vacuum state where $V(\phi)=0$ which gives nearly exponential expansion - inflation.
Eventually, $\phi$ starts to oscillate around the minimum in $V(\phi)$. Oscillations covert $\phi$ energy of into particles and radiation - reheating. The universe exits from the inflation era and enters the radiation dominated era. 

Density perturbations originate from quantum fluctuations in $\phi$. $\phi$ has perturbations $\delta \phi(\vec{x},t)$ from the uniform value $\bar{\phi}(t)$. Fourier theorem implies
$$\delta \phi(\vec{x},t)=\sum_{\vec{k}}\phi_{\vec{k}}(t)e^{ i\vec{k}\cdot \vec{x} }\tag{22.3} $$with Fourier amplitude $\phi_{\vec{k}}(t)$ for the mode with wavevector $\vec{k}$.
During inflation, the [horizon size](Perturbations%20Outside%20Horizon.md) $R_{H}=\frac{c}{H}$ is constant but the proper wavelength of each mode stretched as $\lambda \propto a\propto e^{ Ht }$. The modes which start with microscopic wavelengths $\lambda\ll R_{H}$ get stretched until they become macroscopic and exits the horizon ($\lambda>R_{H}$).
![[Pasted image 20251127123619.png]]

Since wavelengths are initially microscopic, quantum effects are important. Each mode $\phi_{\vec{k}}(t)$ behaves like a harmonic oscillator
$$\ddot{\phi}_{\vec{k}}+\omega^2_{\vec{k}}\phi_{\vec{k}}=0\tag{22.4} $$
In quantum mechanics, the harmonic oscillator with frequency $\omega$ has a ground state with energy $E=\frac{1}{2}\hbar \omega$, and has Gaussian wavefunctions for particle displacement $x$, with $\langle x \rangle=0$.
![[Pasted image 20251127123903.png]]
Even in the ground state, the harmonic oscillator in quantum mechanics has non-zero motions, called zero-point fluctuations. This is a consequence of the Heisenberg uncertainty principle.

The same applies to $\phi_{k}$, $\langle \phi_{\vec{k}} \rangle=0$ but $\langle |\phi_{\vec{k}}|^2 \rangle\neq 0$. In fact, $\phi_{\vec{k}}$ also has a Gaussian probability distribution function. The exponential expansion during inflation stretches wavelengths of $\phi_{\vec{k}}$ modes until they are larger than the horizon size. The evolution of $\phi_{\vec{k}}(t)$ for such a mode then becomes classical, and the amplitude freezes for some $\phi_{\vec{k}}$. The perturbations in $\phi$ gives perturbations in density via $\delta \rho=\frac{V'(\phi)}{c^2}$. When inflation ends, fluctuations $\delta \phi$ generate fluctuations in density of matter and radiation. These density fluctuations are adiabatic and obey Gaussian statistics. Density perturbations over the whole range of scales in the present day universe are thus generated during inflation from fluctuations on initially microscopic scales.

We define $\sigma^2_{\phi}(R,t)$ as the variance in $\delta \phi$ measured in spheres of radius $R$:
- $\sigma_{\phi}(R_{H},t)=\text{const}$ for fluctuations $\delta \phi$ as they exit the horizon during inflation which gives density perturbations as they enter the horizon during radiation or matter domination eras obey
$$\sigma(R_{H},t)=\text{const}=\sigma_{H}\tag{22.5} $$
where $\sigma^2(R_{H},t)$ is the variance in $\frac{\delta \rho}{\bar{\rho}}$ in spheres of radius $R_{H}$ at time $t$.
For perturbations of mass $M$ which enter the horizon at $a=a_{enter}(M)$, we have similarly
$$\sigma(M,a_{enter}(M))=\sigma_{H}\tag{22.6} $$i.e. the rms density perturbations has the same value whatever the mass scale at horizon entry.

Consider dark matter perturbations in the matter dominated era with $a_{eq}\ll a_{enter}$. $R_{H}=\frac{c}{H}$ at $a\propto t^{2/3}$, $\bar{\rho}_{m}\propto t^{-2}$. This gives
$$M_{H}\propto \bar{\rho}_{m}R_{H}^3at\propto a^{3/2},\;M\propto \bar{\rho}_{m}\lambda^3.\tag{22.7} $$
Horizon entry is when $\lambda=R_{H}\implies M=M_{H}(a_{enter})\propto a^{3/2}_{enter}$ so
$$a_{enter}(M)\propto M^{2/3}.\tag{22.8} $$
Dark matter perturbations grow as $D_{+}(a)\propto a$ (independent of $M$) so
$$\sigma(M,a)=\sigma(M)D_{+}(a)\propto\sigma(M)a.\tag{22.9} $$
At horizon entry, $\sigma_{H}=\sigma(M,a_{enter}(M))\propto\sigma(M)a_{enter}(M)$$$\implies\sigma(M)\propto a_{enter}^{-1}(M)\propto M^{-2/3}\tag{22.10} .$$
The same result applies for density perturbations entering the horizon during the radiation-dominated era.

Inflation predict $\sigma \propto M^{-2.4}$. Recall for a [power-law power spectrum](Random%20Density%20Fields.md) $$\sigma(M)\propto M^{-(n+3)/6}\tag{21.20} .$$
Hence inflation predicts an initial power spectrum with power law index with $n=1$, i.e.
$$P(k)\propto k.\tag{22.11} $$
This $P(k)$ form is called the Harrison-Zeldovich spectrum. The initial power spectrum of $\delta$ at some early epoch $a_{inf}<a_{i}<a_{enter}$ is
$$P(k,a_{i})=A_{i}k.\tag{22.12} $$Recall [[Transfer Functions]],
$$\frac{D_{+}(k,a_{f})}{D_{+}(k,a_{i})}\equiv \frac{D_{+}(a_{f})}{D_{+}(a_{i})}T(k)\tag{22.13} $$and$$P(k,t_{f})=\left\lvert  \frac{D_{+}(k,t_{f})}{D_{+}(k,t_{i})}  \right\rvert^2P(k,t_{i}).\tag{22.14}  $$
This gives the power spectra for $\delta_{DM}$ at late times
$$P(k,a_{f})=\left( \frac{D_{+}(k,a_{f})}{D_{+}(k,a_{i})} \right)^2P(k,a_{i})=\left( \frac{D_{+}(a_{f})}{D_{+}(a_{i})} \right)^2T^2(k)A_{i}k.\tag{22.15} $$
![[Pasted image 20251127142216.png]]

The shape of the dark matter power spectrum at late times is modified from the primordial power law to
$$P(k)\propto kT^2(k)\tag{22.16}. $$Recall that $T(k)$ describes the net effect of gas pressure, [[Free Streaming of Dark Matter]], Meszaros effect on the growth of dark matter perturbations inside the horizon at $a\lesssim a_{eq}$ and depends on whether dark matter is cold, warm, or hot. For long-wavelength perturbations, $k\lesssim k_{eq}$, the growth of perturbations are not affected by these effects, as $T(k)\to 1$ which implies that $P(k)$ retains its primordial shape, i.e. $P(k)\propto k$. For shorter wavelengths, $k\gtrsim k_{eq}$, the shape is modified, the modification depending on the type of dark matter considered.
Using $(20.9)$, we het
$$P(k)\propto \begin{cases}
 0 & k\gtrsim \frac{2\pi}{\ell_{FS}} \\
k^{-3} & \frac{2\pi}{\ell_{FS}}\gtrsim k\gtrsim k_{eq} \\
k & k\lesssim k_{eq}
\end{cases}\tag{22.17} $$where for CDM, $\ell_{FS}=0$ so the first range disappears. For HDM, $\ell_{FS}\sim \ell_{H_{eq}}$, so the intermediate range disappears. For WDM, all 3 ranges are important
![[Pasted image 20251127143249.png]]
