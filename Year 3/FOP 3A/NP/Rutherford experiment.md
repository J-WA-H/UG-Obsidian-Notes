The Rutherford experiment shoots $\alpha$ particles at a thin, gold foil. This provides evidence for the nucleus of an atom as most particles don't [scatter](Scattering.md), showing most of the atom is empty space.
![[Pasted image 20241122093807.png]]
In this case the interaction Hamiltonian is
$$H_{int}=\frac{Z_{He}Z_{Au}e^2}{4\pi\varepsilon_{0}r}$$
which gives the matrix element
$$\mathcal{M}_{pp'}=\bra{\psi_{p'}}H_{int}\ket{\psi_{p}}$$
where $\psi_{p}$ are the eigenfunctions of the momentum operator
$$\psi_{p}(\underline{x})=\frac{1}{\sqrt{ V }}e^{i\underline{p}\cdot \underline{x}}.$$
Calculating the matrix element:
$$\mathcal{M}_{pp'}=\frac{Z_{He}Z_{Au}e^2}{4\pi\varepsilon_{0}} \int d^3x \frac{{e^{i(\underline{p}-\underline{p}')\cdot \underline{x}}}}{r} .$$
Setting $\underline{q}=\underline{p}-\underline{p}'$ gives
$$\mathcal{M}_{pp'}=\frac{Z_{He}Z_{Au}e^2}{4\pi\varepsilon_{0}}\int \frac{r^2dr}{r} e^{i\cos \theta_{x}r\lvert \underline{q} \rvert }\sin \theta_{x}d\theta_{x}d\phi_{x}.$$
Integrating over all space multiplies by $2\pi$ since there is no $\phi_x$ dependence.
Change of variables, $\eta=\cos \theta_{x}$, $d \eta=-\sin \theta_{x}d\theta_{x}$. This gives the limits of integration between $1$ and $-1$.
$$\mathcal{M}_{pp'}=\frac{Z_{He}Z_{Au}e^2}{2\varepsilon_{0}}\int_{0}^\infty \int_{-1}^1 drd\eta re^{i\eta rq}$$
$$=\frac{Z_{He}Z_{Au}}{2\varepsilon_{0}}\int_{0}^\infty dr\left[ \frac{1}{iq}(e^{irq}+e^{-irq}) \right]$$
$$=\frac{Z_{He}Z_{Au}e^2}{2\varepsilon_{0}\lvert \underline{q} \rvert^2 }\lim_{ r \to \infty } (1+e^{ir\lvert \underline{q} \rvert })$$
$$=\frac{Z_{He}Z_{Au}e^2}{\varepsilon_{0}q^2}$$
This gives a cross-sectional area of
$$\sigma=\int d\Omega \left\lvert  \frac{E_{p}}{2\pi}\mathcal{M}_{pp'}  \right\rvert ^2=\int d\Omega \left\lvert  \frac{m}{2\pi} \frac{Z_{Au}Z_{He}e^2}{\varepsilon_{0}q^2}  \right\rvert .$$
The transferred momentum, $\underline{q}=\underline{p}-\underline{p}'$ so $q^2=p^2+p'^2-2pp'\cos\theta=2p^2(1-\cos \theta).$
Using $\sin^2\left( \frac{\alpha}{2} \right)=\frac{1}{2}(1-\cos \alpha)$, we get
$$q^2=\left[ 2p \sin\left( \frac{\theta}{2} \right) \right]^2.$$
We can get a differential cross-section:
$$d\sigma=\frac{d\sigma}{d\Omega}d\Omega.$$
We get
$$\frac{d\sigma}{d\Omega}=\frac{\alpha^2Z_{Au}^2Z_{He}^2}{16E_{kin}^2\sin^4\left( \frac{\theta}{2} \right)}$$
where $E_{kin}=\frac{p^2}{2m}$.
$$dN_{scat}=\mathcal{L}\Delta t \frac{d\sigma}{d\Omega}d\Omega=\mathcal{L}\Delta t \frac{d\sigma}{d\Omega}\sin \theta d\theta d\phi=2\pi \mathcal{L}\Delta t \frac{d\sigma}{d\Omega}\sin \theta d\theta.$$
In practice $d\theta$ cannot be infinitesimal so instead we use a change in $\theta$, $\Delta \theta$. Using this we get the number of particles scatter in a range of angles $d\theta$ to be a histogram, that can be modelled with a continuous curve derived from the theory.
![[Pasted image 20241122184110.png]]