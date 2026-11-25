Using the [Green's function](Integral%20Equation%20for%20Scattering.md) the integral equation becomes
$$\psi_{k}(\underline{r})=\psi_{0}(\underline{r})+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')\psi_{k}(\underline{r}')d^3r'$$
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}-\frac{1}{4\pi}\int \frac{e^{ik|\underline{r}-\underline{r}'|}}{|\underline{r}-\underline{r}'|}U(\underline{r}')\psi_{k}(\underline{r}')d^3r'.$$
The potential is taken to have a finite extension $d$, so $U(\underline{r})$ is only important for $r<d$.
As $\underline{r}\to \infty$, consider $\underline{r}'\ll \underline{r}$.
$$|\underline{r}-\underline{r}'|^2=(\underline{r}-\underline{r}')\cdot(\underline{r}-\underline{r}')=\underline{r}\cdot \underline{r}-2\underline{r}\cdot \underline{r}'+\underline{r}'\cdot\underline{r}'=r^2\left( 1-\frac{2\underline{r}\cdot \underline{r}'}{r^2}+\cancelto{0}{\frac{r'^2}{r^2}} \right).$$
$$\therefore |\underline{r}-\underline{r}'| \approx r\left( 1-\frac{2\underline{r}\cdot \underline{r}'}{r^2} \right)^{1/2}\approx r-\frac{{\underline{r}\cdot \underline{r}'}}{r^2}.$$
$$\implies \frac{e^{ik|\underline{r}-\underline{r}'|}}{|\underline{r}-\underline{r}'|}\approx \frac{e^{ikr}e^{-ik\underline{r}\cdot \underline{r}'/r}}{r}.$$
Take $\underline{k}=k\underline{\hat{r}}=\frac{k\underline{r}}{r}$
$$\therefore \frac{e^{ik'|\underline{r}-\underline{r}'|}}{|\underline{r}-\underline{r}'|}\approx \frac{e^{ikr}e^{-i\underline{k}\cdot \underline{r}'}}{r}.$$
Recall the [[Scattering Amplitude]]
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\frac{e^{ikr}}{r}f(k,\theta,\phi)$$
so equating this with the integral formula gives
$$f(k,\theta,\phi)=-\frac{1}{4\pi}\int e^{-i\underline{k}'\cdot \underline{r}'}U(\underline{r}')\psi_{k}(\underline{r}')d^3r'.$$
$$f(k,\theta,\phi)=-\frac{1}{4\pi}\bra{\psi_{0_{k}}}U\ket{\psi_{k}}$$
This inner product is the transition matrix element
$$T_{k'k}=\bra{\psi_{0_{k}}}V\ket{\psi_{k}}=\frac{\hbar^2}{2m}\bra{\psi_{0_{k}}}U\ket{\psi_{k}}$$
so
$$f(k,\theta,\phi)=-\frac{2m}{\hbar^24\pi}T_{k'k}.$$
This gives a cross section of
$$\frac{d\sigma}{d\Omega}=\frac{m^2}{4\pi \hbar^4}|T_{k'k}|^2.$$
