Fermions are 1/2 integer spin particles that follow the [[Fermi-Dirac Distribution]].
$$f_{FD}(\varepsilon)=\frac{1}{e^{\beta(\varepsilon-\mu)}+1}.$$
Using the definition of a distribution function, $f_{j}=\frac{n_{j}}{g_{j}}$, we get the total number of particle in a system as
$$N=\int_{0}^{\infty }g(\varepsilon)f_{FD}(\varepsilon)d\varepsilon.$$
![[Pasted image 20241121123018.png]]
At $T=0\text{ K}$, the distribution function is a step function which for $T>0\text{ K}$ smears out around the Fermi energy.

Example: At $T=0\text{ K}$, calculate the Fermi-level of electrons in a cube of metal of size $a$:
$$N=\int_{0}^{\infty}g(\varepsilon)f_{FD}(\varepsilon)d\varepsilon$$
We know $f_{FD}(\varepsilon)$ is a step function and the [degeneracy](Counting%20Degenerate%20States.md) is
$$g(\varepsilon)d\varepsilon=\frac{V}{2\pi^2}\left( \frac{2m}{\hbar^2} \right)^{3/2}\varepsilon^{1/2}d\varepsilon=4\pi V\left( \frac{2m}{h^2} \right)^{3/2}\varepsilon^{1/2}d\varepsilon \times 2$$
where the $\times 2$ comes from the fact that each fermion has two possible spin states. This gives
$$N=8\pi V\left( \frac{2m}{h^2} \right)^{3/2}\int_{0}^{\mu}\varepsilon^{1/2}d\varepsilon$$
$$=\frac{16}{3}\pi V\left( \frac{2m}{h^2} \right)^{3/2}\mu^{3/2}$$
$$\implies \mu=\frac{h^2}{2m}\left( \frac{3N}{16\pi V} \right)^{2/3}.$$
Example: The same but for $T>0\text{ K}$.
$$N=4\pi V\left( \frac{2m}{h^2} \right)^{3/2}\int_{0}^{\infty} \frac{\varepsilon^{1/2}}{e^{\beta(\varepsilon-\mu)}+1}d\varepsilon.$$
This integral is difficult to solve but we could use the integral
$$\int_{0}^{\infty} \frac{x^{1/2}}{e^x+1}dx=\frac{1}{4}(2-\sqrt{ 2 })\sqrt{ 2 } \zeta\left( \frac{3}{2} \right),$$
where $\zeta(x)$ is the Riemann-Zeta function.

Example: Ultra high temperature Fermions (relativistic)
If we have high temperatures so high that $k_{B}T\gg mc^2$ then we are in the relativistic regime, like the early universe.
If they are so hot then we also have $k_{B}T\gg N$ (not in their ground state).
$$U=\sum_{J}\varepsilon_{j}g_{j}f_{j}\to ^{bulk} \int_{0}^{\infty}\varepsilon(k) \frac{4\pi k^2dk}{\left( \frac{\pi}{a} \right)^3}f_{FD}(k)$$
where
$$f_{FD}(k)=\frac{1}{e^{\beta\varepsilon(k)}+1}.$$
As we are at such high temperatures, the Fermi-energy is negligible.
In the relativistic regime
$$\varepsilon(k)=(p^2c^2+m_{0}^2c^4)^{1/2}$$
$$=(\hbar^2k^2c^2+m_{0}^2c^4)^{1/2}.$$
In this regime $\hbar kc\gg m_{0}c^2$ so $\varepsilon(k)\approx \hbar kc$. Letting $V=a^3$ we get
$$\frac{U}{V}=\frac{{\hbar c}}{2\pi^2}\int_{0}^{\infty} \frac{k^3}{e^{\beta \hbar kc}+1}dk.$$
Noting that
$$\int_{0}^{\infty} \frac{x^3}{e^x+1}dx=\frac{7\pi^4}{15}$$
so the energy density in the early universe is given by
$$\frac{U}{V}=\frac{\pi^2}{30} \frac{(k_{B}T)^4}{(\hbar c)^3}\cdot \frac{7}{8}$$
