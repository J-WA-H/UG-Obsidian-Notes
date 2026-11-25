Distinguishable particles will be considered classically.
Indistinguishable particles will be considered quantum mechanically.
#### Indistinguishability
Consider a two particle wavefunction, $\psi(r_{1},r_{2})$, and a swap operator $\hat{S}$ that swaps the position of $r_{1}$ and $r_2$.
$$\hat{S}\psi(r_{1},r_{2})=\lambda \psi(r_{2},r_{1})$$
where $\lambda$ is some real number.
$$\hat{S}^2\psi(r_{1},r_{2})=\lambda^2\psi(r_{1},r_{2})$$
Since applying the swap operator twice should give us the same wavefunction, $\lambda^2=1\implies \lambda=\pm 1.$
This defines two classes of particles:
$$\hat{S}\psi(r_{1},r_{2})=-\psi(r_{2},r_{1})\text{ Fermions}$$
$$\hat{S}\psi (r_{1},r_{2})=\psi(r_{2},r_{1})\text{ Bosons}$$
Consider two Fermions at the same position $r_1=r_2=r$.
$$\psi(r,r)=-\psi(r,r)\implies \psi(r,r)=0.$$This shows that the probability of this scenario is 0, which is consistent with the Pauli exclusion principle.

Now consider a set of 3 spins.
Configurations: $\uparrow\uparrow\uparrow, \uparrow\uparrow\downarrow, \uparrow\downarrow\uparrow, \downarrow\uparrow\uparrow,\uparrow\downarrow\downarrow,\downarrow\uparrow\downarrow,\downarrow\downarrow\uparrow,\downarrow\downarrow\downarrow$.
The three spin up state is spin 3. The two spin up one spin down states are spin 1. The two spin down and one spin up states are spin -1. The three spin down state is spin -3.

$P(spin=3)=P(spin=-3)=\frac{1}{8}$
$P(spin=1)=P(spin=-1)=\frac{3}{8}.$

If we have $N$ distinguishable objects then we have $n!$ permutations.
If we split the N objects into two groups of size $r$, $N-r$, the number of possible permutations are
$$\begin{pmatrix}
1 \\
2
\end{pmatrix}=\frac{N!}{r!(N-r)!}.$$
  