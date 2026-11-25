The Feynman propagator is defined as
$$G_{F}(x-y)\equiv \bra{0} T(\hat{\phi}(x)\hat{\phi}(y))\ket{0}.\tag{6.1}  $$
This is a two-point correlation function where the 2 fields are time ordered. The time ordered product is defined as
$$T(\hat{\phi}(x)\hat{\phi}(y))=\begin{cases}
\hat{\phi}(x)\hat{\phi}(y) & x_{0}>y_{0} \\
\hat{\phi}(y)\hat{\phi}(x) & y_{0}>x_{0}
\end{cases}.\tag{6.2} $$
$$\therefore G_{F}(x-y)=\bra{0} T(\hat{\phi}(x)\hat{\phi}(y))\ket{0}=\begin{cases}
\bra{0} \hat{\phi}(x)\phi(y)\ket{0}\equiv D(x-y) &  x^{0}>y^{0} \\
\bra{0} \hat{\phi}(y)\hat{\phi}(x)\ket{0} \equiv D(y-x) & y^{0}>x^{0}
\end{cases}.\tag{6.4} $$
These expressions can be expressed as integrals
$$D(x-y)=\int \frac{d^3k}{(2\pi)^32E_{k}} \int \frac{d^3k'}{(2\pi)^32E_{k'}}\bra{0} \hat{a}(k)\hat{a}^{\dagger}(k')\ket{0}e^{ -ik_{\mu}x^{\mu}+ik'_{\mu}x^{\mu}}.\tag{6.5}  $$
Using the commutator for the [creation and annihilation operators](Quantisation%20of%20Fields.md), $\hat{a}(k)\hat{a}^{\dagger}(k')=[\hat{a},\hat{a}^{\dagger}]+\hat{a}^{\dagger}\hat{a}$. As $\bra{0}\hat{a}^{\dagger}=0=\hat{a}\ket{0}$, only the commutator survives, leaving a delta function which simplifies $(6.5)$ to
$$D(x-y)=\int \frac{d^3k}{(2\pi)^32E_{k}}e^{ -ik_{\mu}x^{\mu} }.\tag{6.6} $$
We can rewrite this in a Lorentz covariant way,
$$G_{F}(x-y)=\int \frac{d^4p}{(2\pi)^4} \frac{i}{p_{\mu}p^{\mu}-m^2}e^{ -ip_{\mu}(x-y)^{\mu} }.\tag{6.7} $$
Proof: Separate the time and space components,
$$\int d^4p=\int dp_{0}\int d^3p.\tag{6.8} $$
This integral has a singularity at $p_{0}=\pm E_{p}=\pm \sqrt{ |\vec{p}|^2+m^2 }$. This can be solved using a contour integral using Feynman prescription. First assume $x^{0}>y^{0}$. Figure out which plane to integrate in by setting $p_{0}=i|R|$,
$$e^{ -ip_{0}(x^{0}-y^{0}) }=e^{ R(x^{0}-y^{0}) }\to 0\implies R\to -\infty \tag{6.9} $$
so integrate in the lower half plane.
![[Pasted image 20251028170135.png]]
In this contour the only pole enclosed is at $+E_{p}$ so using [[Residue Theorem]] gives
$$G_{F}(x-y)=-2\pi i\int \frac{d^3p}{(2\pi)^4} \frac{i}{2E_{p}}e^{ -ip_{\mu}(x-y)^{\mu} }=\int \frac{d^3p}{(2\pi)^32E_{p}}e^{ -ip_{\mu}(x-y)^{\mu} }\equiv D(x-y)\;\square.\tag{6.10} $$
This same process can be repeated for $y^{0}>x^{0}$. Instead the contour integrates over the upper half plane.
![[Pasted image 20251028170828.png]]
Again using residue theorem gives $G_{F}(x-y)\equiv D(y-x)$ $\square$.

This proves the result of $(6.7)$. 

The contour can be simplified by rewriting the integral as
$$G_{F}(x-y)=\int \frac{d^4p}{(2\pi)^4} \frac{i}{p_{\mu}p^{\mu}-m^2+i\varepsilon}e^{ -ip_{\mu}(x-y)^{\mu} }\tag{6.11} $$where $\varepsilon$ is small and positive, which shifts the poles to $p_{0}=-E_{p}+i\varepsilon,E_{p}-i\varepsilon$, so there is no need to deform the contour.
![[Pasted image 20251028171430.png]]

The Lorentz invariant form of $G_{F}(x-y)$ is a Fourier transform so we can get the propagator in momentum space
$$\tilde{G}_{F}(p)=\frac{i}{p_{\mu}p^{\mu}-m^2+i\varepsilon}.\tag{6.12} $$
Consider applying the [Klein-Gordon](Classical%20Field%20Theory.md) equation to the propagator. This gives
$$(\partial_{\mu}\partial^{\mu}+m^2)G_{F}(x-y)=-i\delta^{(4)}(x-y)\tag{6.13} $$
which shows the Feynman propagator is a Greens function of the Klein-Gordon equation.