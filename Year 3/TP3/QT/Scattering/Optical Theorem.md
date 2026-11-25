From [[Phase Shifts]] we have the scattering amplitude
$$f_{\ell}(k)=\frac{2\ell+1}{k}e^{i\delta_{\ell}(k)}\sin(\delta_{\ell}(k)).$$
The total scattering amplitude is
$$f(k,\theta,\phi)=\sum_{\ell=0}^{\infty}f_{\ell}(k)P_{\ell}(\cos \theta).$$
Consider forward scattering, where $\theta=\phi=0$, so $\cos \theta=1$ and we have normalised the Legendre polynomials so $P_{\ell}(1)=1$ so, using the expansion for $e^{i\delta_{\ell}}$, gives
$$f(k,0,0)=\sum_{\ell=0}^{\infty}f_{\ell}(k)=\sum_{\ell=0}^{\infty} \frac{2\ell+1}{k}(\cos\delta_{\ell}+i\sin\delta_{\ell})\sin\delta_{\ell}.$$
Take the imaginary part of this:
$$\mathrm{Im}[f(k,0,0)]=\sum_{\ell=0}^{\infty} \frac{2\ell+1}{k}\sin^2\delta_{\ell}.$$
Recall that $$\sigma=\sum_{\ell=0}^{\infty} \frac{4\pi}{k^2}(2\ell+1)\sin^2\delta_{\ell}.$$
This gives
$$\sigma=\frac{4\pi}{k}\mathrm{Im}[f(k,0,0)].$$
This is the optical theorem.