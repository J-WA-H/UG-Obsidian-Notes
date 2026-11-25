We can link bulk thermodynamic properties with the statistical partition function:
$$F=-Nk_{B}T\ln(Z)$$
$$Z=\sum_{j}e^{-\epsilon_{j}/k_{B}T}$$
$$U=-N \frac{\partial}{\partial \beta}(\ln(Z))$$
$$S=\frac{1}{T}(U-F)$$
Heat capacity is defined by 
$$C_{V}=\left( \frac{\partial U}{\partial T} \right)_{V}=-k_{B}T^2\left( \frac{\partial U}{\partial \beta} \right)_{V}.$$
These equations all link the microscopic quantity of the partition function with macroscopic thermodynamic properties.

Example (1D harmonic oscillator):
$$\epsilon_{n}=\left( n+\frac{1}{2} \right)\hbar \omega.$$
There are an infinite number of energy levels so
$$Z=\sum_{n=0}^\infty e^{-\beta \epsilon_{n}}=\sum_{n=0}^\infty e^{-\beta(n+1/2)\hbar \omega}=e^{-\beta \hbar \omega/2}\sum_{n=0}^\infty e^{-\beta \hbar \omega n}.$$This is a geometric sum of the form $\sum_{n=0}^\infty x^n=\frac{1}{1-x}$ so evaluating this sum gives
$$Z=\exp\left( -\frac{\beta\hbar\omega}{2} \right) \frac{1}{1-\exp({-\beta \hbar \omega})}.$$
To find an expression for free energy, we need $\ln(Z)$.
$$\ln(Z)=\ln\left( \frac{\exp\left( -\frac{1}{2}\beta \hbar \omega \right)}{1-\exp(-\beta \hbar \omega )} \right)=-\frac{1}{2}\beta \hbar \omega-\ln(1-\exp(-\beta \hbar \omega)).$$
This gives
$$F=-\frac{N}{\beta}\ln(Z)=\frac{N\hbar\omega}{2}+\frac{N}{\beta}\ln(1-\exp(-\beta \hbar \omega)).$$
$$U=-N \frac{\partial}{\partial \beta}(\ln(Z))=\frac{1}{2}N\hbar \omega-\frac{\hbar \omega}{1-\exp(-\beta \hbar \omega)}.$$
$$S=\frac{{U-F}}{T}=k_{B}\beta(U-F)=Nk_{B}\left[\frac{\beta\hbar\omega}{1-\exp(-\beta \hbar \omega)}-\ln(1-\exp(-\beta \hbar \omega)) \right]$$
$$C_{V}=-k_{B}^2\beta\left(\frac{\partial U}{\partial \beta}\right)_{V}=\frac{Nk_{B}(\beta \hbar \omega)^2\exp(\beta \hbar \omega)}{(\exp(\beta \hbar \omega)-1)^2}.$$
Plotting these results gives:
![[Pasted image 20241024160647.png]]
Example (3D infinite square well):
$$\epsilon_{n_{x},n_{y},n_{z}}=\frac{h^2}{8ma^2}(n_{x}^2+n_{y}^2+n_{z}^2).$$
$$Z=\sum_{n_{x},n_{y},n_{z}=1}^\infty \exp(-\beta(\epsilon_{n_x}+\epsilon_{n_y}+\epsilon_{n_{z}}))=\sum_{n_{x}=1}^\infty \exp(-\beta \epsilon_{n_{x}})\sum_{n_{y}=1}^\infty \exp(-\beta \epsilon_{n_{y}})\sum_{n_{z}=1}^\infty \exp(-\beta \epsilon_{n_{z}})$$
$$=\left( \sum_{n=1}^\infty \exp(-\beta \epsilon_{n}) \right)^3=\left( \sum_{n=1}^\infty \exp\left( -\frac{\beta h^2n^2}{8ma^2} \right) \right)^3.$$
Consider the high temperature limit as $T\to \infty$:
$$Z\approx\left( \int_{0}^\infty \exp\left( -\frac{\beta h^2n^2}{8ma^2} \right)dn \right)^3=\left( \frac{2\pi mk_{B}T}{h^2} \right)^{3/2}V$$
where $V=a^3$.
From this we can calculate the macroscopic thermodynamic properties.