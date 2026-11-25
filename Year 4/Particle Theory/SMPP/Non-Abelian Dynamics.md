We aim to get Feynman rules for QCD. A gluon vertex
![[Pasted image 20260210110332.png]]
has the interaction Lagrangian
$$\mathcal{L}_{int}=g_{s}\bar{\psi}_{i}\gamma^\mu(T^a)_{ij}A_{\mu}^{\;a}\psi_{j}\tag{3.1} $$where $i,j$ are colour indices. This gives the vertex factor
$$-g_{s}\gamma^\mu(T^a)_{ij}\tag{3.2} $$
The gluon propagator in the [Feynman gauge](Photon%20Propagator.md) is
$$-\frac{ig_{\mu \nu}\delta^{ab}}{p^2+i\varepsilon}\tag{3.3}. $$
The quark propagator is
$$\frac{i(p\!\!\!/+m)}{p^2-m^2+i\varepsilon}\tag{3.4}. $$
For external spinors

| Incoming   | Spinor             | Outgoing   | Spinor             |
| ---------- | ------------------ | ---------- | ------------------ |
| quarks     | $u^i(p_{1})$       | quarks     | $\bar{u}^i(k_{1})$ |
| antiquarks | $\bar{v}^i(p_{2})$ | antiquarks | $v^i(k_{2})$       |
The product of spinors are
$$\sum_{spin}u_{\alpha}^{i}\bar{u}_{\beta}^j=p\!\!\!/_{\alpha\beta}\delta^{ij}\tag{3.5} $$
where $\alpha,\beta$ are spinor indices, which are normally suppressed.

For external gluons, incoming gluons have the polarisation vector $\varepsilon_{\mu}^{\;a}(k)$ and outgoing gluons have $\varepsilon_{\mu}^{\;a*}(k)$. These satisfy transversality and completeness
$$k^\mu\varepsilon_{\mu}^{\;a}(k)=0;\;\sum \varepsilon_{\mu}^{\;a}(k)\varepsilon_{\nu}^{\;a*}(k)=-g_{\mu \nu}.\tag{3.6}. $$
For scattering amplitudes, we will need
$$\mathrm{Tr}[T^aT^b]=\sum_{colour}(T^a)_{ij}(T^b)_{ji}=\frac{1}{2}\delta^{ab},\;(T^a)_{ij}(T^b)_{k\ell}=\frac{1}{2}\left( \delta_{i\ell}\delta_{jk}-\frac{1}{N_{c}}\delta_{ij}\delta_{k\ell} \right)\tag{3.7} $$where $N_{c}$ is the number of colours, which for QCD is 3.
$$(T^aT^b)_{ij}=C_{F}\delta_{ij}= \frac{{N_{c}^2-1}}{2N_{c}}\delta_{ij}\tag{3.8} $$
$$f^{acd}f^{bcd}=C_{A}\delta^{ab}=N_{c}\delta^{ab}\tag{3.9} $$
Consider the scattering process $q\bar{q}\to \bar{q}'q'$ where $q\neq q'$.
![[Pasted image 20260210113030.png]]
The matrix element is
$$\mathcal{M}=[\bar{v}^j(p_{2})(-ig_{s}\gamma^\mu T^a_{ij})u^i(p_{1})] \frac{{-ig_{\mu \nu}\delta^{ab}}}{\underbrace{ (p_{1}+p_{2})^2 }_{ s }}[\bar{u}^m(k_{1})(-ig_{s}\gamma^\nu T^b_{mn})v^n(k_{2})]=i \frac{g_{s}^2}{s}[\bar{v}(p_{2})\gamma^\mu T^au(p_{1})][\bar{u}(k_{1})\gamma_{\mu}T^av(k_{2})].\tag{3.10} $$
$$|\overline{\mathcal{M}}|^2=\frac{1}{4} \frac{1}{N_{c}^2}\sum_{s,c}|\mathcal{M}|^2\tag{3.11} .$$
$$\sum_{s}\bar{v}_{\alpha}(p_{2})\gamma^\mu_{\alpha\beta}T^au_{\beta}(p_{1})\bar{u}(p_{1})\gamma^\nu_{\gamma\delta}T^bv_{\delta}(p_{2})=\sum_{s}\bar{v}_{\alpha}(p_{2})[\gamma^\mu T^ap\!\!\!/_{1}\gamma^\nu T^b]_{\alpha\delta}v_{\delta}(p_{2})=[\gamma^\mu T^ap\!\!\!/_{1}\gamma^\nu T^b]p\!\!\!/_{2\delta\alpha}=\mathrm{Tr}[\gamma^\mu p\!\!\!/_{1}\gamma^\nu p\!\!\!/_{2}]T^aT^b.\tag{3.12} $$
Using $\mathrm{Tr}[a\!\!\!/\gamma^\mu b\!\!\!/\gamma^\nu]=4(a^\mu b^\nu+a^\nu b^\mu+g^{\mu \nu}(ab))$,
$$\sum_{s,c}|\mathcal{M}|^2=\frac{g_{s}^4}{s^2}\mathrm{Tr}[p\!\!\!/_{2}\gamma^\mu p\!\!\!/_{1}\gamma^\nu]\mathrm{Tr}[k\!\!\!/_{1}\gamma_{\mu}k\!\!\!/_{2}\gamma_{\nu}]\sum_{c}T^a_{ij}T^b{ij}T^a_{mn}T^b_{mn}\tag{3.13}=\frac{16g_{s}^{4}}{s^2}(t^2+u^2). $$
$$|\overline{M}|^2=\frac{1}{2} \frac{N_{c}^2-1}{N_{c}^2} \frac{g_{s}^4}{s^2}(t^2+u^2)=\frac{4}{9} \frac{g_{s}^4}{s^2}(t^2+u^2).\tag{3.14} $$
For multiple diagrams, consider $q\bar{q}\to gg$
![[Pasted image 20260210114843.png]]
