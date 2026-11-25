The [drop-model](The%20Strong%20Force%20and%20Binding%20Energy.md) fails to predict some binding energies by underestimating it for certain isotopes.
![[Pasted image 20241206102229.png]]
For the shell nuclear model, consider the potential for a given nucleon sourced by the rest of the nucleus which is in a $J=0$ [state](Angular%20Momentum.md) - as each nucleon is coupled.
![[Pasted image 20241206102444.png]]
The potential experienced by the nucleon is given by
$$V(r)=V_{0}(r)+V_{LS}(r)\underline{L}\cdot \underline{S}.$$
To find the energy levels of this nucleon, first solve the first wavefunction from $V_{0}$
$$\frac{1}{r^2} \frac{d}{dr}\left( r^2 \frac{d\psi(r)}{dr} \right)+\left( V_{0}-\frac{l(l+1)}{r^2} \right)\psi(r)=E\psi(r).$$
This gives the principle quantum number $n$.
We also find the splitting from the spin-orbit coupling, $\Delta E_{SO}=\bra{nJ}V_{LS}\underline{L}\cdot \underline{S}\ket{nJ}.$

The $nL$ convention tells us the principal and orbital angular momentum quantum numbers. E.g. $1S$ means $n=1,l=0$.
$J$ is given by
$$\left\lvert  l-\frac{1}{2}  \right\rvert\leq J\leq l+\frac{1}{2}. $$
For a spin $J$ there are $2J+1$ states.

The nuclear shell model makes predictions for spin and [parity](Symmetries%20and%20Parity.md), with two assumptions
- States found for the one nucleon potential are valid for all nucleons.
- Two protons or neutrons in the same state pair up to give 0 spin/angular momentum.

Spin and parity will be given by unpaired electrons.

For an even number of protons and an even number of neutrons, all protons and neutrons pair up so $J_{tot}=0$, $P=((-1)^{L})^{N_{p}}((-1)^{L})^{N_{n}}$. Here $N_{p}=N_{n}$, which is some even number.

For an even-odd configuration, $J_{tot}=J$, which is the angular momentum of the unpaired proton, $P=(-1)^{L}$, also from the left over proton.

For an odd-odd configuration, we have an unpaired proton and an unpaired neutron. The angular momentum lies between $\lvert J_{p}-J_{n} \rvert\leq J_{tot}\leq J_{p}+J_{n}$ and parity $P=(-1)^{L_{p}}(-1)^{L_{n}}$.
