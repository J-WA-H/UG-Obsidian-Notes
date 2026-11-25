To determine the [[Feynman Propagator]] for photons, it obeys the equation of motion
$$(\partial_{\sigma}\partial^\sigma g_{\mu \nu}-(1-\alpha)\partial_{\mu}\partial_{\nu})G^{\rho \nu}_{0}=i\delta^{(4)}(\vec{x}-\vec{y})g_{\mu}^{\;\rho}.\tag{6.1} $$
Taking the Fourier transform of this gives
$$(k^2g_{\mu \nu}-(1-\alpha)k_{\mu}k_{\nu})\tilde{G}_{0}^{\rho \nu}(k^2)=-ig_{\mu}^{\;\rho}.\tag{6.2} $$
Using the Feynman gauge where $\alpha=1$, the solution becomes
$$k^2g_{\mu \nu}\tilde{G}^{\rho \nu}_{0}(k^2)=k^2\tilde{G}_{0\mu}^{\;\rho}(k^2)\tag{6.3} $$
$$\tag{6.4} \implies \tilde{G}_{0\mu}^{\;\rho}(k^2)=-\frac{i}{k^2}g_{\mu}^{\;\rho}.$$
The full form of the propagator is
$$D^{\mu \nu}(k^2)=-i \frac{{g^{\mu \nu}-\frac{1-\alpha}{\alpha} \frac{k^\mu k^\nu}{k^2}}}{k^2+i\varepsilon}.\tag{6.5} $$
In the Feynman gauge, this becomes
$$D^{\mu \nu}(k^2)=-i {\frac{g^{\mu \nu}}{k^2+i\varepsilon}}\tag{6.6} $$which in real space yields
$$D^{\mu \nu}(x,y)=-ig^{\mu \nu} \int \frac{d^4k}{(2\pi)^4} \frac{e^{ -ik(x-y) }}{k^2+i\varepsilon}\tag{6.7} .$$
