We have the Hamiltonian for [[Electron-Phonon Interaction]]
$$H'=H_{0}+\sum_{\vec{k},\vec{k}',\vec{q}}\sum_{\sigma,\sigma'}|M_{\vec{q}}|^2 \frac{\hbar\omega_{\vec{q}}}{(\varepsilon_{\vec{k}'}-\varepsilon_{\vec{k}-\vec{q}})^2-(\hbar \omega_{\vec{q}})^2}c_{\vec{k}'+\vec{q},\sigma'}^{\dagger}c_{\vec{k}-\vec{q},\sigma}^{\dagger}c_{\vec{k},\sigma}c_{\vec{k},\sigma'}\tag{19.1}.$$
They lie close together when they are near the Fermi energy,
$$\varepsilon_{\vec{k}'},\varepsilon_{\vec{k}-\vec{q}},\varepsilon_{\vec{k}'+\vec{q}}\simeq\varepsilon_{F}\implies V_{\vec{q}}^{eff}=-\frac{|M_{\vec{q}}|^2}{\hbar \omega_{\vec{q}}}\tag{19.2}. $$
This gives that electrons deforms the crystal around it as a phonon is emitted.

Consider 2 electrons at the Fermi surface. They could lower their energy by forming a bound state using available states. The available states have momenta near $\vec{k}_{F}$ because of Pauli's exclusion principle. If the effective attractive interaction is short range, the two electrons will arrange their spins $\uparrow\downarrow$ and form a singlet. This is the Cooper instability of electron gas by formation of pairs in the presence of weak particle-particle interactions at $T=0$ (low $T$).

We cast the electron-proton Hamiltonian in an effective e-e interaction, with the reduced Hamiltonian
$$H_{red}=\sum_{\vec{p},\sigma}\varepsilon_{\vec{p}}c_{\vec{p}\sigma}^{\dagger}c_{\vec{p}\sigma}+\sum_{\vec{p},\vec{q}}V_{\vec{p}\vec{q}}c_{\vec{p}\uparrow}^{\dagger}c_{-\vec{p}\downarrow}^{\dagger}c_{-\vec{q}\downarrow}c_{\vec{q}\uparrow}\tag{19.3} $$
Using $\varepsilon_{\vec{p}}=\varepsilon_{-\vec{p}}$ we rewrite,
$$H_{red}=\sum_{\vec{p}}\varepsilon_{\vec{p}}[c_{\vec{p}\uparrow}^{\dagger}c_{\vec{p}\uparrow}+c_{-\vec{p}\downarrow}^{\dagger}c_{-p\downarrow}]+\sum_{\vec{p},\vec{q}}V_{\vec{p}\vec{q}}c_{\vec{p}\uparrow}^{\dagger}c_{-\vec{p}\downarrow}^{\dagger}c_{-\vec{q}\downarrow}c_{\vec{q}\uparrow}\tag{19.4} $$
In a more compact notation, the positive sign in front of the wavenumber implies the spin up and negative signs implies spin-down:
$$H_{red}=\sum_{\vec{p}}\varepsilon_{\vec{p}}[c_{\vec{p}}^{\dagger}c_{\vec{p}}+c_{-\vec{p}}^{\dagger}c_{-\vec{p}}]+\sum_{\vec{p},\vec{q}}V_{\vec{p}\vec{q}}c_{\vec{p}}^{\dagger}c_{-\vec{p}}^{\dagger}c_{-\vec{q}}c_{\vec{q}}\tag{19.5}. $$
The number operator is
$$\hat{N}=\sum_{\vec{p}}[c_{\vec{p}}^{\dagger}c_{\vec{p}}+c_{-\vec{p}}^{\dagger}c_{-\vec{p}}]\tag{19.6}. $$
Assume Bose-Einstein condensation $\vec{p}=0$ state. Hence, $\vec{k}+\vec{k}'=0$. Use the Trial BCS state,
$$\ket{\Psi_{BCS}}=\prod_{\vec{k}}(U_{\vec{k}}+U_{\vec{k}}c_{\vec{k}\uparrow}^{\dagger}c^{\dagger}_{-\vec{k}\downarrow})\ket{0} \tag{19.7}. $$
$\hat{N}$ is not a good quantum number for $\ket{\Psi_{BCS}}$ or $\ket{\Psi_{n}}$.

We can see if the normal state is a BCS state,
$$\ket{\Psi_{n}}=c_{k_{\frac{N}{2}}\downarrow}^{\dagger}c_{k_{\frac{N}{2}}\uparrow}^{\dagger}\dots c_{k_{2}\downarrow}^{\dagger}c_{k_{1}\downarrow}^{\dagger}c_{k_{1}\uparrow}^{\dagger}\ket{0}\tag{19.8}=\left( c_{-k_{\frac{N}{4}}\downarrow}^{\dagger}c_{k_{\frac{N}{4}}\downarrow}^{\dagger}\dots c_{k_{1}\downarrow}c_{-k_{1}\downarrow} \right)\left( c_{-k_{\frac{N}{4}}\uparrow}^{\dagger} c_{k_{\frac{N}{4}}\uparrow}^{\dagger}\dots c_{-k_{1}\uparrow}^{\dagger}c_{k_{1}\uparrow}^{\dagger} \right)\ket{0}.$$
For the normal state we have
$$\begin{cases}
\vec{k}\leq \vec{k}_{F} \begin{cases}
v_{k}=1 \\
u_{k}=0
\end{cases} \\
\vec{k}>\vec{k}_{F}\begin{cases}
u_{k}=1 \\
v_{k}=0
\end{cases}
\end{cases} \tag{19.9} $$
This shows the normal state is a BCS state so for a fixed number of electrons, either $u_{k}$ or $v_{k}$ must be zero.

From expectation values,
$$\braket{ \Psi_{BCS} | \Psi_{BCS} }= \prod_{\vec{p}}(u_{\vec{p}}^{*}u_{\vec{p}}+v_{\vec{p}}^{*}v_{\vec{p}})\tag{19.10} $$
$$\bra{\Psi_{BCS}}\hat{N}\ket{\Psi_{BCS}}=2\sum_{\vec{k}}v_{\vec{k}}^{*}v_{\vec{k}}\prod_{\vec{p}\neq \vec{k}}(u_{\vec{p}}^{*}u_{\vec{p}}+v_{\vec{p}}^{*}v_{\vec{p}})\tag{19.11}.   $$
$$\bra{\Psi_{BCS}}H_{red}\ket{\Psi_{BCS}}=2\sum_{\vec{k}}\varepsilon_{\vec{k}}v_{\vec{k}}^{*}v_{\vec{k}}\prod_{\vec{p}\neq \vec{k}}(u_{\vec{p}}^{*}u_{\vec{p}}+v_{\vec{p}}^{*}v_{\vec{p}})+\sum_{\vec{k},\vec{k}'}V_{\vec{k}\vec{k}'}u_{\vec{k}'}^{*}v_{\vec{k}}^{*}u_{\vec{k}}v_{\vec{k}'}\prod_{\vec{p}\neq \vec{k},\vec{k}'}(u_{\vec{p}}^{*}u_{\vec{p}}+v_{\vec{p}}^{*}v_{\vec{p}})  \tag{19.12}. $$
$$\bra{\Psi_{BCS}}c_{-\vec{q}\downarrow}c_{\vec{q}\uparrow}\ket{\Psi_{BCS}} =u_{\vec{q}}^{*}v_{\vec{q}}\prod(|u_{\vec{p}}|^2+|v_{\vec{p}}|^2)\neq 0\tag{19.13}.  $$
From the norm $\braket{ \Psi_{BCS} | \Psi_{BCS} }=1$ we can choose
$$|u_{\vec{k}}|^2+|v_{\vec{k}}|^2=1,\qquad \forall\;\vec{k}\tag{19.14}. $$
This simplifies the expectation values.

We can introduce a new variable $u_{\vec{k}}=\sin \theta_{\vec{k}},\;v_{\vec{k}}=\cos \theta_{\vec{k}}$. 

To optimise the trial BCS state, use the [grand-canonical ensemble](Statistical%20Physics%20from%20Quantisation.md) $(T=0)$ and minimise
$$\bra{\Psi_{BCS}}H_{red}-\mu \hat{N}\ket{\Psi_{BCS}}=\sum_{\vec{p}}(\varepsilon_{\vec{p}}-\mu)(1+\cos 2\theta_{\vec{p}}) +\frac{1}{4}\sum_{\vec{p},\vec{p}'}V_{\vec{p}\vec{p}'}\sin 2\theta_{\vec{p}}\sin 2\theta_{\vec{p}'}\tag{19.15}.  $$
Fix the average number of particles with $N=\varepsilon_{F}$, and take the derivative with respect to $\theta_{\vec{k}}$ and set it to zero.
$$-2\sin 2\theta_{\vec{k}}(\varepsilon_{\vec{k}}-\mu)+2 \frac{2}{4}\cos 2\theta_{\vec{k}}\sum_{\vec{p}}V_{\vec{k}\vec{p}}\sin 2\theta_{\vec{p}}=0\implies(\varepsilon_{\vec{k}}-\mu)\tan \theta_{\vec{k}}=-\left( \underbrace{ -\sum_{\vec{p}}V_{\vec{k}\vec{p}}\sin \theta_{\vec{p}}\cos \theta_{\vec{p}}  }_{ e^{ -i\alpha }\Delta_{\vec{k}} }\right)\tag{19.16} .$$
with
$$\Delta_{\vec{k}}=-\sum_{\vec{p}}V_{\vec{k}\vec{p}}\sin \theta_{\vec{p}}\cos \theta_{\vec{p}}e^{ i\alpha }=-\sum_{\vec{q}}V_{\vec{k}\vec{q}}u_{\vec{q}}^{*}v_{\vec{q}}=-\sum_{\vec{q}}V_{\vec{k}\vec{q}}\bra{\Psi_{BCS}} c_{-\vec{q}\downarrow}c_{\vec{q}\uparrow}\ket{\Psi_{BCS}} \tag{19.17} .$$
This is the mean field picture.

Minimisation gives
$$\tan 2\theta_{\vec{k}}=\frac{e^{ -i\alpha }}{\varepsilon_{\vec{k}}-\mu},\qquad\sin 2\theta_{\vec{k}}=\frac{e^{ -i\sigma }}{E_{\vec{k}}},\qquad \cos 2\theta_{\vec{k}}=\frac{{\mu-\varepsilon_{\vec{k}}}}{E_{\vec{k}}}\tag{19.18} $$
where
$$E_{\vec{k}}=\sqrt{ |\Delta_{\vec{k}}|^2+(\varepsilon_{\vec{k}}-\mu)^2 }\tag{19.19}. $$
This gives
$$\Delta_{\vec{k}}=-\frac{1}{2}\sum_{\vec{p}}V_{\vec{k}\vec{p}}\sin 2\theta_{\vec{p}}e^{ i\alpha }=-\frac{1}{2}\sum_{\vec{p}}V_{\vec{k}\vec{p}} \frac{\Delta_{\vec{p}}}{E_{\vec{p}}}\tag{19.20}. $$
We consider
$$V_{\vec{k}\vec{p}}=\begin{cases}
-V & |\varepsilon_{\vec{k},\vec{p}}-\mu|<\omega_{D} \\
0 & \text{otherwise}
\end{cases}\tag{19.21} $$
This gives
$$|\Delta_{\vec{k}}|=\frac{V}{2}\sum_{|\varepsilon_{\vec{p}}-\mu|<\omega_{D}} \frac{|\Delta_{\vec{p}}|}{\sqrt{ \Delta^2+(\varepsilon_{\vec{p}}-\mu)^2 }}\tag{19.22}.$$
We obtain $\Delta_{\vec{k}}=0$ for $|\varepsilon_{\vec{k}}-\mu|>\omega_{D}$.

Try the solution with $\Delta_{\vec{k}}$ independent of $\vec{k}$, $\Delta_{\vec{k}}=\Delta e^{ i\vartheta }$ for $\varepsilon_{\vec{k}}\simeq \mu$.
$$1=\frac{V}{2}\sum_{|\varepsilon_{\vec{p}}-\mu|<\omega_{D}} \frac{1}{\sqrt{ \Delta^2+(\varepsilon_{\vec{p}}-\mu)^2 }}\tag{19.23} $$
The phase $\vartheta$ of $\Delta_{\vec{k}}$ is undetermined. This is the basic equation to obtain $\Delta$. 

Note for $\varepsilon_{\vec{k}}<\mu-\omega$, 
$$\sin 2\theta_{\vec{k}}=2\underbrace{ \sin \theta_{\vec{k}} }_{ |u_{\vec{k}}|=0 }\underbrace{ \cos \theta_{\vec{k}} }_{ |v_{\vec{k}}|=1 }=0\tag{19.24}. $$
The fact that $\sin 2\theta_{\vec{K}}=0$ implies that either $|u_{\vec{k}}|$ or $|v_{\vec{k}}|=0$, and from equation $(19.9)$, the other must be 1. For $\varepsilon_{\vec{k}}<\varepsilon_{F}$ $|u_{\vec{k}}|=0$ and $|v_{\vec{k}}|=1$.

For $\varepsilon_{\vec{k}}>\mu+\omega$, $\varepsilon_{\vec{k}}>\varepsilon_{F}$ so $|u_{\vec{k}}|=1$ and $|v_{\vec{k}}|=0$.

For $\mu-\omega_{D}\leq\varepsilon_{\vec{k}}\leq \mu+\omega_{F}$, since 
$$\cos^2\theta_{\vec{k}}=\frac{1}{2}(1+\cos 2\theta_{\vec{k}})=\frac{1}{2}\left( 1-\frac{{\varepsilon_{\vec{k}}-\mu}}{E_{\vec{k}}} \right)\tag{19.25} $$
we have
$$|v_{\vec{k}}|^2=\cos^2\theta_{\vec{k}}=\frac{1}{2}\left( 1-\frac{{\varepsilon_{\vec{k}}-\mu}}{E_{\vec{k}}} \right),\qquad |u_{\vec{k}}|^2=\frac{1}{2}\left( 1+\frac{{\varepsilon_{\vec{k}}-\mu}}{E_{\vec{k}}} \right)\tag{19.26} $$
![[Pasted image 20260329130946.png]]
