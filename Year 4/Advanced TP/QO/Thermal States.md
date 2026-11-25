A blackbody is a perfect emitter and absorber of radiation. Radiation is modelled in a cavity in thermal equilibrium with its walls. Radiation couples to a heat bath.

The probability for a system to be in its nth energy eigenstate $\ket{\psi_{n}}$ is
$$P_{n}(T)=\frac{e^{ -E_{n}/k_{B}T }}{\sum_{n'}e^{ -E_{n'}/k_{B}T }}\tag{6.1}. $$
In terms of [[Density Operators]],
$$P_{n}(T)=\mathrm{Tr}(\rho \ket{\psi_{n}} \bra{\psi_{n}} )\tag{6.2} $$where
$$\rho(T)=\frac{e^{ -\hat{H}/k_{B}T }}{\mathrm{Tr}(e^{ -\hat{H}/k_{B}T })}\tag{6.3}. $$Note that $\ket{\psi_{n}}\bra{\psi_{n}}$ is a projector - an operator observable with eigenvalues equal to 1 for $\ket{\psi_{n}}$ or otherwise $0$.

Define the partition function
$$Z(T)=\mathrm{Tr}(e^{ -\hat{H}/k_{B}T })\tag{6.4}. $$
We can then rewrite the density operator as
$$\rho(T)=\sum_{n}P_{n}(T)\ket{\psi_{n}} \bra{\psi_{n}}\tag{6.5}  $$
$$P_{n}(T)=\frac{e^{ -E_{n}/k_{B}T }}{Z(T)}\tag{6.6}. $$
For a single field mode, consider [Hamiltonian](Creation%20and%20Annihilation%20Operators.md) 
$$\hat{H}=\hbar \omega\left( \hat{a}^{\dagger}\hat{a}+\frac{1}{2} \right)\tag{6.7} $$with eigenvalues $$E_{n}=\hbar \omega\left( n+\frac{1}{2} \right).\tag{6.8} $$
This gives the density operator
$$\rho(T)=\frac{e^{ -\hbar \omega(\hat{a}^{\dagger}\hat{a}+1/2) /k_{B}T}}{Z(T)}\tag{6.9} $$with
$$Z(T)=e^{ -\hbar \omega/2k_{B}T }\sum_{n=0}^{\infty}e^{ -\hbar \omega n/k_{B}T }.\tag{6.10} $$This is a geometric series it can easily be evaluated to be
$$Z(T)=\frac{e^{ -\hbar \omega/2k_{B}T }}{1-e^{ -\hbar \omega/k_{B}T }}.\tag{6.11} $$
The mean photon number is given by
$$N(T)=\mathrm{Tr}(\rho(T)\hat{N})=\sum_{n=0}^{\infty}n\bra{n} \rho(T)\ket{n}\tag{6.12}  $$where the number operator is given by $\hat{N}=\hat{a}^{\dagger}\hat{a}$. In term from statistical mechanics,
$$N(T)=\frac{e^{ -\hbar \omega/2k_{B}T }}{Z(T)}\sum_{n=0}^{\infty}ne^{ -\hbar \omega n/k_{B}T }\tag{6.13} $$where the sum evaluates to
$$\sum_{n=0}^{\infty}ne^{ -\hbar \omega n/k_{B}T }=\frac{e^{ -\hbar \omega/k_{B}T }}{(1-e^{ -\hbar \omega/k_{B}T })^2}.\tag{6.14} $$
The photon number can be simplified in limiting cases,
$$N(T)=\frac{e^{ -\hbar \omega /k_{B}T}}{1-e^{ -\hbar \omega/k_{B}T }}=\frac{1}{e^{ \hbar \omega/k_{B}T }-1}.\tag{6.15} $$
For high temperature,
$$N(T)\to \frac{k_{B}T}{\hbar \omega}\tag{6.16} $$
and for low temperature
$$N(T)\to e^{ -\hbar \omega/k_{B}T }.\tag{6.17} $$$(6.15)$ can be inverted to give
$$e^{ -\hbar \omega/k_{B}T }=\frac{N}{1+N}\tag{6.18}. $$
This means $\rho$ can be written in terms of $N$,
$$\rho=\frac{1}{N+1}\sum_{n=0}^{\infty}\left( \frac{N}{1+N} \right)^{n}\ket{n} \bra{n}\tag{6.19} . $$
The probability to observe $n$ photons is
$$P_{n}=\frac{N^{n}}{(1+N)^{n+1}}.\tag{6.20} $$
To determine number fluctuations, similar to $N=\langle \hat{N} \rangle$, we can determine $\langle \hat{N}^2 \rangle=N+2N^2$. Number fluctuations are then given by the variance$$\langle \hat{N}^2 \rangle -\langle \hat{N} \rangle ^2=N+N^2\tag{6.21} .$$
The fluctuations $N+N^2$ are larger than the mean $N$. The RMS deviation is then $$\Delta N=\sqrt{ N+N^2 }\tag{6.22} ,$$tends for large $N$ to $\Delta N\approx N+\frac{1}{2}$. The relative uncertainty is then $\frac{\Delta N}{N}\approx 1$, which for small $N$ tends to $\frac{\Delta N}{N}\approx \frac{1}{\sqrt{ N }}$.

Planck's law involves multiplying the average energy due to the number of photons by the density of modes $\rho(\omega)$ per unit interval in $\omega$ in a unit volume.
We need a continuum limit of our cubical cavity model. Within a volume $V=L^3$ cubic space, total number of modes in k-space increment is
$$\Delta m=2\left( \frac{L}{2\pi} \right)^{3}\Delta k_{x}\Delta k_{y}\Delta k_{z}.\tag{6.23} $$
The continuum limit is then
$$dm=2\left( \frac{V}{8\pi^3} \right)dk_{x}dk_{y}dk_{z}\tag{6.24}. $$In spherical coordinates,
$$dm=2\left( \frac{V}{8\pi^3} \right)k^2dk\sin \theta d\theta d\phi.\tag{6.25} $$
Using $\omega=ck$,
$$dm=2\left( \frac{V}{8\pi^3c^3} \right)\omega^2d\omega \sin \theta d\theta d\phi.\tag{6.26} $$
Integrating over $\theta,\phi$ gives
$$V\left( \frac{\omega^2}{\pi^2c^3} \right)d\omega=V\rho(\omega)d\omega.\tag{6.27} $$
The average energy density per unit interval in $\omega$ is $U(\omega)=\hbar \omega N\rho(\omega)$. Hence
$$U(\omega)=\hbar \frac{\omega^3}{\pi^2c^2} \frac{1}{e^{ \hbar \omega/k_{B}T }-1}.\tag{6.28} $$
Rayleigh's law - In the high temperature limit,
$$U(\omega)\approx \frac{\omega^2k_{B}T}{\pi^2c^3}\tag{6.29} .$$
Wien's law - in the low temperature limit
$$U(\omega)\approx \frac{\hbar\omega^3k_{B}T}{\pi^2c^3}e^{ -\hbar \omega/k_{B}T }.\tag{6.30} $$
Wien's displacement law is given by differentiating $U(\omega)$ and find the extremum, there is a peak at
$$\omega=\frac{2\pi c}{\lambda}=\frac{2.9k_{B}T}{\hbar}\tag{6.31}. $$
Integrating $U(\omega)$ over all frequencies yields the average energy density. From Wien's law,
$$U\approx \hbar \frac{k_{B}T}{\pi^2c^3}\int d\omega \;\omega^3e^{ -\hbar \omega/k_{B}T }=\frac{\pi^2(k_{B}T)^4}{15c^3\hbar^3}\tag{6.32} .$$This is the Stefan-Boltzmann law, energy is proportional to $T^{4}$.
