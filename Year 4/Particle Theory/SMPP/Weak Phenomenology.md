Consider scattering with a heavy/unstable mediator, e.g. $e^+e^-\to Z\to \mu^+\mu^-$
![[Pasted image 20260221141939.png]]
This is an $s$-channel diagram, so
$$-i\mathcal{M}\propto \frac{1}{s-M_{z}^2+i\varepsilon}\tag{6.1}. $$
As $s\to(90 \text{ GeV})^2$, we get resonance,
![[Pasted image 20260221142230.png]]
Replace $M_{Z}$ with $M_{Z}-\frac{i}{2} \Gamma_{Z}$. This gives the wavefunction
$$\psi(t)\propto e^{ i(M_{Z}-i\Gamma_{Z}/2)t }\implies P\propto e^{ -\Gamma_{Z}t }\tag{6.2}. $$
This is the Breit-Wigner distribution. This gives the differential cross-section
$$d\sigma \propto \frac{1}{\left\lvert s-M_{Z}^2+\frac{i}{2}\Gamma_{Z}M_{Z}-\frac{\Gamma_{Z}^2}{4}\right\rvert^2}\tag{6.3} =\frac{1}{\left( s-M_{Z}^2-\frac{\Gamma_{Z}^2}{4} \right)^2+\Gamma_{Z}^2M_{Z}^2}$$
In the narrow-width approximation,
$$\sigma_{NW}=\frac{3}{4} \frac{4\pi}{\frac{M_{Z}^2}{4}} \frac{\Gamma(Z\to e^+e^-)\Gamma(Z\to \mu^+\mu^-)}{(s-M_{Z})+M_{Z}^2\Gamma_{Z}^2}=\frac{12\pi}{M_{Z}^2} \frac{\Gamma(Z\to e^+e^-)\Gamma(Z\to \mu^+\mu^-)}{(s-M_{Z}^2)+M_{Z}^2\Gamma_{Z}^2}\tag{6.4}.$$
Consider the interaction $e^+e^-\to Z\to \nu \bar{\nu}$. The interaction Lagrangian comes from the [Yukawa terms](The%20Standard%20Model.md),
$$\mathcal{L}^{Z\to \nu \bar{\nu}}_{int}=i\ell_{L}\gamma^\mu \mathcal{D}_{\mu}\ell_{L} \supset i\bar{v} \frac{igZ_{\mu}}{c_{w}}\gamma^\mu  \frac{(\sigma_{3})_{11}}{2}P_{L}v\tag{6.5} $$
as the neutrino is the first component of the lepton doublet. This shows the Z-boson only couples to left-handed neutrinos. This gives the matrix element
$$i\mathcal{M}_{Z\to \nu \bar{\nu}}=\varepsilon^\mu \bar{u}_{\nu} \frac{-ig}{2c_{w}}\gamma_{\mu}P_{L}v_{\nu}\tag{9.6}. $$
We have 3 spin polarisations for $Z$ so we want
$$\frac{1}{3}\sum_{\lambda}\sum_{s_{\nu},s_{\bar{\nu}}}|\mathcal{M}|^2=\frac{1}{3} \frac{g^2}{4c_{w}^2}\sum_{\lambda}\sum_{s_{\nu},s_{\bar{\nu}}}\varepsilon_{\mu}\varepsilon_{\rho}^{*}\bar{u}\gamma^\mu P_{L}v\bar{v}P_{L}^{*}(\gamma^\rho)^{\dagger}(\gamma^0)^{\dagger}u\tag{9.7} $$
as $(\gamma^\rho)^{\dagger}=\gamma^0\gamma^\mu \gamma^0$, $P_{L}\gamma_{\mu}=\gamma_{\mu}P_{R}$. We get
$$|\overline{\mathcal{M}}|^2=\frac{1}{3} \frac{g^2}{4c_{w}^2}\left( \frac{P_{Z}^\mu P_{Z}^\rho}{M_{Z}^2}-\eta^{\mu \rho} \right)\mathrm{Tr}[\gamma_{\mu}P_{L}p\!\!\!/_{\bar{\nu}}\gamma_{\rho}P_{L}p\!\!\!/_{\nu}]\tag{9.8} .$$
Evaluating the trace gives
$$\gamma_{\mu}P_{L}p\!\!\!/_{\bar{\nu}}\gamma_{\rho}P_{L}p\!\!\!/_{\nu}=\gamma_{\mu}p\!\!\!/_{\bar{\nu}}P_{R}\gamma_{\rho}P_{L}p\!\!\!/_{\nu}=\gamma_{\mu}p\!\!\!/_{\bar{\nu}}\gamma_{\rho}P_{L}^2p\!\!\!/_{\nu}=\gamma_{\mu}p\!\!\!/_{\bar{\nu}}\gamma_{\rho}P_{L}p\!\!\!/_{\nu}=\gamma_{\mu}p\!\!\!/_{\bar{\nu}}\gamma_{\rho}p\!\!\!/_{\nu}P_{R}\tag{9.9} $$
$$\mathrm{Tr}[\gamma_{\mu}\gamma_{\alpha}\gamma_{\rho}\gamma_{\beta}P_{R}]=2(\eta^{\mu\alpha}\eta^{\rho \beta}+\eta^{\rho \mu}\eta^{\alpha\beta}+i\epsilon^{\mu\alpha \rho\beta})\tag{9.10}. $$
This gives
$$|\overline{\mathcal{M}}|^2=\frac{g^2}{6c_{w}^2}\left( \frac{1}{M_{Z}^2}(2(p_{Z}p_{\bar{\nu}})(p_{Z}p_{\nu})-p_{Z}^2p_{\nu}p_{\bar{\nu}})-2p_{\bar{\nu}}p_{\nu}+4p_{\bar{\nu}}p_{\nu} \right)=\frac{g^2}{6c_{w}^2}\left( 2 \frac{(p_{Z}p_{\bar{\nu}})(p_{Z}p_{\nu})}{M_{Z}^2}+p_{\nu}p_{\bar{\nu}} \right)\tag{9.11}. $$
In the centre of mass frame, $p_{\nu}p_{\bar{\nu}}=|\vec{p}_{\nu}||\vec{p}_{\bar{\nu}}|-\vec{p}_{\nu}\cdot \vec{p}_{\bar{\nu}}=2|\vec{p}_{\nu}|^2=\frac{M_{Z}^2}{2}$ and $p_{\nu}p_{Z}=M_{Z}|\vec{p}_{\nu}|=\frac{M_{Z}^2}{2}$.

The phase space is
$$\int \frac{d^3p_{\nu}d^3p_{\bar{\nu}}}{(2\pi)^62|\vec{p}_{\nu}|2|\vec{p}_{\bar{\nu}}|}(2\pi)^4\delta^{(4)}(p_{Z}-p_{\nu}-p_{\bar{\nu}})=\int \frac{d^3p_{\nu}}{(2\pi)^24|\vec{p}_{\nu}||\vec{p}|}\delta(M_{Z}-|\vec{p}_{\nu}|-|\vec{p}_{\bar{\nu}}|)\tag{9.12} =\int \frac{d^2\Omega}{4(2\pi)^2}d|\vec{p}_{\nu}|\delta(M_{Z}-2|\vec{p}_{\nu}|)=\int \frac{d^2\Omega}{8(2\pi)^2}$$
$$\implies\Gamma_{Z\to \nu \bar{\nu}}=\frac{1}{2M_{Z}}\cdot(\text{phase space})\cdot |\overline{\mathcal{M}}|^2=\frac{g^2}{96\pi c_{w}^2}M_{Z}N_{\nu}.\tag{9.13} $$
Z bosons can be used to produce W bosons,
![[Pasted image 20260225182723.png]]
This requires $\sqrt{ s }>2M_{W}$.

The standard model predicts
$$\frac{M_{W}^2}{M_{Z}^2}=\cos^2\theta_{w}\tag{9.14} $$
and experiments give
$$\frac{M_{W}^2}{c_{w}M_{Z}^2}=1.0010\pm 0.0050\tag{9.15}. $$
