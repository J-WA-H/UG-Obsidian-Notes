With a charged scalar field $\phi$ and gauge field $A^{\mu}$, the [Lagrangian](Symmetry%20Breaking.md) is given by $(1.5)$,
$$\mathcal{L}=(\partial_{\mu}+ieA_{\mu})\bar{\phi}(\partial^{\mu}-ieA^{\mu})\phi-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}-\frac{1}{4}\lambda(|\phi|^2-\eta^2)^2. \tag{1.5} $$
The energy of a static vortex configuration in two dimensions is
$$\tag{10.1} E=\int d^2r\left[ |(\vec{\nabla}-ie\vec{A})\phi|^2+\frac{1}{2}(\vec{E}^2+\vec{B}^2)+V(|\phi|) \right].$$
As this integral must converge, there must be some restrictions. Far from the string core $|\phi|$ must be the VEV $\eta$ to minimise $V(\phi)$. The covariant derivative must also vanish at infinity which implies that the field must take the form of a pure gauge rotation
$$A_{\theta}\to \frac{1}{er} \frac{d\vartheta}{d\theta}+\dots,\;r\to \infty,\tag{10.2} $$
where $\mathscr{v}$ is the phase of $\phi$. This Higgs screening by the gauge fields prevents the logarithmic divergence of the [string](Cosmic%20Strings.md) in $(7.6)$. As the field must traverse a closed path, $\phi(2\pi)=\phi(0)$, so the winding number in the phase $\vartheta$ must be an integer,
$$\tag{10.3} n=\frac{1}{2\pi}\int_{0}^{2\pi} \frac{d\vartheta}{d\theta}d\theta=\frac{e}{2\pi}\oint \vec{A}\cdot d\vec{l}.$$
There is a non-zero winding $n$ if $\phi$ has a zero somewhere in the vortex core, $\phi(x)=0$, where $x$ is gauge-invariant. From stokes theorem, the vortex configuration has a quantised magnetic flux $\Phi_{B}=2\pi n/e$.

To work out the size and mass of a vortex, we need two characteristic scales - determined by the regions over which the scalar and gauge fields depart from their asymptotic values. These distance scales are related to the Higgs and particle masses off the string, $r_{s}$ and $r_{v}$. To an order of magnitude, the energy is
$$E\approx{2}\pi \eta^2\left[ \ln\left( \frac{r_{v}}{r_{s}} \right)+\frac{1}{e^2\eta^2r_{v}^2}+\lambda \eta^2r_{s}^2 \right].\tag{10.4} $$
The first term represents the gradient energy of the scalar field, the second is a consequence of magnetic pressure since the flux does not wish to be confined, and the last term is the potential energy cost of the departure of $|\phi|$ from the minimum at $|\phi|=\eta$. The energy expression is minimised by
$$\tag{10.5} \begin{matrix}
r_{s}\approx m_{s}^{-1}=(\sqrt{ \lambda }\eta)^{-1} \\
r_{v}\approx m_{v}^{-1}=(\sqrt{ 2 }e\eta)^{-1}.
\end{matrix}$$
These two string core widths correspond to the Compton wavelengths of the scalar and vector particles respectively. The values give the approximate mass of the vortex configuration
$$\tag{10.6} \mu \approx{2}\pi \eta^2\ln\left( \frac{m_{s}}{m_{v}} \right),$$which in three dimensions becomes the string mass per unit length.

The field equations for the abelian-Higgs model is given by the Euler-Lagrange equations,
$$(\partial_{\mu}-ieA_{\mu})(\partial^{\mu}-ieA^{\mu})\phi+\frac{\lambda}{2}\phi(\phi \bar{\phi}-\eta^2)=0\tag{10.7} $$
$$\partial_{\mu}F^{\mu \nu}=j^{\nu}\tag{10.8} $$
where
$$j^{\nu}\equiv 2e\mathrm{Im}[\bar{\phi}(\partial^{\nu}-ieA^{\nu})\phi].\tag{10.9} $$
The gauge chosen is the Lorenz gauge, $\partial_{\mu}A^{\mu}=0$. For convenience rescale $\phi\to \eta^{-1}\phi$, $A^{\mu}\to \eta^{-1}A^{\mu}$ and $x\to \eta x$. This makes all these quantities dimensionless so set $\eta=1$. Further rescaling $x\to ex$ shows the only significant parameter is the ratio between the Higgs and vector masses,
$$\tag{10.10} \beta=\frac{m_{s}^2}{m_{v}^2}=\frac{\lambda}{2e^2}.$$
The static cylindrically symmetric solutions for the scalar and gauge fields, $\phi_{s},\vec{A}_{s}$ is given by
$$\tag{10.11} \phi_{s}(\vec{r})=e^{ in\theta }f(r),$$
$$\tag{10.12} A_{s\;a}(\vec{r})=-\epsilon_{ab}x_{b} \frac{n}{er^2}\alpha(r)$$
where $a,b=1,2$. This gives $A_{s\;\theta}=-n\alpha(r)/er$, where $n$ is the vortex winding number. This ansatz for a straight string lying along the z-axis is only dependent on polar coordinates. The asymptotic boundary conditions are
$$
\lim_{ r \to \infty }f(r)=\lim_{ r \to \infty }  \alpha(r)=1\tag{10.13}
$$$$f(0)=\alpha(0)=0.$$
Substituting $(10.11-12)$ into the field equations give
$$\frac{d^2f}{dr^2}+\frac{1}{r} \frac{df}{dr}-\frac{n^2f}{r^2}(\alpha-1)^2-\frac{\lambda}{2}f(f^2-1)=0\tag{10.14} $$
$$\frac{d^2\alpha}{dr^2}-\frac{1}{r} \frac{d\alpha}{dr}-2e^2f^2(\alpha-1)=0.\tag{10.15} $$
Although analytic solutions are not known, but solutions can be approximated for large $r$. Assuming $|\phi|$ as a constant, then $(10.15)$ reduces to the modified Bessel equation with solutions
$$\alpha(r)\approx 1-rK_{1}(\sqrt{ 2 }er)\approx 1-\mathcal{O}(\sqrt{ r }\exp[-\sqrt{ 2 }er]).\tag{10.16} $$
The asymptotic form of $\phi$ depends on $\beta$. For $\beta>4$, the large distance fall of of $f$ is controlled by the gauge field contribution $\propto(1-\alpha)^2$. For $\beta\lesssim 4$, the gauge fields can be ignored as $r\to \infty$ and $(4.14)$ yields
$$f(r)\approx 1-K_{0}(\sqrt{ \lambda }r)\approx 1-\mathcal{O}(\exp[-\sqrt{ \lambda }r]).\tag{10.17} $$
Close to the vortex core, the leading order dependence for the Higgs field is $f(r) \sim r^{n}$, that is, we have an $n^{th}$ order zero of $\phi$. Full solutions for $f,\alpha$ are obtained numerically.

Critical coupling is the limit in which the Higgs and vector masses become identical, $\beta=1$. This limit in QFT can be extended to become supersymmetric. The field equations then reduce to a coupled first-order system. The vortex energy can be rewritten as
$$E=\int d^2x\left[ |[(\partial_{x}-iA_{x})\pm i(\partial_{y}-iA_{y})]\phi|^2+\frac{1}{2}[B_{z}\pm(\phi \bar{\phi}-1)^2] \right]\pm \int d^2xB_{z}+(\beta-1)\int d^2x(\phi \bar{\phi}-1)^2,\tag{10.18} $$
where $B_{z}=F_{12}=\partial_{x}A_{y}-\partial_{y}A_{x}$ and the upper sign is for $n\geq 0$ and the lower for $n<0$.
This integral is positive definite and the magnetic flux gives the lower bound $E\geq 2\pi |n|$. The critical coupling field equations become
$$\tag{10.19} \begin{matrix}
[(\partial_{x}-iA_{x})\pm i(\partial_{y}-iA_{y})]\phi=0, \\
B_{z}=\mp(\phi \bar{\phi}-1).
\end{matrix}$$
At critical coupling the solutions to these equations satisfy the general field equations. For cylindrically symmetric fields, $(10.11-12)$, the above equations reduce to
$$\begin{matrix}
\frac{df}{dr}=\frac{nf}{r}(1-\alpha), \\
\frac{1}{r} \frac{d\alpha}{dr}=\mp \frac{1}{n}[f^2-1].
\end{matrix}\tag{10.20} $$
For small $r$, the $n=1$ solutions take the form
$$\alpha(r)=-\frac{1}{n}\sum_{k=1}^{\infty}\beta_{k}\left( \frac{r}{\sqrt{ 2 }} \right)^{2k},\tag{10.21} $$
with the recursion relation 
$$\beta_{k}=\frac{1}{k(k-1)}\sum_{l=2}^{k-1}l\beta_{l}\beta_{k-l},\;\beta_{1}=-1,\;\beta_{2}\approx 0.7279\dots \tag{10.22} $$
The other solution is
$$\tag{10.23} f(r)\approx 1-Z_{1}\left[ \frac{\pi}{2}\sqrt{ 2 }r \right]^{1/2} e^{ -\sqrt{ 2 }r }+\mathcal{O}(e^{ -2\sqrt{ 2 }r })\approx \alpha(r)+\mathcal{O}(e^{ -2\sqrt{ 2 }r })$$
with $Z_{1}\approx 1.7079\dots$

There are many other solutions that appear in vortex dynamics and interactions.

The same process is done for the [Goldstone model](Symmetry%20Breaking.md) with no gauge fields, which gives the field equation in just $\phi$,
$$\tag{10.24} \partial_{\mu}\partial^{\mu}\phi+\frac{\lambda}{2}\phi(\phi \bar{\phi}-1)=0.$$
The cylindrically symmetric equation becomes
$$\frac{d^2f}{dr^2}+\frac{1}{r} \frac{df}{dr}-\frac{n^2}{r^2}f-\frac{\lambda}{2}f(f^2-1)=0. \tag{10.25} $$
There is no Higgs mechanism that breaks the global symmetry and the massless Goldstone boson introduces a long-range force. This causes the energy per unit length to be divergent. These are known as global $U(1)$ strings.