Consider an [Intrinsic semiconductor](Intrinsic%20Semiconductors.md) like Si with dopants (Foreign atoms). Consider adding a phosphorus atom in the silicon lattice.
![[Pasted image 20250219161812.png]]
The double line represents a covalent bond - not a double bond. Phosphorus has 5 valence electrons so there is one unbound electron.
Considering the band structure:
![[Pasted image 20250219162339.png]]
The unbound electron cannot be in the valance bound as it doesn't form a covalent bound, and it cannot be in the conduction band as it is still weakly bound the phosphorus atom so it cannot move freely through the crystal. This means it must exist in its own energy level - the donor level.

From Bohr's theory of the hydrogen atom, the energy is
$$E=\frac{e^{4}m}{2(4\pi\varepsilon_{0}\hbar)^2}.$$
Adjusting this for semiconductors gives
$$E_{SC}=\frac{e^4m^{*}}{2(4\pi\varepsilon_{r}\varepsilon_{0})^2}$$
where $\varepsilon_{r}$ is the relative permittivity, which is $\approx 11$ for Si.

Because of $\varepsilon_{r}$, $E_{SC}$ is much smaller than the hydrogen atom, $E=-13.6\text{ eV}$, so $E_{SC}$ is of order $\text{meV}.$ 
Considering the Bohr radius,
$$r=\frac{4\pi \varepsilon_{0}\hbar^2}{me^2}\to r_{SC}=\frac{4\pi\varepsilon_{0}\varepsilon_{r}\hbar^2}{m^{*}e^2}.$$
This implies the donor electrons are delocalised due to larger separation and smaller energy.

At $T=0\text{ K}$, both the valence and donor band are full.
As temperature is increased, the smallest energy transition is between the donor level and the conduction band so this is prioritised.
![[Pasted image 20250219164557.png]]
This is the freeze-out regime where donors are ionised.
![[Pasted image 20250219164703.png]]
Electron carriers are generated, but not holes.

If temperature increases further, then eventually all donor electrons move to the conduction band. This is the saturation regime where all donors are ionised, but the valance band is still full.
![[Pasted image 20250219164919.png]]
As temperature is increased even further, all valence band electrons move to the conduction band so both electrons and holes are generated.
This is the intrinsic regime.
![[Pasted image 20250219165046.png]]
Plotting electron concentration against temperature gives these three regimes.
![[Pasted image 20250219165144.png]]
For most semiconductors, at room temperature they fall in the saturation regime.
To work out the concentration use the law of mass action:
$$np=N_{C}N_{V}\exp\left[ -\frac{E_{g}}{k_{B}T} \right].$$
This is valid for any semiconductor.
For the intrinsic semiconductor, $np=n_{i}^2$ and $n=p+N_{D}$ where $N_D$ is the donor concentration.

Solving these equations for $n$ give
$$n=\frac{N_{D}}{2}+\sqrt{ \left( \frac{N_{D}}{2} \right)^2+n_{i}^2 }.$$
Assume $N_{D}\gg n_{i}\therefore n\approx N_{D}$ for saturation.
$$\implies p=\frac{n_{i}^2}{N_{D}}.$$
$$\implies n>n_{i}, \; p=n_{i}\left( \frac{n_{i}}{N_{D}} \right)<n_{i}\implies n>p.$$
This means electrons are the majority carriers. These are n-type semiconductors ($n>p$).

For the chemical potential - consider the intrinsic case where $\mu$ lies in the middle of the band gap.

For extrinsic n-type semiconductor, both the valance and donor bands are full so considering the shape of the [[Fermi-Dirac Distribution]] at $T=0\text{ K}$, it is a step function at $\mu$ so the chemical potential must be between $E_{d}$ and $E_{C}$.
![[Pasted image 20250219170215.png]]
In the saturation regime $n\approx N_{D}$ so
$$n=N_{C}\exp\left[ -\left( \frac{{E_{C}-\mu}}{k_{B}T} \right) \right]$$
$$N_{D}=N_{C}\exp\left[ -\left( \frac{{E_{C}-\mu}}{k_{B}T} \right) \right]\implies \mu=E_{C}-k_{B}T\ln\left( \frac{N_{C}}{N_{V}} \right).$$
