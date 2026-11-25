Jellium is a simple model of a uniform electron gas where the positive charge that attracts and binds the electrons is smeared out in jelly. For high density $\rho(\vec{r})$ it is a good approximation for simple metals like Na.

Recall that for a free electron in a box with periodic boundary conditions, the single particle wavefunctions are plane waves
$$\phi_{k}(\vec{r})=\frac{i\vec{k}\cdot \vec{r}}{\sqrt{ V }}\tag{6.1} .$$
The many body wavefunction is
$$\Phi(\vec{r}_{1},\sigma_{1};\vec{r}_{2},:\sigma_{2};,\dots)=\frac{1}{\sqrt{ N }}\det[\phi_{\vec{k}_{1}}^\uparrow,\phi_{\vec{k}_{1}}^\downarrow;\phi_{\vec{k}_{2}}^\uparrow,\phi_{\vec{k}_{2}}^\downarrow;\dots;\phi_{\vec{k}N/2}^\uparrow,\phi_{\vec{k}N/2}^\downarrow].\tag{6.2} $$
The spin density is hence given by
$$\rho^\uparrow(\vec{r})=\sum_{\vec{k}}^{k\leq k_{F}}|\phi_{\vec{k}}(\vec{r})|^2=\frac{1}{V}\left( \sum_{\vec{k}}^{k\leq k_{F}}1 \right)=\frac{N}{2V}\tag{6.3}. $$
This gives the total density $\rho(\vec{r})=2\rho^\uparrow(\vec{r})=\frac{N}{V}$. In the limit where $V\to 0$,
$$\sum_{\vec{k}}^{k\leq k_{F}}\to \frac{V}{8\pi^3}\int_{k\leq k_{F}} d^3k\tag{6.4}. $$
The elementary volume in $k$ space is $d^3k=\frac{8\pi^{3}}{V}$. This can be used to calculate the Fermi wavevector,
$$\sum_{\vec{k}}^{k\leq k_{F}}1=\frac{N}{2}\implies \frac{V}{8\pi^{3}}\int_{k\leq k_{F}}d^{3}k=\frac{V}{8\pi^{3}} \frac{4\pi k_{F}^{3}}{3}=\frac{N}{2}\implies k_{F}^3=3\pi^2 \frac{N}{V}=3\pi^2\rho \tag{6.5} $$
which gives $k_{F}=(3\pi^2\rho)^{1/3}$.

A useful quantity to characterise $\rho$ of a material is $r_{s}$, the radius of a small sphere that contains 1 electron,
$$\rho=\frac{1}{\frac{4}{3}\pi r_{s}^3}\implies r_{s}^3=\frac{3}{4\pi \rho}\implies r_{s}=\left( \frac{3}{4\pi \rho} \right)^{1/3}.\tag{6.6} $$
For metals $r_{s}$ is between $1$ and $6$ in a.u. (Bohr radius).
The relation between $k_{F}$, $r_{s}$ is
$$k_{F}^3r_{s}^3=\frac{9\pi}4 \implies k_{F}=\left( \frac{9\pi}{4} \right)^{1/3} \frac{1}{r_{s}} \simeq \frac{1.91916}{r_{s}}\tag{6.7}. $$
The kinetic energy of free electrons is given by
$$-\frac{\nabla^2}{2}\phi_{k}(\vec{r})=\varepsilon_{k}\phi_{k}(\vec{r})=\frac{k^2}{2}\phi_{k}(\vec{r}).\tag{6.8} $$
For $N$ electrons, 
$$E_{kin}=2\sum_{\vec{k}}^{k\leq k_{F}} \frac{k^2}{2}=\sum_{\vec{k}}^{k\leq k_{F}}\to \frac{V}{8\pi^3}\int_{k\leq k_{F}}d^3k\,k^2=\frac{V}{8\pi^3}4\pi \int_{0}^{k_{F}}k^4dk=\frac{V}{2\pi^2} \frac{k_{F}^5}{5}=\frac{3V}{10}\rho k_{F}^2=\frac{3Nk_{F}^2}{10}.\tag{6.9} $$
This gives the kinetic energy per electron
$$\varepsilon_{kin}=\frac{3}{10}k_{F}^2=\frac{3}{10}\left( \frac{1.91916}{r_{s}} \right)^{2}\simeq \frac{1.105}{r_{s}}\tag{6.10}. $$
The atomic units of energy is 1 Hartree $=27.2\text{ eV}=2\times 13.6\text{ eV}=2\text{ Ry}$
$$\implies\varepsilon_{kin}=\frac{2.21}{r_{s}}\tag{6.11} $$
Plane waves are orthogonal and complete,
$$\braket{ \phi_{\vec{k}} | \phi_{\vec{q}} } =\delta_{\vec{q},\vec{k}}\to \frac{1}{V}\int d^3r\,e^{ i(\vec{k}-\vec{q})\cdot \vec{r} }\tag{6.12} $$
$$\sum_{\vec{k}}\phi_{\vec{k}}(\vec{r})\phi_{\vec{k}}^{*}(\vec{r}')=\delta^{(3)}(\vec{r}-\vec{r}')\implies \frac{1}{V}\sum_{\vec{k}}e^{ i\vec{k}(\vec{r}-\vec{r}') }\tag{6.13} .$$
We can expand $\frac{1}{|\vec{r}|}$ in terms of plane waves,
$$\frac{1}{|\vec{r}|}=\frac{1}{V}\sum_{\vec{p}} \frac{4\pi}{p^2}e^{ i\vec{p}\cdot \vec{r} }\tag{6.14} .$$
This uses the Fourier transform $\mathcal{F}\left[ \frac{1}{r} \right]=\frac{4\pi}{k^2}$.
$$\therefore \frac{1}{|\vec{r}-\vec{r}'|}=\frac{1}{V}\sum_{\vec{p}} \frac{4\pi}{p^2}e^{ i\vec{p}\cdot(\vec{r}-\vec{r}') }\tag{6.15}. $$
This can give the [Hartree-Fock equations](Hartree-Fock%20Approximation.md) for jellium. First consider the Hartree term,
$$V_{H}[\rho](\vec{r})=\int d^3r' \frac{\rho(\vec{r}')}{|\vec{r}-\vec{r}'|}=\frac{N}{V}\int d^3r' \frac{1}{|\vec{r}-\vec{r}'|}\tag{6.16}. $$
This uses the density of homogeneous positive charge, $\rho_{+}=\frac{N}{V}$, but it diverges. The external potential is
$$V_{ext}(\vec{r})=-\int d^3r' \frac{\rho_{+}(\vec{r}')}{|\vec{r}-\vec{r}'|}=-\frac{N}{V}\int \frac{d^3r'}{|\vec{r}-\vec{r}'|}\tag{6.17} .$$This cancels out the divergence from the Hartree term so the only term left is the Fock term.
$$\hat{V}_{X}[\rho^\sigma]\phi_{k}(\vec{r})=- \int d^3r' \frac{\rho^\sigma(\vec{r},\vec{r}')\phi_{k}^\sigma(\vec{r}')}{|\vec{r}-\vec{r}'|}\tag{6.18} $$
Using
$$\rho^\sigma(\vec{r},\vec{r}')=\sum_{\vec{q}}^{q\leq k_{F}}\phi_{q}(\vec{r})\phi_{q}^{*}(\vec{r}')=\frac{1}{V}\sum_{\vec{q}}^{q\leq k_{F}}e^{ i\vec{q}\cdot(\vec{r}-\vec{r}') }\tag{6.19} $$
and $(6.15)$ gives
$$\hat{V}_{X}[\rho^\sigma]\phi_{k}^\sigma(\vec{r})=-\int d^3r' \frac{1}{V}\sum_{\vec{q}}^{q\leq k_{F}}e^{ i\vec{q}\cdot(\vec{r}-\vec{r}') } \frac{1}{V}\sum_{\vec{p}} \frac{4\pi}{p^2}e^{ i\vec{p}\cdot(\vec{r}-\vec{r}') } \frac{e^{ i\vec{k}\cdot \vec{r}' }}{\sqrt{ V }}.\tag{6.20} $$
$$=-\frac{1}{V^{5/2}}\sum_{\vec{q}}^{q\leq k_{F}}\sum_{\vec{p}} \frac{4\pi}{p^2}e^{ i(\vec{q}+\vec{p})\cdot \vec{r} }\underbrace{\int d^3r' e^{ i(\vec{k}-\vec{q}-\vec{p})\cdot \vec{r}' }}_{V\delta_{\vec{k}-\vec{q},\vec{p}}}=\underbrace{-\frac{1}{V}\sum_{\vec{q}}^{q\leq k_{F}} \frac{4\pi}{|\vec{k}-\vec{q}|^2}}_{\lambda_{\vec{k}}} \frac{e^{ i\vec{k}\cdot \vec{r} }}{\sqrt{ V }}\tag{6.21} .$$
This gives an eigenvalue equation with the eigenvalue
$$\lambda_{\vec{k}}=-\frac{4\pi}{V} \frac{V}{8\pi^3}\int d^3q \frac{1}{|\vec{k}-\vec{q}|^2}=-\frac{2k_{F}}{\pi}F\left( \frac{k}{k_{F}} \right).\tag{6.22} $$
where
$$F(x)=\frac{1}{2}+\frac{{1-x^2}}{4x}\ln \left\lvert  \frac{{1+x}}{1-x}  \right\rvert .\tag{6.23} $$
We now have the Hartree-Fock equations for jellium,
$$\left( -\frac{\nabla^2}{2}+V_{ext}+V_{H}+\hat{V}_{X} \right)\phi_{\vec{k}}(\vec{r})=\left( \frac{k^2}{2}+\lambda_{\vec{k}} \right)\phi_{\vec{k}}(\vec{r}).\tag{6.24} $$
![[Pasted image 20260130142401.png|369]]
The solutions don't exactly describe metals like Na, which behave more like free electrons, due to limitations of the Hartree-Fock equations - the slater determinant wavefunction does not hold for interactions. $\varepsilon_{k}$ is not very accurate for simple metals. It predicts they are almost insulating (semi-metals). This is a failure of lack of correlation, meaning our wavefunction is a slater determinant which treats electrons as non-interacting. 

The total energy of jellium in the Hartree-Fock approximation is given by
$$\bra{\Phi_{HF}} H\ket{\Phi_{HF}} =2\left[ \sum_{\vec{k}}^{k\leq k_{F}} \frac{k^2}{2}+\frac{1}{2}\sum_{\vec{k}}^{k\leq k_{F}}\lambda_{\vec{k}} \right].\tag{6.25} $$
$$\frac{2}{2}\sum_{\vec{k}}^{k\leq k_{F}}\lambda_{\vec{k}}=\dots=-\frac{3Nk_{F}}{4\pi}\implies\varepsilon_{X}=\frac{E_{X}}{N}=-\frac{3k_{F}}{4\pi}=-\frac{0.458}{r_{s}}\text{ a.u}=-\frac{0.915}{r_{s}}\text{ Ry}.\tag{6.26} $$
$\varepsilon_{X}$ is the exchange energy per electron. The kinetic energy term is 
$$T=\frac{2.21}{r_{s}^2}\tag{6.27} $$
which gives one positive energy contribution and one negative contribution which gives a minima.
![[Pasted image 20260130143150.png]]
The exact energy of jellium per particle is
$$\varepsilon_{exact}=\frac{2.21}{r_{s}^2}-\frac{0.916}{r_{s}}+\underbrace{ 0.0622\ln r_{s}-0.096+\mathcal{O}(r_{s}) }_{ \varepsilon_{c} }\tag{6.28} $$
where $\varepsilon_{c}$ is the energy difference between the exact solution and the Hartree-Fock approximation.