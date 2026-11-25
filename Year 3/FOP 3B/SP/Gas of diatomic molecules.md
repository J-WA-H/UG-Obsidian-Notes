Consider a diatomic molecule - two particles connected by a spring-like bond.
![[Pasted image 20241120175820.png]]
The four main sources of energy in this system are translational, rotational, vibrational, and electronic.

The total [[Partition Function]] of this system is given by
$$Z=\sum_{\text{all states}}\exp[-\beta(E_{elec}+E_{vib}+E_{rot}+E_{cn})].$$
Using laws of exponentials this can be broken down into the product four separate partition functions
$$Z=Z_{elec}Z_{vib}Z_{rot}Z_{cm}.$$
This assumes each contribution to the energy is independent of each other.
For N indistinguishable molecules, this [partition function](Partition%20Function%20In%20Classical%20and%20Quantum.md) becomes
$$Z_{N}=\frac{Z^N}{N!}=\frac{(Z_{elec})^N(Z_{vib})^N(Z_{rot})^N(Z_{cm})^N}{N!}.$$
Electronic contribution:
For electrons with given energy levels, $E_{i}$, the partition function is given by
$$Z_{elec}=e^{-\beta E_{0}}+e^{\beta E_{1}}+e^{-\beta E_{2}}+\dots$$
$$=e^{-\beta E_{0}}(1+e^{-\beta(E_{1}-E_{0})}+e^{-\beta(E_{2}-E_{0})}+\dots).$$
Given that it takes tens of thousands of Kelvin to excite an electron from the ground state to excited state, the only term that makes any contribution to the partition function is the ground state, which is a constant.

For temperatures less than a few thousand kelvin, the electronic contribution is straight forward, i.e. $0$.

Vibrational contribution:
We can find the vibrational contribution from the harmonic oscillator.
$$\varepsilon_{n}=\left( n+\frac{1}{2} \right)\hbar \omega$$
We have already calculated the partition function for the [1D harmonic oscillator](Link%20Between%20Statistical%20and%20Thermodynamics.md) to be
$$Z_{vib}=\frac{\exp\left( -\beta \hbar \frac{\omega}{2} \right)}{1-\exp(-\beta \hbar \omega)}$$$$\implies U_{vib}=\frac{{N\hbar \omega}}{2}+\frac{{N\hbar \omega}}{e^{-\beta \hbar \omega}-1}.$$
$$C_{V}^{vib}=\frac{\partial U}{\partial T}=\frac{{Nk_{B}(\hbar \omega \beta)^2e^{\beta \hbar \omega}}}{(e^{\beta \hbar \omega}-1)^2}.$$
![[Pasted image 20241120184638.png]]
For a typical $O_{2}$ molecule in its first state, they vibrate at around $62\text{ THz}$, which gives a temperature of $T_{vib}=5000\text{ K}$. For all normal purposes, taking a low temperature limit would be a good approximation.
At low $T$, we can ignore states above the first excited state so
$$Z_{vib}\approx e^{-\beta \hbar \omega/2}[1+e^{-\beta \hbar \omega}].$$
This gives
$$\ln(Z_{vib})=-\frac{{\beta \hbar \omega}}{2}+\ln(1+e^{-\beta})$$hence
$$U_{vib}=\frac{{N\hbar \omega}}{2}+\frac{{N\hbar \omega e^{-\beta \hbar \omega}}}{1-e^{-\beta \hbar \omega}}.$$
We can see the far right term is of the form $\frac{x}{1-x}\approx x$ for small $x$ which gives
$$U_{vib}\approx \frac{{N\hbar \omega}}{2}+N\hbar \omega e^{-\beta \hbar \omega}$$
$$C_{V}^{vib}=N\hbar^2\omega^2\beta^2e^{-\beta \hbar \omega}.$$
For the high temperature limit:
$$Z_{vib}=e^{-\beta \hbar \omega/2}\sum_{n=0}^{\infty}e^{-\beta \hbar \omega n}\approx e^{-\beta \hbar \omega/2}\int_{0}^{\infty}e^{-\beta \hbar \omega n}dn.$$
We can approximate the sum as an integral as we are dealing with a large number of energy levels so if we call $dn=1$, which as $n\to \infty$, $dn$ is essentially infinitesimal.

Evaluating this integral gives
$$Z_{vib}=\frac{e^{-\beta \hbar \omega/2}}{\beta \hbar \omega}.$$
As we have this fairly simple form of the partition function, we gain simple results for $U$ and $C_V$.
$$U_{vib}=\frac{{N\hbar \omega}}{2}+Nk_{B}T$$
$$C_{V}^{vib}=Nk_{B}.$$
Rotational contribution:
Similarly for vibrations, rotations of a diatomic molecule are also quantised. They have angular momentum $L^2=l(l+1)\hbar^2$.

If a diatomic molecule has a moment of inertia $I$ then
$$E=\frac{L^2}{2I}=\frac{l(l+1)\hbar^2}{2I}.$$
This gives a partition function:
$$Z_{rot}=\sum_{l=0}^{\infty}g(E_{l})e^{-\beta E_{l}}=\sum_{l=0}^{\infty}(2l+1)\exp\left[ -\frac{\beta l(l+1)\hbar^2}{2I} \right].$$
For the general case we have to deal with the sum, which has no closed form.

Consider the high temperature limit:
$$Z_{rot}=\int_{0}^{\infty}dl(2l+1)\exp\left[ -\frac{\beta l(l+1)\hbar^2}{2I} \right]=\ln(2I)-\ln(\beta \hbar^2)$$
so $U_{rot}=\frac{N}{\beta}Nk_{B}T$, $C_{V}^{vib}=Nk_{B}$.

At the low temperature limit:
$$Z_{rot}=1+3e^{-\beta \hbar^2/I}$$
which gives 
$$U_{rot}=\frac{3N\hbar^2}{I}e^{-\beta \hbar^2/I};\;C_{V}^{rot}=Nk_{B}.$$
We now have low and high temperature contributions to each of $U$, $C_{V}$.
![[Pasted image 20241120192459.png]]
