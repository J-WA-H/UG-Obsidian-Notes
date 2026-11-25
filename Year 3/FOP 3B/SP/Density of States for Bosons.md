From [degeneracy](Counting%20Degenerate%20States.md) we had $g(\varepsilon)\propto \sqrt{ \varepsilon }\implies g(0)=0$ which loses the lowest energy state. We need to modify the density of states for discrete states so they can describe bosons. This is done by adding a delta function
$$g(\varepsilon)\propto \sqrt{ \varepsilon }+\delta(0).$$
This delta function allows the lowest energy state to be occupied without affecting any other state.

Another difference between [[Fermions]] and [[Bosons]] are the distribution function. The [[Bose-Einstein Distribution]], given by
$$f_{BE}(\varepsilon)=\frac{1}{e^{\beta(\varepsilon-\mu)}-1},$$
appear so be negative for $\varepsilon<\mu$, however, given the fractional occupancy must be a positive quantity, this implies the fermi-energy must be $\mu=0$.

Consider the total number of particles
$$N=\int_{0}^{\delta E}\delta(\varepsilon)f_{BE}(\varepsilon)d\varepsilon+\int_{0}^{\infty}g(\varepsilon)f_{BE}(\varepsilon)d\varepsilon.$$
The first integral is the number of particles in the ground state, $n_{gs}(T)$, known as a condensate.
The second integral is the total number of particles in the excited state, $n_{es}(T)$.
Evaluating the integrals gives
$$N=f_{BE}(0)+\frac{2\pi V}{h^3}(2m)^{3/2}\int_{0}^{\infty} \frac{\sqrt{ \varepsilon }}{e^{\beta\varepsilon}-1}d\varepsilon$$
$$=\frac{1}{e^{-\beta \mu}-1}+\frac{2\pi V}{h^3}(2m)^{3/2}\int \frac{\sqrt{ \varepsilon }}{e^{\beta\varepsilon}-1}d\varepsilon.$$
At a certain temperature, around the first excitation value, the bosons will move from an excited state down into a ground state.
Examine the normal term as the ground state term does not take a nice form as $\mu\to 0$:
$$n_{es}(T)=\frac{2\pi V}{h^3}(2m)^{3/2}\int_{0}^{\infty} \frac{\sqrt{ \varepsilon }}{e^{\beta\varepsilon}-1}d\varepsilon \approx{2}.612 \frac{V}{h^3}(2\pi mk_{B})^{3/2}T^{3/2}.$$
$$n_{es}(T)\propto T^{3/2}.$$
Set the constants to $1/T_{B}^{3/2}$.

We can use this to calculate the ground state term
$$\frac{n_{gs}}{N}=\frac{{N-n_{es}}}{N}=1-\frac{n_{es}(T)}{N}.$$
This gets
$$n_{gs}(T)=N\left( 1-\left( \frac{T}{T_{B}} \right) \right)^{3/2}.$$
![[Pasted image 20241204162241.png]]
This yields an internal energy
$$U(T)=\int_{0}^{\infty}\varepsilon\delta(\varepsilon)f_{BE}(\varepsilon)d\varepsilon+\int_{0}^{\infty}\varepsilon g(\varepsilon)f_{BE}(\varepsilon)d\varepsilon$$
$$=\frac{2\pi V}{h^3}(2m)^{3/2}\int_{0}^{\infty} \frac{\varepsilon \sqrt{ \varepsilon }}{e^{\beta\varepsilon}-1}d\varepsilon.$$
Using the integral
$$\int_{0}^{\infty} \frac{x^{3/2}}{e^{x}-1}dx\approx 1.783.$$
This gives $U(T)\propto T^{5/2}$.