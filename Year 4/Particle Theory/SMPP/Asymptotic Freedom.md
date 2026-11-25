So far only tree level diagrams have been considered. In reality, we have to consider quantum loop corrections.
![[Pasted image 20260309104310.png]]
For example, a propagating photon can emit a virtual fermion pair, which then annihilate and another photon propagates.
![[Pasted image 20260309104520.png]]
$\ell$ is an unconstrained momenta so we integrate over it,
$$\int \frac{d^4\ell}{(2\pi)^4} \frac{g^2}{(q-\ell)^2\ell^2}\tag{9.1} $$
which is logarithmically divergent.

This is solved through renormalisation. Infinities are absorbed into parameters, so the Lagrangian parameters no longer represent to observables. The measured couplings at an energy $E$ gives the bare coupling plus the corrections up to scale $E$. These give
$$\alpha(s)=\frac{g^2(s)}{4\pi}=\alpha(s_{0})-\frac{\beta}{4\pi}\alpha^2(s_{0})\log\left( \frac{s}{s_{0}} \right)\tag{9.2} $$
$\beta$ is the beta function which encodes the theory. For [[QCD]] and QED,
$$\beta_{QED}=-\frac{4}{3},\qquad \beta_{QCD}=11-\frac{2}{3}N_{q}\tag{9.2} $$
This shows for QCD, $\alpha$ shrinks in the UV range, and grows in the IR range.

This shows the coupling gets weaker for higher energies in QCD, known as asymptotic freedom. This shows why quark confinement happens, at low energies, the coupling constant is large so quarks do not exist on their own, however at high energies the coupling constant is low so we do get free quarks.