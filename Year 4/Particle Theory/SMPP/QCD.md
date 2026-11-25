The strong force is described by the $SU(3)_{c}$ group in [[The Standard Model]]. Consider muon production from the annihilation of an electron-positron pair,
![[Pasted image 20260225184032.png]]
We have
$$\frac{s}{M_{Z}^2}\sim \left( \frac{10\text{ GeV}}{90\text{ GeV}} \right)^2\sim 10^{-2}\tag{7.1} $$
so the process is mediated by a photon.

The matrix element of this process is
$$-i\mathcal{M}=ie\bar{v}_{e}\gamma^\mu u_{e} \frac{-ig_{\mu \nu}}{s}(-ieQ_{i})\bar{u}_{i}\gamma^{\nu}v_{i}\tag{7.2}. $$
To calculate the cross-section, we first need the flux
$$\frac{1}{2s}=\frac{1}{4\sqrt{ (p_{e^{+}}p_{e^{-}}) -m_{e}^4}}\approx \frac{1}{4(p_{e^+}p_{e^-})}=\frac{1}{4p_{e^+}^2}\tag{7.3} .$$
We now have the cross-section
$$\sigma=\frac{1}{2s}\int \frac{1}{4}\sum_{s_{e^+},s_{e^-}}\sum_{s_{\mu^-},s_{\mu^+}}|\mathcal{M}|\underbrace{  (2\pi)^4 \delta^{(4)}(p_{e^+}+p_{e^-}-p_{\mu^-}-p_{\mu^+}) \frac{d^3p_{\mu^+}d^3p_{\mu^-}}{(2\pi)^62|\vec{p}_{\mu^+}||\vec{p}_{\mu^-}|} }_{ d\Phi_{2} }\tag{7.4} .$$
The matrix element squared is
$$|\overline{\mathcal{M}}|^2=\frac{e^4}{s^2}[2(u^2+t^2)]Q_{\mu}^2\tag{7.5}. $$
The Mandelstam variables $u,t$ can be written in terms of $s$,
$$t=-\frac{s}{2}(1-\cos \theta),\qquad u=-\frac{s}{2}(1+\cos \theta)\tag{7.6}.$$
This gives
$$|\overline{\mathcal{M}}|^2=e^4Q_{\mu}^2(1+\cos \theta).$$
The phase space element is
$$d\Phi_{2}=(2\pi)^4\delta^{(3)}(|\vec{p}_{\mu^+}|+|\vec{p}_{\mu^-}|-\sqrt{ s }) \frac{d^3p_{\mu^-}}{(2\pi)^64|\vec{p}_{\mu^-}|^2}\tag{7.7} $$
the volume element is
$$d^3p_{\mu^-}=|\vec{p}_{\mu^-}|^2d|\vec{p}_{\mu^-}|d\Omega \tag{7.8}. $$
This gives
$$d\Phi_{2}=(2\pi)^4 \frac{1}{2}\delta^{(3)}\left( |\vec{p}_{\mu^-}|-\frac{\sqrt{ s }}{2} \right) \frac{d|\vec{p}_{\mu^-}|d\Omega}{(2\pi)^64}=\frac{1}{32\pi^2}d\Omega \tag{7.9}. $$
The differential cross-section is
$$d\sigma=\frac{1}{64\pi^2s}e^4Q_{\mu}^2(1+\cos\theta)d\Omega \tag{7.10}\implies\sigma=Q_{\mu}^2 \frac{e^4}{12\pi s} .$$
If this produces a $q\bar{q}$ pair instead of a $\mu^+\mu^-$ pair,
- $Q_{u}=\frac{2}{3}$, $Q_{d}=-\frac{1}{3}$
- Colour sum $\implies$ overall factor of $N_{c}=3$ for QCD

Quark hadron duality is described by the scattering process
![[Pasted image 20260225190818.png]]
For length scales $\frac{1}{\Lambda_{QCD}}\sim 1\text{ fm}$, we don't see quarks on there own.

We may calculate at parton level, and results agree with hadronic processes.

Define
$$R\equiv \frac{\sigma(e^+e^-\to\text{hadrons})}{\sigma(e^+e^-\to \mu^+\mu^-)}=3\sum_{i}Q_{i}^2\tag{7.11}. $$
![[Pasted image 20260225191635.png]]
From quarks, they can emit gluons,
![[Pasted image 20260225191728.png]]
The $R$ corrections are
$$R=\left( 3\sum_{i}Q_{i}^2 \right)\left( 1+\frac{g_{s}^2}{4\pi^2} \right)+\mathcal{O}(g_{s}^4)\tag{7.12}. $$
The strong coupling constant is
$$\alpha_{s}=\frac{g_{s}^2}{4\pi}\tag{7.13}. $$
If $\sqrt{ s }=34\text{ GeV}$ which gives $\alpha_{s}=0.135<\pi$.

In an experiment we might see a parton shower, consisting of many jets.
![[Pasted image 20260225192028.png]]
The radius of the jets gets smaller the large momentum.