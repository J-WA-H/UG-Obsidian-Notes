 The resistivity of a metal with respect to temperature can be modelled by
$$\rho(T)=\rho_{0}+aT^2+bT^5.$$
The quadratic term comes from electron-electron scattering, the quintic term comes from electron-phonon scattering and $\rho_{0}$ is due to impurities. Plotting this gives the expected resistivity,
![[Pasted image 20250226164314.png]]
The purer the material, the smaller $\rho_{0}$.

However, if the resistivity of mercury is measured, the results are
![[Pasted image 20250226164411.png]]
where there is a discontinuous jump to zero resistivity at some critical temperature $T=T_{c}$. For mercury it is about $\approx 4\text{ K}$.

The discontinuous jump in resistivity implies a phase transition. This gives a new state of matter - the superconducting state.

Materials with the highest $T_{c}$ are high $T_c$ cuprates, they consist of copper and oxygen. These have a high $T_c$ so can be cooled with liquid nitrogen so they have many industrial applications.

Ohm's law gives
$$\underline{J}=\sigma \underline{E}$$where $\sigma$ is the conductivity. 
For a superconductor,
$$\sigma=\frac{1}{\rho}\to \infty$$
For a constant current density, the E-field must be zero.

Superconductors don't need an E-field to drive charge.

Faraday's law:
$$\underline{\nabla}\times \underline{E}=-\frac{ \partial \underline{B} }{ \partial t }=0 $$
$\implies$ the B-field is independent of time.
Consider a strip of a superconducting material and apply a B-field at $T>T_{c}$:
![[Pasted image 20250226165953.png]]
- At $T>T_{c}$, the strip is in its normal state and a B-field is applied.
- Cool to $T<T_{c}$ so it transitions to the superconducting state
- Then turn off the B-field so $\underline{B}_{applied}=\underline{0}$.
![[Pasted image 20250226170321.png]]
Since the B-field is time-independent, the material tries to restore this B-field.
- This generates a supercurrent to restore the B-field.

As superconductors have zero resistivity, the current keeps going so it doesn't decay like a normal metal,
$$J(t)=J_{0}\exp\left[ -\frac{t}{\tau} \right]$$
where $\tau$ is the scattering time. For a superconductor, the scattering time is of the order of years which is why it appears to not decay.

In the normal state, the $B$ field penetrates the material unaffected as it is non-magnetic, but for a superconductor, it is a perfect [diamagnet](Diamagnetism.md), it repels the B-field.
![[Pasted image 20250226170832.png]]
This is the Meissner effect.

For a diamagnet, $\underline{B}=\underline{0}$ so using $\underline{B}=\mu_{0}(\underline{M}+\underline{H})$ which gives $\underline{M}=-\underline{H}$.
This gives the volume magnetic susceptibility as
$$\chi=\frac{M}{H}=-1.$$
