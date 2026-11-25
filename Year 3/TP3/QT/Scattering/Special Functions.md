We are aiming to solve the [[Potential Scattering]] Schrodinger equation,
$$[\nabla^2+k^2-u(\underline{r})]\psi_{k}(\underline{r})=0.$$
We will try to solve this for a central potential, where $U(\underline{r})=U(r)$, there is no angular dependence.

In spherical coordinates,
$$\nabla^2=\frac{1}{r^2} \frac{\partial}{\partial r}\left( r^2 \frac{\partial}{\partial r} \right)+\frac{1}{r^2\sin \theta} \frac{\partial}{\partial \theta}\left( \sin \theta  \frac{\partial}{\partial \theta} \right)+\frac{1}{r^2\sin^2\theta} \frac{\partial^2}{\partial \phi^2}$$
$$=\frac{1}{r^2} \frac{\partial}{\partial r}\left( r^2 \frac{\partial}{\partial r} \right)-\frac{\hat{L}^2}{\hbar^2r^2}$$
where $\hat{L}^2$ is the total angular momentum operator.
Take the wavefunction
$$\Psi(\underline{r})=\sum_{\ell=0}^{\infty}\sum_{m=-\ell}^{\ell}c_{k\ell m}\psi_{k\ell m}(r,\theta,\phi)$$
where $\psi_{k\ell m}(r,\theta,\phi)=R_{k\ell}(r)Y_{\ell m}(\theta,\phi)$.
Substituting this into the Laplacian gives
$$\frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{dR_{k\ell}}{dr} \right)Y_{\ell m}(\theta,\phi)-R_{kl}(r) \frac{\hat{L}^2Y_{\ell m}}{\hbar^2r^2}=\left[ \frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{d}{dr} \right)-\frac{\ell(\ell+1)}{r^2} \right]R_{k\ell}(r)Y_{\ell m}(\theta,\phi).$$
$$\therefore \left[ \frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{d}{dr} \right)-\frac{\ell(\ell+1)}{r^2}-U(\underline{r})+k^2 \right]R_{k\ell}(r)Y_{\ell m}(\theta,\phi)=0.$$
We know the solutions for $Y_{\ell m}(\theta,\phi)$ so we just need to find $R_{k\ell}(r)$.
We expect
$$\lim_{ r \to \infty } \psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+f(k,\theta,\phi) \frac{e^{ikr}}{r}.$$
It is hard to find analytical solutions for the [[Scattering Amplitude]] $f(k,\theta,\phi)$ so it is normally found numerically.

To simplify the problem set $U(\underline{r})=0$.
For the simplest case, $\ell=0$.
Parametrise $u_{k\ell}(r)=rR_{k\ell}(r)$.
$$\therefore \frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{d}{dr}\left( \frac{u_{k\ell}}{r} \right) \right)=\frac{1}{r^2} \frac{d}{dr}\left[ r^2 \left( \frac{1}{r} \frac{du_{k\ell}}{dr}-\frac{u_{k\ell}}{r^2} \right) \right]$$
$$=\frac{1}{r^2} \frac{d}{dr}\left( r \frac{du_{k\ell}}{dr}-u_{k\ell} \right)=\frac{1}{r^2}\left( r \frac{d^2u_{k\ell}}{dr^2}+\frac{du_{k\ell}}{dr}-\frac{du_{k\ell}}{dr} \right)=\frac{1}{r} \frac{d^2u_{k\ell}}{dr^2}$$
so
$$\left( \frac{d^2}{dr^2}+k^2 \right)u_{k\ell}(r)=0.$$
This is a simple harmonic oscillator so
$$u_{k\ell}(r)=A\sin(kr)+Bcos(kr)$$
$$\implies R_{k\ell}(r)=\frac{A}{r}\sin(kr)+\frac{B}{r}\cos(kr).$$
As the wavefunction needs to be finite at the origin, set $B=0$.

This suggests it may be useful to use the substitution $\rho=kr$.
This gives for the general case
$$\left( \frac{d^2}{d\rho^2}+\frac{2}{\rho} \frac{d}{d\rho}-\frac{\ell(\ell+1)}{\rho^2}+1 \right)R_{\ell}(\rho)=0.$$
This is the Spherical Bessel equation.
This gives for $\ell=0$, 
$$R_{0}(\rho)=\frac{Ak\sin \rho}{\rho}+\frac{Bk\cos \rho}{\rho}.$$
From this we can ansatz
$$R_{\ell}(\rho)=\rho^{\ell}\chi_{\ell}(\rho).$$
$$\frac{dR_{\ell}}{d\rho}=\ell \rho^{\ell-1}\chi_{\ell}(\rho)+\ell \rho^{\ell-1} \frac{d\chi_{\ell}}{d\rho}.$$
$$\frac{d^2R_{\ell}}{d\rho^2}=\ell(\ell-1)\rho^{\ell-2}\chi_{\ell}(\rho)+\ell \rho^{\ell-1} \frac{d\chi_{\ell}}{d\rho}+\ell \rho^{\ell-1} \frac{d\chi_{\ell}}{d\rho}+\rho^{\ell} \frac{d^2\chi_{\ell}}{d\rho^{2}}.$$
The Bessel equation becomes:
$$\rho^{\ell-2}\ell(\ell-1)\chi_{\ell}(\rho)+2\rho^{\ell-1} \frac{d\chi_{\ell}}{d\rho}+\rho^{\ell} \frac{d^2\chi_{\ell}}{d\rho^2}+\frac{2}{\rho}\left( \ell \rho^{\ell-1}\chi_{\ell}(\rho)+\rho^{\ell} \frac{d\chi_{\ell}}{d\rho} \right)-\frac{\ell(\ell+1)}{\rho^2}\rho^{\ell}\chi_{\ell}(\rho)+\rho^{\ell}\chi_{\ell}(\rho).$$
$$\implies \left[ \rho^{\ell} \frac{d^{2}\chi_{\ell}}{d\rho^2}+2\rho^{\ell-1} \frac{d\chi_{\ell}}{d\rho}(\ell+1)+(\cancel{\ell(\ell-1)\rho^{\ell-2}}+\cancel{2\ell \rho^{\ell-2}}-\cancel{\ell(\ell+1)\rho^{\ell-2}}+\rho^{\ell})\chi_{\ell}(\rho) \right].$$
$$\implies \rho^{\ell}\left( \frac{d^2}{d\rho^2}+\frac{2}{\rho}(\ell+1) \frac{d}{d\rho}+1 \right)\chi_{\ell}(\rho)=0.$$
We will assume
$$\chi(\rho)=\frac{1}{\rho} \frac{d\chi_{\ell}}{d\rho}.$$
So differentiating the above ODE gives
$$\frac{d}{d\rho}\left[\left( \frac{d^2}{d\rho^2}+\frac{2}{\rho}(\ell+1) \frac{d}{d\rho}+1 \right)\chi_{\ell}(\rho)\right]=0$$
$$\implies \frac{d^3\chi_{\ell}}{d\rho^3}+\frac{2}{\rho}(\ell+1) \frac{d^2\chi_{\ell}}{d\rho^2}-\frac{2}{\rho^2}(\ell+1) \frac{d\chi_{\ell}}{d\rho}+ \frac{d\chi_{\ell}}{d\rho}=0.$$
$$\frac{d}{d\rho}\left( \frac{d\chi_{\ell}}{d\rho} \right)=\frac{d}{d\rho}(\rho \chi)=\rho  \frac{d\chi}{d\rho}+\chi$$
$$=\rho  \frac{d^2\chi}{d\rho^2}+2 \frac{d\chi}{d\rho}.$$
$$\implies \left( \frac{d^2}{d\rho^2}+2 \frac{d}{d\rho}+\frac{2(\ell+1)}{\rho} \left(\frac{d}{d\rho}+\frac{1}{\rho}\right)-\frac{2(\ell+1)}{\rho^2}+ 1 \right)\rho \chi=0$$
$$\implies \rho\left( \frac{d^2}{d\rho^2}+\frac{2(\ell+2)}{\rho} \frac{d}{d\rho}+\cancel{\frac{2(\ell+1)}{\rho^2}}-\cancel{\frac{2(\ell+1)}{\rho^2}}+1 \right)\chi(\rho)=0.$$
$$\rho\left( \frac{d^2}{d\rho^2}+\frac{2(\ell+2)}{\rho} \frac{d}{d\rho}+1 \right)\chi(\rho)=0.$$
This is the Bessel equation for $\ell+1$.
$$\therefore \chi_{\ell+1}(\rho)=\frac{1}{\rho} \frac{d\chi_{\ell}}{d\rho}.$$
This gives
$$\chi_{\ell}(\rho)=\left( \frac{1}{\rho} \frac{d}{d\rho} \right)^{\ell}\chi_{0}(\rho).$$
This gives:
$$j_{\ell}(\rho)=(-1)^{\ell}\rho^{\ell}\left( \frac{1}{\rho} \frac{d}{d\rho} \right)^{\ell} \frac{{\sin \rho}}{\rho}.$$
These are the spherical Bessel functions of the first kind.
$$n_{\ell}(\rho)=(-1)^{\ell}\rho^{\ell}\left( \frac{1}{\rho} \frac{d}{d\rho} \right)^{\ell} \frac{{\cos \rho}}{\rho}.$$
These are the Neumann functions (spherical Bessel functions of the second kind).
