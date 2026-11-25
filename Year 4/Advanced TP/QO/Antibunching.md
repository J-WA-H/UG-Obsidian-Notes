The [[Quantum Coherence Function]] $g^{(2)}(\tau)$ characterises the joint probability of detecting one photon followed by another within a time $\tau$ later.
Antibunching is when $g^{(2)}(\tau)$ increases from some initial $g^{(2)}(0)$. This is contrasted to bunching, which for a multimode thermal field $g^{(2)}(0)=2$ and $g^{(2)}(\tau)\to 1$ (photons independent) as $\tau\to \infty$.

For a single mode field, $g^{(2)}(\tau)$ is independent of $\tau$ so
$$g^{(2)}(0)=\frac{{\langle \hat{a}^{\dagger{2}}\hat{a}^2 \rangle }}{\langle \hat{a}^{\dagger}\hat{a} \rangle ^2}=1+\frac{{\langle \Delta \hat{N}^2 \rangle -\langle \hat{N} \rangle }}{\langle \hat{N} \rangle ^2}\tag{18.1} .$$
The [p-representation](Quadrature%20Squeezing.md) for $g^{(2)}(0)$ is
$$g^{(2)}(0)=1+\frac{{\int d^2\alpha\;p(\alpha,\alpha ^{*})(|\alpha|^2-\langle \hat{a}^{\dagger}\hat{a} \rangle )^2}}{\langle \hat{a}^{\dagger}\hat{a} \rangle ^2}.\tag{18.2} $$
Hence $g^{(2)}(0)<1$ requires $P(\alpha,\alpha ^{*})<0$. 

Bunching or antibunching requires $g^{(2)}(\tau)$ to be independent of $\tau$, so a multimode field. The p-representation of $g^{(2)}(\tau)$ is
$$g^{(2)}(\tau)=1+\frac{{\int d^2\{ \alpha_{j} \}}\;p(\{ \alpha_{j},\alpha_{j}^{*} \})\sum_{k}(|\alpha_{k}|^2-\langle \hat{a}_{k}^{\dagger} \hat{a}_{k}\rangle ^2)}{\left( \sum_{k}\langle \hat{a}_{k}^{\dagger}\hat{a}_{k} \rangle  \right)^2}.\tag{18.3} $$
Hence $g^{(2)}(0)<1$ requires $p(\{ \alpha_{j},\alpha ^{*}_{j} \})<0$. 

The negative $p$ and $g^{(2)}(0)<1$ are non-classical results. The classical coherence function must fulfil $\gamma^{(2)}(0)\geq \gamma^{(2)}(\tau)$, hence $g^{(2)}(\tau)<g^{(2)}(\tau)$ is also non-classical. We expect $g^{(2)}(\tau)\to 1$ for $\tau\to \infty$ hence $g^{(2)}(\tau)<1$ typically implies antibunching.
![[Pasted image 20251121114110.png]]

The stationary $g^{(2)}(\tau)$ is given by 
$$g^{(2)}(\tau)=(1-e^{ -\gamma \tau/2 })^2,\;\Omega\ll\gamma \tag{18.4} $$
$$g^{(2)}(\tau)=1-e^{ -3\gamma \tau/4 }\cos(\Omega \tau),\;\Omega\gg\gamma.\tag{18.5} $$
The fluorescence photon results from the decay of a single atom from an excited to ground state. There is zero probability of a second photon if $\tau=0$, the atom must first be driven back to its excited state.