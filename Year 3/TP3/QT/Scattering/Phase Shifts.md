Assume that $\lim_{ r \to \infty }rU(r)=0$ so $U(r)\approx 0$ for $r>d$ where $d$ is the range of the potential.

For $r\gg d$, solutions should be the [solutions](Special%20Functions.md) with $U(r)=0$, i.e.
$$R_{\ell}(k,r)=B_{\ell}(k)j_{\ell}(kr)+C_{\ell}(k)n_{\ell}(kr).$$
$B_{\ell}$ and $C_{\ell}$ can be complex but we will take them to be real.
$B_{\ell}=e^{i\alpha}b_{\ell}$, $C_{\ell}=e^{i\alpha}c_{\ell}$, which consist of a real parameter and a constant phase.

In practice, we can find $B_{\ell},C_{\ell}$ by matching to the exact solution at $r=d$.
For large $r$, 
$$R=\frac{e^{i\alpha}}{kr}\left[ b_{\ell}(k)\sin\left( kr-\ell \frac{\pi}{2} \right) -c_{\ell}(k)\cos\left( kr-\ell \frac{\pi}{2} \right)\right].$$
Define
$$A_{\ell}(k)=\sqrt{ b_{\ell}^2(k)+c^2_{\ell}(k) }$$
and
$$\tan\delta_{\ell}(k)=-\frac{c_{\ell}(k)}{b_{\ell}(k)}=\frac{\sin(\delta_{\ell})}{\cos(\delta_{\ell})}$$
so
$$R=\frac{A_{\ell}(k)e^{i\alpha}}{kr}\left[ \cos(\delta_{\ell})\sin\left( kr-\ell \frac{\pi}{2} \right)+\sin(\delta_{\ell})\cos\left( kr-\ell \frac{\pi}{2} \right) \right]$$
$$=\frac{A_{\ell}(k)e^{i\alpha}}{kr}\sin\left( kr-\ell \frac{\pi}{2}+\delta_{\ell}(k) \right).$$
This must be equal to
$$(2\ell+1)i^{\ell} \frac{\sin\left( kr-\ell \frac{\pi}{2} \right)}{kr}+f_{\ell}(k) \frac{e^{ikr}}{r}.$$
Write the sin as an exponential:
$$\frac{A_{\ell}(k)e^{i\alpha}}{2kri}[e^{ikr}e^{-i\ell \pi/2+i\delta_{\ell}}-e^{-ikr}e^{i\ell \pi/2-i\delta_{\ell}}]$$$$=\frac{1}{2ikr}[(2\ell+1)i^{\ell}e^{ikr}e^{-i\ell \pi/2}-(2\ell+1)i^{\ell}e^{-ikr}e^{i\ell \pi/2}+2ikf_{\ell}(k)e^{ikr}].$$
Equating $e^{-ikr}$ coefficients:
$$-\frac{A_{\ell}(k)e^{i\alpha}}{2kri}e^{i\ell \pi/2-i\delta_{\ell}}=-\frac{1}{2ikr}(2\ell+1)i^{\ell}e^{i\ell \pi/2}.$$
$$\implies A_{\ell}(k)e^{i\alpha}=(2\ell+1)i^{\ell}e^{i\delta_{\ell}}.$$
Equating $e^{ikr}$ coefficients:
$$\frac{A_{\ell}(k)e^{i\alpha}}{2kri}(e^{-i\ell \pi/2+i\delta_{\ell}})=\frac{1}{2ikr}[(2\ell+1)i^{\ell}e^{-i\ell \pi/2}+2ikf_{\ell}(k)]$$
$$(2\ell+1)i^{\ell}e^{i\delta_{\ell}}e^{-i\ell \pi/2+i\delta_{\ell}}=(2\ell+1)i^{\ell}e^{-i\ell \pi/2}+2ikf_{\ell}(k)$$
$$\implies f_{\ell}(k)2ik=(2\ell+1)i^{\ell}(e^{2i\delta_{\ell}-i\ell \pi/2}-e^{-i\ell \pi/2})=(2\ell+1)e^{i\delta_{\ell}}(e^{i\delta_{\ell}}-e^{-i\delta_{\ell}})$$
$$\implies f_{\ell}(k)=\frac{{2\ell+1}}{k}e^{i\delta_{\ell}}\sin(\delta_{\ell}).$$
So for the total [cross section](Method%20of%20Partial%20Waves.md) is
$$\sigma_{\ell}=\frac{4\pi}{2\ell+1}|f_{\ell}(k)|^2=\frac{4\pi}{k^2}(2\ell +1)\sin^2\delta_{\ell}.$$
From this we can see that phase shifts, determined by matching to the full solution, completely determines the cross-section.
There are very few cases where the phase shifts can be calculated analytically:
- No potential - solution has to be valid everywhere $\implies |\psi|$ is finite everywhere. At $r=0,n_{\ell}\to \infty\therefore B=0$ so we only use Bessel functions $\implies \delta_{\ell}=0$ so no scattering. 

At large $\ell$, $\frac{\ell(\ell+1)}{r^2}\gg U(r)$ so not all terms are equally important so we get approximately the free solution.
If the potential has range $a$, neglect $\ell>ka$.
At particularly low energies, $k\to 0$ so the s-wave scattering dominates.
For low energy scattering, define scattering length
$$l_{s}=-\lim_{ k \to 0 } \frac{\tan(\delta_{\ell})}{k}. $$
As $R\to 0$, $f_{0}\to l_{s}$, $$\frac{d\sigma}{d\Omega}\to l_{s}^2\implies\sigma=4\pi l_{s}^2.$$
