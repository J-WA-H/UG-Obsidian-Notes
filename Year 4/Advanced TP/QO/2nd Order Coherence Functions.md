First order [[Coherence Functions]] may be understood as the factorisation of expectation values of the field,
$$|\langle E^{*}(x_{1})E(x_{2}) \rangle |=\sqrt{ \langle |E(x_{1})|^2 \rangle  }\sqrt{ \langle |E(x_{2})|^2 \rangle  }.\tag{12.1} $$
$$|\langle \hat{E}^{-}(x_{1})\hat{E}^{+}(x_{2}) \rangle |=\sqrt{ \langle \hat{E}^{-}(x_{1})\hat{E}^{+}(x_{1}) \rangle  }\sqrt{ \langle \hat{E}^{-}(x_{2})\hat{E}^{+}(x_{2}) \rangle  }.\tag{12.2} $$
Young's double slit can determine monochromaticity of a light source, or coherence length, but it conveys nothing about the statistical properties of light. 
Since the mode field in a number or coherent states have very different photon number distributions, but both are first-order coherent.

Consider the Hanbury Brown Twiss experiment,
![[Pasted image 20251104102620.png]]
where the two detectors are equidistant from the beam splitter.

The rate of coincidence counts is proportional to $\langle I(t)U(t+\tau) \rangle$ with $I$ being the instantaneous intensity at the detectors.

Assuming stationary fields, $\langle I(t)I(t+\tau) \rangle$ is a function of just $\tau$ and $\langle I(t) \rangle=\langle I(t+\tau) \rangle$.

The probability of a coincidence count is given by
$$\gamma^{(2)}(\tau)=\frac{{\langle I(t)I(t+\tau) \rangle }}{\langle I(t) \rangle ^2}\tag{12.3} .$$This gives the second order classical coherence function
$$\gamma^{(2)}(\tau)=\frac{{\langle E^{*}(t)E^{*}(t+{\tau})E(t+\tau)E(t) \rangle }}{\langle E^{*}(t)E(t) \rangle^2 }.\tag{12.4} $$More generally,
$$\gamma^{(2)}(x_{1},x_{2};x_{2},x_{1})=\frac{{\langle E^{*}(x_{1})E^{*}(x_{2})E(x_{2})E(x_{1}) \rangle }}{\langle E^{*}(x_{1})E(x_{1}) \rangle \langle E^{*}(x_{2})E(x_{2}) \rangle }.\tag{12.5} $$
For complete coherence, both $|\gamma^{(1)}(x_{1},x_{2})|=1$ and $\gamma^{(2)}(x_{1},x_{2};x_{2},x_{1})=1$. This requires the factorisation,
$$\langle E^{*}(x_{1})E^{*}(x_{2})E(x_{2})E(x_{1}) \rangle =\langle |E(x_{1})|^2 \rangle \langle |E(x_{2})|^2 \rangle \tag{12.6} .$$
Consider a plane wave propagating in the $z$ direction, $E(z,t)=E_{0}e^{ i(kz-\omega t) }$. It follows that
$$\langle E^{*}(t)E^{*}(t+\tau)E(t+\tau)E(t) \rangle =E_{0}^{4},\;\langle E^{*}(t)E(t) \rangle =E_{0}^2\tag{12.7}. $$Hence $\gamma^{(2)}(\tau)=1$, complete coherence holds for any beam of constant, non-fluctuating intensity.

Note $\langle I(t)^2 \rangle-\langle I(t) \rangle^2=\langle [I(t)-\langle I(t) \rangle]^2 \rangle\geq0$. Hence $\langle I(t)^2 \rangle\geq \langle I(t) \rangle^2$. It follows that
$$1\leq \gamma^{(2)}(0)<\infty \tag{12.8} $$so that $\gamma^{(2)}(0)$ is finite.

The Cauchy-Schwatz inequality gives
$$\langle I(t)I(t+\tau) \rangle ^2\leq \langle I(t)^2 \rangle \langle I(t+\tau)^2 \rangle .\tag{12.9} $$
For stationary fields, $\langle I(t+\tau)^2 \rangle=\langle I(t)^2 \rangle$ so $\langle I(t)I(t+\tau) \rangle\leq \langle I(t)^2 \rangle$.
Hence $\gamma^{(2)}(\tau)\leq \gamma^{(2)}(0)$.

In general, for chaotic light sources
$$\gamma^{(2)}(\tau)=1+|\gamma^{(1)}(\tau)|^2\tag{12.12} .$$Since $0\leq |\gamma^{(1)}(\tau)|\leq 1$, $1\leq |\gamma^{(2)}(\tau)|\leq 2$. For a chaotic light source with a Lorentzian frequency spectrum,
$$\gamma^{(2)}(\tau)=1+e^{ -2|\tau|/\tau_{0} }.\tag{12.13} $$
It can be understood as photons arriving in pairs at zero time delay and independently at long time delays. This is the photon bunching effect.

For the quantum case, limit ourselves to scalar fields.
the transition probability for the absorption of two photons analogously
$$|\bra{f}\hat{E}^{+}(x_{2})\hat{E}^{+}(x_{1})\ket{i}  |^2.\tag{12.14} $$
Summing over all possible final states similarly produces
$$\bra{i} \hat{E}^{-}(x_{1})\hat{E}^{-}(x_{2})\hat{E}^{+}(x_{2})\hat{E}^{+}(x_{1})\ket{i} .\tag{12.15}  $$
Generalising to mixed states, define the quantum second order correlation function
$$G^{(2)}(x_{1},x_{2};x_{2},x_{1})=\mathrm{Tr}[\rho_{F}\hat{E}^{-}(x_{1})\hat{E}^{-}(x_{2})\hat{E}^{+}(x_{2})\hat{E}^{+}(x_{1})].\tag{12.16} $$
Normalising this gives the second order coherence function,
$$g^{(2)}(x_{1},x_{2};x_{2},x_{1})=\frac{G^{(2)}(x_{1},x_{2};x_{2},x_{1})}{G^{(1)}(x_{1},x_{1})G^{(1)}(x_{2},x_{2})}\tag{12.17}. $$
This is the joint probability of measuring a photon at $x_{1}$ and another at $x_{2}$.

For complete coherence, $|g^{(1)}(x_{1},x_{2})|=1$ and $g^{(2)}(x_{1},x_{2};x_{2},x_{1})=1$. This requires the factorisation $$G^{(2)}(x_{1},x_{2};x_{2},x_{1})=G^{(1)}(x_{1},x_{1})G^{(1)}(x_{2},x_{2})\tag{12.18}. $$For time delay only, at fixed position (equidistant detectors), coherence function of a time delay $\tau=t_{2}-t_{1}$ only
$$g^{(2)}(\tau)=\frac{{\langle \hat{E}^{-}(t)\hat{E}^{-}(t+\tau)\hat{E}^{+}(t+\tau)\hat{E}^{+}(t) \rangle }}{\langle \hat{E}^{-}(t)\hat{E}^{+}(t) \rangle \langle \hat{E}^{-}(t+\tau)\hat{E}^{+}(t+\tau) \rangle }.\tag{12.19} $$
For a quantised single mode plane wave, $\hat{E}^{+}(x)=iK\hat{a}e^{ i(\vec{k}\cdot \vec{x}-\omega t) }$. From this follows
$$g^{(2)}(\tau)=\frac{{\langle \hat{a}^{\dagger}\hat{a}^{\dagger}\hat{a}\hat{a} \rangle }}{\langle \hat{a}^{\dagger}\hat{a} \rangle ^2}=\frac{{\langle \hat{N}(\hat{N}-1) \rangle }}{\langle \hat{N} \rangle ^2}.\tag{12.20} $$
Bringing in number variance $\langle \Delta \hat{N}^2 \rangle$,
$$g^{(2)}(\tau)=1+\frac{{\langle \Delta \hat{N}^2 \rangle -\langle \hat{N} \rangle }}{\langle \hat{N} \rangle ^2}.\tag{12.21} $$
For a coherent state $\ket{\alpha}$, $g^{(2)}(\tau)=1$. 
For a single-mode thermal state $g^{(2)}(\tau)=2$.
For a multi-mode thermal state, $g^{(2)}(\tau)=1+|g^{(1)}(\tau)|^2$.

For collision broadened light with a Lorentzian spectrum,
$$g^{(1)}(\tau)=e^{ -i\omega \tau-|\tau|/\tau_{0} };\;g^{(2)}(\tau)=1+e^{ -2|\tau|/\tau_{0} }.\tag{12.22} $$
This is identical to the classical results, including branching.

For single mode number states $\ket{n}$,
- When $n=0,1$ then $g^{(2)}(\tau)=g^{(2)}(0)=0$
- When $n\geq 2$, then $g^{(2)}(\tau)=g^{(2)}(0)=1-\frac{1}{n}$.
- $g^{(2)}(\tau)\leq 1$ which is classically impossible.

