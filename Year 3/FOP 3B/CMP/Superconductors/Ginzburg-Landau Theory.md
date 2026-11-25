There are two main theories of superconductivity:
- Bardeen, Cooper, and Schrieffer (BCS) theory
	- This is a microscopic theory that is valid for elements but not for high $T_{c}$ [cuprates](Superconductivity.md)
- Ginzburg-Landau Theory (GL):
	- This is a phenomenological theory
	- Has order parameters, e.g. magnetisation for [[Ferromagnetism]] and $|\psi|^2$ for superconductivity where $\psi\in \mathbb{C}$.

Close to the critical temperature the [free energy](Thermodynamics%20of%20Superconductivity.md) is
$$G_{S}(T)=G_{N}(T)+a(T)|\psi|^2+\frac{b(T)}{2}|\psi|^4.$$
The quadratic and quartic term are some perturbations.

GL theory is a purely mathematical construct but matches with the observed physics.

Consider the leading coefficient, there are two possible configurations
![[Pasted image 20250227160322.png]]
The first possibility is an energy minimum and the second is an energy maximum.
As the system tries to minimise energy, the second graph must be the one observed which gives $b(T)>0$.

Consider the order parameter at equilibrium,
$$\frac{dG_{S}}{d|\psi|}=2|\psi|[a(T)+b(T)|\psi^2|]=0$$
This is set to zero to make sure this is a minimum.
This gives two solutions,
$$|\psi|=0;\;|\psi|^2=-\frac{a(T)}{b(T)}.$$
If $|\psi|=0$, there is no superconductive electrons so this solution is the normal state.

If $|\psi|^2=-\frac{a(T)}{b(T)}$, this is the solution for the superconducting state. This can be shown by considering the two regions
- $T>T_{c}$ (normal), $a(T)>0$ so $|\psi|^2<0$ which is unphysical so $|\psi|=0$.
- $T<T_{c}$ (superconducting), $a(T)<0$ so $|\psi|^2>0$ which is physical

Taylor expanding the parameters gives
$$b(T)=b>0$$
$$a(T)=0+(T-T_{c})\dot{a}=(T-T_{c})\dot{a}$$
$$\therefore |\psi|^2=\frac{\dot{a}(T-T_{c})}{b}.$$
Consider thermodynamics of GL theory,
![[Pasted image 20250227161331.png]]
To find the condensation energy, substitute the equilibrium $|\psi|^2$,
$$|\psi|^2_{eqm}=\frac{\dot{a}(T-T_{c})}{b}.$$
This gives the condensation energy
$$\frac{\dot{a}^2(T-T_{c})^2}{2b}.$$
From thermodynamics, the condensation energy is
$$\frac{B_{c}^2(T)}{2\mu_{0}}=\frac{\dot{a}^2(T-T_{c})^2}{b}.$$
The entropy is
$$S=-\frac{dG}{dT}=-\frac{\dot{a}^2(T-T_{c})}{b}=S_{N}-S_{S}.$$
At $T=T_{c}$, $S_{N}=S_{S}$ so there is no latent heat so this is a second order transition.

