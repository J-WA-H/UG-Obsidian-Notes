Now aim to find solutions for the [[Scattering Amplitude]].

We have the asymptotic solution
$$\psi_{k}=e^{i\underline{k}\cdot \underline{r}}+f(k,\theta,\phi) \frac{e^{ikr}}{r}.$$
If we start with an azimuthally symmetric state then we end with an azimuthally symmetric state.

As Legendre polynomials span the space. we can write a general function
$$G(\theta,\phi)=\sum_{\ell=0}^{\infty}\sum_{m=\ell}^{\ell}G_{\ell m}Y_{\ell m}(\theta, \phi)$$
or if azimuthally symmetric
$$G(\theta)=\sum_{\ell=0}^\infty G_{\ell}P_{\ell}(\cos \theta).$$
This means we can write the scattering amplitude as
$$f(k,\theta,\phi)=\sum_{\ell=0}^{\infty}f_{\ell}(k)P_{\ell}(\cos \theta).$$
Each term is known as a partial wave, and $f_\ell(k)$ is the partial wave amplitude.

We can use this to rewrite the differential cross-section
$$\frac{d\sigma}{d\Omega}=|f(k,\theta,\phi)|^2=\sum_{\ell=0}^{\infty}f_{\ell}(k)P_{\ell}(\cos \theta)\sum_{\ell'=0}^{\infty}f_{\ell'}(k)P_{\ell'}(\cos \theta).$$
The total cross section is
$$\sigma=\int \frac{d\sigma}{d\Omega}d\Omega=2\pi \int_{-1}^{1}d\cos \theta  \frac{d\sigma}{d\Omega}$$
$$=2\pi \int_{-1}^{1}d\cos \theta \sum_{\ell,\ell'}P_{\ell}(\cos \theta)P_{\ell'}(\cos \theta)f_{\ell}(k)f_{\ell'}(k).$$
As the Legendre polynomials are orthogonal,
$$\int_{-1}^{1}dxP_{\ell}(x)P_{\ell'}(x)=\frac{2}{2\ell+1}\delta_{\ell \ell'}$$
$$\therefore \sigma=\sum_{\ell=0}^{\infty} \frac{4\pi}{2\ell+1}|f_{\ell}(k)|^2.$$
Let 
$$\sigma=\sum_{\ell=0}^{\infty} \sigma_{\ell}$$
where $\sigma_{\ell}$ is the partial wave cross section, given by
$$\sigma_{\ell}=\frac{4\pi}{2\ell+1}|f_{\ell}(k)|^{2}.$$
This gives
$$\psi_{k}(r)=\sum_{\ell=0}^{\infty}R_{\ell}(r)P_{\ell}(\cos \theta)\to ^{r\to \infty} e^{i\underline{k}\cdot \underline{r}}+f(k,\theta,\phi) \frac{e^{ikr}}{r}.$$
At large $r$, from [Rayleigh's formula](Properties%20of%20Bessel%20Functions.md),
$$\psi_{k}(r)=\sum_{\ell=0}^{\infty}\left[ (2\ell+1)i^{\ell}j_{\ell}(kr)+f_{\ell}(k) \frac{e^{ikr}}{r} \right]P_{\ell}(\cos \theta)$$
$$\implies \lim_{ r \to \infty } R_{\ell}=(2\ell+1)i^{\ell}j_{\ell}(kr)+f_{\ell}(k) \frac{e^{ikr}}{r}.$$
