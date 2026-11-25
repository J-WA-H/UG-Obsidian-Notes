Superconductor phenomenology is given by the effective interaction between electrons in metals. Focus on the simplest type of superconductors.

- Zero Resistance
	The typical signature of superconductivity is the vanishing of the electrical resistance below some critical temperature $T_{c}$. It is a second order phase transition of the electron gas at low temperatures. The superconducting state is a thermodynamically distinct state of matter. Below $T_{c}$, a current flows without loss.

- Meissner-Ochsenfeld Effect
	It is the expulsion of a magnetic field from a superconductor during its transition to the superconducting state when it is cooled below the critical temperature. The expulsion will repel a nearby magnet.
	![[Pasted image 20260329210932.png]]
	The figure shows the fall-off of the magnetic field in a Type-I superconductor. The penetration depth $\lambda$ is the distance over which the magnetic field decreases by $\frac{1}{e}$.
	Materials in which the Meissner effect is complete are known as Type-I superconductors, so their interior is a perfect diamagnet. A magnetic field applied at the boundary of a Type-I superconductor falls off exponentially with distance in the interior of the material. A rod-shaped sample of superconductor help parallel to a weak applied magnetic field $H_{appl}$ has the property that the field can penetrate only a short distance into the sample. This penetration depth is typically of the order of $10^{-5}\text{ cm}$. The Meissner effect is sometimes thought of as perfect diamagnetism.
	This is a little misleading. We would have perfect diamagnetism if the magnetic moment of the rod were the consequence  of a uniform magnetization of the rod. What really happens is the magnetization of the rod is due to currents flowing in the surface layers of the rod (perfect conductor).
	If we had uniform magnetisation inside the rod, the magnetic susceptibility would be $−1/4π$ which is the most negative value thermodynamically permissible:  
	Since the magnetic field inside a superconductor is zero,
	$$B-0=H_{appl}+4\pi M\tag{21.1} $$
	$H_{appl}$ is the applied field and $M$ is the magnetisation. Hence, the magnetisation is
	$$M=-\frac{1}{4\pi}H_{appl}\tag{21.2}. $$
	The negative value of $M$ signals that the interior of a superconductor is diamagnetic.
	If the strength of the applied field is increased the superconductivity is eventually destroyed, and this can happen in two ways. 
	In a type I superconductor the whole rod becomes normal at a critical applied field $H_{c}$.
	![[Pasted image 20260329213507.png]]
	In a Type-II superconductor, the magnetic field starts to penetrate the sample at an applied field, $H_{e{1}}$. However, $B$ approaches $H_{appl}$ within the rod only when a greater field, $H_{e 2}$, is reached, A thin surface layer may remain superconducting up to a higher field $H_{e 3}$.
	![[Pasted image 20260329213825.png]]
	The vortex lattice form a regular two-dimensional array in the plane perpendicular to $H_{appl}$. Often, we can predict whether a superconductor will be of type I or II from measurements of $∆$ and $λ$. We define the “coherence length” $ξ_{0} = ℏvF /π∆$ with $v_F$ the Fermi velocity. When $\lambda \gg\xi_{0}$ the superconductor tends to exhibit properties of type II.

- Acoustic Attenuation
	When sound wave propagates through a metal the microscopic electric fields due to the displacement of the ions can impart energy to electrons near $\varepsilon_{F}$, thereby removing energy from the wave. But when the energy of the sound wave is lower than $\hbar \omega < 2\Delta$ this cannot happen. So, experimentally, it is found that for $T<T_{c}$ the rate of attenuation is lower in a superconductor. No damping of impinging beam of phonons is observed if $\hbar \omega<2\Delta$.

-  Microwave and Infrared Properties/absorption of photons
	As a result of the gap, photons possessing energies less than $2\Delta$ are not absorbed: all such photons are reflected. Perfect reflection occurs for $\hbar \omega<2\Delta$. When this condition is true, photons see a completely resistance-less surface.
	When $\hbar \omega>2\Delta$, the behaviour approaches that of the normal state. We estimate this energy by assuming a [[Weak Coupling Limit]] description. Then $\Delta\sim 2k_{B}T_{c}$ and $\omega \sim 4k_{B}T_{c}/\hbar$. For $T_{c}=5\text{K}$, $\omega\sim 10^{12}\text{ s}^{-1}$. This frequency is in the infrared. Infrared radiation can then penetrate a superconductor and scatter the electrons.

- Heat Capacity
	In the superconducting state, the entropy decreases continuously but dramatically, signalling the formation of a highly ordered state,
	![[Pasted image 20260329214927.png]]
	The temperature derivative of the entropy is steeper on the superconducting side than on the normal side of the transition. Superconductivity is a second-order phase transition.
	The heat capacity $C_{V}$ is discontinuous at $T_{c}$.
	![[Pasted image 20260329215110.png]]
	The heat capacity $C_{S}$ falls off as $C_{S}\propto \exp[-\Delta/k_{B}T]$ where $\Delta$ is an energy scale. A heat capacity of this form is indicative of an energy gap in the excitation spectrum. The formation of a gap at the Fermi-level in the superconducting state results in a lowering of the ground state energy of the system. The gap is $2\Delta$.
	Thermodynamically, the gap gives rise to a discontinuity in the heat capacity,
	$$C_{S}(T_{c})=C_{N}(T_{c}')\neq 0\tag{21.3} $$
	![[Pasted image 20260329215356.png]]
	A weak coupling superconductor has $\frac{2\Delta(T=0)}{k_{B}T_{c}}$ is between $1,3$. The strong coupling is
	$$\frac{2\Delta(T=0)}{k_{B}T_{c}}>4\tag{21.4} $$
	The basic energy scale for the creation of an electron-hole pair in a superconductor is $2\Delta$.

- Isotope Effect
	Experimentally, it is observed that if the mass of the ions is changed isotopically, $T_{c}$ changes accordingly
	$$T_{c}\propto \frac{1}{\sqrt{ M }}\propto \omega_{D}\tag{21.5} .$$
	This observation implies that electron-phonon coupling is at the heart of [[BCS Superconductivity]] (phonon-mediated superconductivity.)
	The isotope effect assumes the harmonic approximation for the phonon frequencies. If there are strong anharmonicities, the isotope effect is difficult to quantify.
