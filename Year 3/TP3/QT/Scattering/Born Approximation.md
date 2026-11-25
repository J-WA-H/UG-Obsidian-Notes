In general the [[Lippmann-Schwinger Equation]] is difficult to directly solve as $\psi_{k}$ appears on both sides. Consider
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')\psi_{k}(\underline{r}')d^3r'.$$
Substitute in the integral equation for $\psi_{k}(\underline{r}')$:
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')\left[ e^{i\underline{k}\cdot \underline{r}'}+\int G_{0}(k,\underline{r}'-\underline{r}'')U(\underline{r}'')\psi_{k}(\underline{r}'')d^3r'' \right]d^3r'.$$
Repeating this gives a series expansion in $U(\underline{r})$:
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')e^{i\underline{k}\cdot \underline{r}'}d^3r'+\dots$$
If $U$ is small we get a perturbative expansion, so we can keep only the first few terms, which is known as the Born approximation.

Only considering the first term is the first born approximation:
$$\psi_{k}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')e^{i\underline{k}\cdot \underline{r}'}d^3r'.$$
Using the large $r$ asymptotic form of the Green's function,
$$G_{0}(k,\underline{r}-\underline{r}')=-\frac{1}{4\pi} \frac{e^{ikr}}{r}e^{-i\underline{k}'\cdot \underline{r}'}$$$$\implies f(k,\theta,\phi)=-\frac{1}{4\pi}\int e^{-i\underline{k}'\cdot \underline{r}'}U(\underline{r}')e^{i\underline{k}\cdot \underline{r}'}d^3r'.$$
Take $\underline{\Delta}=\underline{k}-\underline{k}'$, this gives
$$f^{B}(k,\theta,\phi)=-\frac{1}{4\pi}\int e^{i\underline{\Delta}\cdot \underline{r}}U(\underline{r})d^3r.$$
This shows that the scattering amplitude is the [[Fourier Transform]] of the potential, with momentum transfer $\Delta \hbar$.

For elastic scattering, $|\underline{k}|=|\underline{k}'|$
$$\implies \underline{k}\cdot \underline{k}'=k^2\cos \theta$$
$$\Delta^2=(\underline{k}-\underline{k}')^2=2k^2-2k^2\cos \theta=2k^2(1-\cos \theta )=4k^2\sin^2 \frac{\theta}{2}$$
$$\implies \Delta=2k\sin \frac{\theta}{2}.$$
For a central potential,
$$f^{B}(k,\theta,\phi)=-\frac{1}{4\pi}\int_{0}^{\infty} drr^2U(r)\int_{0}^{2\pi}d\phi \int_{-1}^{1}e^{i\Delta r\cos \theta'}d\cos\theta'$$
$$=-\frac{1}{2}\int_{0}^{\infty}dr r^2U(r)\left[ \frac{e^{i\Delta \cos\theta'}}{i\Delta r} \right]_{-1}^{1}=-\frac{1}{\Delta}\int_{0}^{\infty}drr \frac{1}{2i}(e^{i\Delta r}-e^{-i\Delta r})=-\frac{1}{\Delta}\int_{0}^{\infty}drr\sin(\Delta r)U(r).$$
$$f^{B}(k,\theta,\phi)=-\frac{1}{\Delta}\int_{0}^{\infty}drr\sin(\Delta r)U(r).$$

