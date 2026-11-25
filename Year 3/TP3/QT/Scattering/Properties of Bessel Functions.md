The [Bessel functions](Special%20Functions.md) are damped oscillators which decrease as $r$ increases.
$$\lim_{ r \to 0 }j_{\ell}(\rho)= \frac{2^{\ell}\ell!}{(2\ell+1)!}\rho^{\ell} $$
$$\lim_{ r \to 0 } n_{\ell}(\rho)=\frac{{-(2\ell)!}}{2^{\ell}\ell!}\rho^{-(\ell+1)} $$
$$\lim_{ r \to \infty } j_{\ell}(\rho)=\frac{1}{\rho}\sin\left( \rho-\ell \frac{\pi}{2} \right)$$
$$\lim_{ r \to \infty } n_{\ell}(\rho)=\frac{1}{\rho}\cos\left( \rho-\ell \frac{\pi}{2} \right).$$
Summary:
$$\left( \frac{d^2}{dr^2}+\frac{2}{r} \frac{d}{dr}-\frac{\ell(\ell+1)}{r^2}+k^2 \right)R_{k\ell}(r)=0$$
has solutions
$$R_{k\ell}(r)=Aj_{\ell}(kr)+Bn_{\ell}(kr).$$
This gives the full solution
$$\psi_{k}(\underline{r})=\sum_{\ell,m}c_{k\ell m}[A_{\ell}j_{\ell}(kr)+B_{\ell}n_{\ell}(kr)]Y_{\ell m}(\theta,\phi).$$
If the solution is azimuthally symmetric then the spherical harmonics go to the Legendre polynomials.
$$\psi_{k}(\underline{r})=\sum_{\ell=0}^{\infty}[A_{\ell}j_{\ell}(kr)+B_{\ell}n_{\ell}(kr)]P_{\ell}(\cos \theta).$$
Rayleigh's formula states
$$e^{ikz}=e^{ikr\cos \theta}=\sum_{\ell=0}^{\infty}(2\ell+!)i^{\ell}j_{\ell}(kr)P_{\ell}(\cos \theta).$$
