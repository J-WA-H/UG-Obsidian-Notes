There are many tests of the standard model that strongly constrain and BSM theories:
- Electroweak precision tests
	Consider the diagram
	![[Pasted image 20260330105931.png]]
	With loop corrections, the photon propagator becomes
	$$-\frac{ig_{\mu \nu}}{q^2-m_{v}^2}\to -\frac{ig_{\mu \nu}}{q^2-m_{v}^2+\Pi_{vv}(q^2)}\tag{12.1} $$
	where $\Pi_{vv}(q^2)$ gives the effective mass from loop corrections. $vv=WW,ZZ,\gamma \gamma,\gamma Z$.
	$$T=\frac{1}{\alpha}\left( \frac{\Pi_{WW}(0)}{m_{W}^2}-\frac{\Pi_{ZZ}(0)}{m_{Z}^2} \right)\tag{12.2} .$$
	This shows new physics couple in the same way to the $W$ and $Z$. Experiments show $T\sim 0.05\pm 0.1$.

- Higgs Couplings: SM fixes these as masses are known
- [[Flavour Physics]]: CKM, CPV in the standard model, $\mathcal{M}_{SM}\sim \frac{g^2}{16\pi^2} \frac{\text{CKM factors}}{M_{W}^2}$.
	From this
	$$\mathcal{M}_{BSM}\sim \frac{g_{*}^2}{M_{BSM}^2}\implies M_{BSM}\gg M_{W}\tag{12.3} $$
	can still compete.
- QCD measurements: e.g. [[Deep Inelastic Scattering]], hadron spectroscopy
- Direct searching for new states or SM forbidden processes.

Even though the standard model has passed many experimental tests, there are still many open problems,
- Quantum gravity
- Dark matter - must be electrically neutral, stable non-relativistic, weakly interacting
	One possible candidate are WIMPs. Initially, these WIMPs can transfer to and from the SM,
	$$X\bar{X}\leftrightarrow SM\tag{12.4} $$
	As the universe cools,
	$$X\bar{X}\xrightarrow{T\lesssim m_{X}}SM\tag{12.5} $$
	Then Freeze-out, the annihilation stops happening.
	![[Pasted image 20260330112353.png]]
	The relic abundance is $\sim \frac{1}{\langle \sigma v \rangle}\sim \frac{m_{X}^2}{g^4}$. Choosing $g\sim 0.1-1$ (weak coupling) gives $M_{X}\sim 10-100\text{ GeV}$.
	This is loosing favour due to experimental constraints.
	New candidates includes ultra-light dark matter (axions) with $m\sim 10^{-22}\text{ eV}-1\text{ eV}$, or primordial black holes $m\sim 10^{6}M_{\odot}$.

Another problem is neutrino masses. Extensions to describe this adds right-handed neutrinos $\nu_{R}$. This adds a term $m_{D}\bar{\nu}_{L}\nu_{R}$ that is consistent with the standard mode, but sterile neutrinos are also consistent, $\frac{1}{2}M_{R}\nu_{R}^{T}c\nu_{R}$. This is the SM singlet so doesn't violate $SU(2)$.

$M_{D}\sim 100\text{ GeV}$, and $M_R$ could be very large.
$$\mathcal{L}\ni -\frac{1}{2}\begin{bmatrix}
\bar{\nu}_{L} & \bar{\nu}_{R}'
\end{bmatrix}\begin{bmatrix}
0 & M_{D} \\
M_{D} & M_{R}
\end{bmatrix}\begin{bmatrix}
\nu_{L}' \\
\bar{\nu}_{R}
\end{bmatrix}\implies \begin{vmatrix}
-\lambda & M_{D} \\
M_{D} & M_{R}-\lambda
\end{vmatrix}=0\tag{12.6} $$
This gives
$$\lambda^2-M_{R}\lambda-M_{D}^2=0\implies\lambda=\frac{M_{R}}{2}\pm \frac{1}{2}\sqrt{ M_{R}^2-4M_{D}^2 }\tag{12.7}. $$
This gives $\frac{M_{D}^2}{M_{R}}\sim 0.1\text{ eV}$, so small ratio could give neutrino masses, if $M_{R}\sim 10^{14}\text{ GeV}$.

Another problem is matter-antimatter asymmetry. We know that matter dominates. The asymmetry is
$$\eta_{B}= \frac{{n_{B}-n_{\bar{B}}}}{n_{\gamma}}\approx 6\times 10^{-10}\tag{12.8} .$$
To build a theory to explain this, we must have
1. Violation of baryon number
2. C+CP violation
3. Departure from equilibrium, B-violating interactions drive $\mu_{B}\to 0$.
$$n_{B}=g\int \frac{d^3p}{(2\pi)^3} \frac{1}{e^{ (E-\mu_{B})/T }+1}=n_{\bar{B}}.\tag{12.9} $$
	To extend the standard model,
	1. Respect gauge symmetry
	2. Consider allowed interactions
	3. Look for symmetries
	4. Consider with tests and check future tests
	5. Does it solve a problem

