From electrodynamics the [potential](Fields%20from%20Continuous%20Distributions.md) is given by
$$V(\underline{r})=\int \frac{Ze^2}{|\underline{s}|}\rho(\underline{r}')d\underline{r}'$$
where $\underline{s}=\underline{r}-\underline{r}'$, $Z$ is the nuclear charge and $e$ is the charge of a positron.
The charge distribution $\rho(\underline{r}')$ is defined such that
$$\int \rho(\underline{r}')d\underline{r}'=1$$
as for a [point charge](Nucleon%20Shapes.md) $\rho(\underline{r}')=\delta(\underline{r}')$.

This can be used to find the scattering amplitude using the [[Born Approximation]],
$$f(k,\theta)=-\frac{m}{2\pi \hbar^2}\int e^{i\Delta \cdot \underline{r}}V(\underline{r})d\underline{r}=-\frac{m}{2\pi \hbar^2}\int e^{i\underline{\Delta}\cdot \underline{r}}\int  \frac{Ze^2}{|\underline{s}|}\rho(\underline{r}')d\underline{r}'d\underline{r}.$$change variables to $\underline{s}=\underline{r}-\underline{r}'$,
$$f(k,\theta)=-\frac{m}{2\pi \hbar^2}Ze^2\int e^{i\underline{\Delta}\cdot(\underline{s}+\underline{r}')}\int \frac{1}{|\underline{s}|}\rho(\underline{r}')d\underline{r}'d\underline{s}$$
$$=-\frac{mZe^2}{2\pi \hbar^2}\int e^{i\underline{\Delta}\cdot \underline{r}'}\rho(\underline{r}')d\underline{r}'\int \frac{e^{i\underline{\Delta}\cdot \underline{s}}}{|\underline{s}|}d\underline{s}.$$
The first integral is the [[Fourier Transform]] of the charge distribution,
$$\tilde{\rho}(\underline{k}-\underline{k}')=\int e^{i\underline{\Delta}\cdot \underline{r}'}\rho(\underline{r}')d\underline{r}'.$$
This is known as the form factor.
$$\therefore f(k,\theta)=-\frac{mZe^2}{2\pi \hbar^2}\tilde{\rho}(\underline{k}-\underline{k}')\int \frac{e^{i\underline{\Delta}\cdot \underline{r}}}{s}d\underline{s}.$$
The constants and the integral give the [Rutherford scattering amplitude](Rutherford%20experiment.md) so the total scattering amplitude is the product of the form factor and Rutherford's scattering amplitude.
$$f(k,\theta)=\tilde{\rho}(\underline{k}-\underline{k}')f_{Ruth}$$
$$\implies \frac{d\sigma}{d\Omega}=|\tilde{\rho}(\underline{k}-\underline{k}')|^2 \left( \frac{d\sigma}{d\Omega} \right)_{Ruth}.$$
The Fourier transform of the charge distribution can be obtained by measuring the cross-section.