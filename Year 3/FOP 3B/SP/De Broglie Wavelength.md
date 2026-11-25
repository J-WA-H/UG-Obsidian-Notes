We have the De Broglie wavelength
$$\lambda_{D}=\frac{h}{\sqrt{ 2\pi mk_{B}T }}.$$
This was derived from the [[Maxwell-Boltzmann Distribution]] so represents a classical quantity, but examining the interparticle spacing in a material, $\lambda$, then we have a classical-quantum crossover:
$$\text{If } \lambda >\lambda_{D}\text{ then classical (Dilute limit)}$$
$$\text{If } \lambda\leq \lambda_{D} \text{ then quantum}.$$
Example (particle speeds):
$$\frac{\hbar^2k^2}{2m}=\frac{1}{2}mv^2\implies k\propto v.$$
The average of some quantity $Q(v)$ in terms of speed is
$$\langle Q\rangle=\frac{\int v^{2}e^{-\beta mv^2/2}Q(v)dv}{\int v^{2}e^{-\beta mv^{2}/2}dv}$$
$v^{2}e^{-\beta mv^{2}/2}$ is the the Maxwell-Boltzmann distribution for speed i.e. the number of particles with speed in the range $v\to v+dv$.
Note that the number of particles is given by $N=\int n(v)dv$
$$n(v)dv\approx v^2e^{-\beta mv^2/2}=Cv^2e^{-\beta mv^2/2}$$then
$$C=4\pi N\left( \frac{\beta m}{2\pi} \right)^{3/2}.$$
![[Pasted image 20241115155324.png]]
The most likely velocity is given by the peak of this distribution
$$\frac{dn}{dv}=0=C 2ve^{-\beta mv^2/2}\left( 1-\frac{\beta mv^2}{2} \right).$$
$$v_{max}=\sqrt{ \frac{2}{\beta m} }\approx \frac{1.41}{\sqrt{ \beta m }}.$$
Mean speed
$$\langle v\rangle=\frac{\int v^2e^{-\beta mv^2/2}vdv}{\int v^2e^{-\beta mv^2/2}dv}.$$
Here $Q(v)=v$
$$=\frac{\sqrt{ 8 }}{\sqrt{ \pi\beta m }}=\frac{1.60}{\sqrt{ \beta m }}.$$
RMS speed:
$$\langle v_{rms}^2\rangle=\frac{\int v^2e^{-\beta mv^2/2}v^2dv}{\int v^2e^{-\beta mv^2/2}dv}=\frac{3}{\beta m}$$
$$\implies\langle v_{rms}\rangle=\sqrt{ \frac{3}{\beta m} }=\frac{1.75}{\sqrt{ \beta m }}.$$
$\langle \varepsilon\rangle=\frac{1}{2}mv_{rm}^2=\frac{3}{2\beta}=\frac{3}{2}k_{B}T$. Each degree of freedom contributes $\frac{1}{2}k_{B}T$ to the internal energy of the system.