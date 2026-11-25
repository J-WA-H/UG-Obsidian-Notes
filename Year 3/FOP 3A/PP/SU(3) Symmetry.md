Consider all 9 possible ground state meson, $1^{1}S_{0}$, combinations of up, down and strange quarks,

| $\pi^{+}(u\bar{d})$ | $\pi^{-}(d\bar{u})$     | $\pi^{0}\left( \frac{1}{\sqrt{ 2 }}(u\bar{u}+d\bar{d}) \right)$        | $k^{+}(u\bar{s})$                                                      | $k^{-}(s\bar{u})$ |
| ------------------- | ----------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------- | ----------------- |
| $k^{0}(d\bar{s})$   | $\bar{k}^{0}(\bar{d}s)$ | $\eta\left( \frac{1}{\sqrt{ 6 }}(u\bar{u}+d\bar{d}-2s\bar{s}) \right)$ | $\eta'\left( \frac{1}{\sqrt{ 3 }}(u\bar{u}+d\bar{d}+s\bar{s}) \right)$ |                   |
Plotting these particles on a graph of [[Isospin and Strangeness]] gives
![[Pasted image 20250227191501.png]]
Here it can be seen that the $\pi$ triplet each differs by an isospin of 1.
Antiparticles are the reflection though the origin.
Consider the same plot for the first excited state, $1^{3}S_{1}$.
![[Pasted image 20250228100146.png]]
This shows the symmetry between the different types of $u,d,s$ mesons.

Similarly [[Colour Charge]], we've seen how colour flows through a diagram mediated by [[Gluons]]. This allows colour of particles to be swapped.

Nature flips red, green and blue colour via gluons.

Such a flipping can be represented by [[Rotations]]. Consider a basis of colours
$$C=\{ \ket{r} , \ket{g} , \ket{b}  \}.$$
We can define an operator/matrix $F$ s.t.
$$F\ket{c_{j}} =\pm \ket{c_{j}} $$
where $\ket{c_{i}},\ket{c_{j}}\in C$.
Represent the basis as column vectors
$$\ket{r} =\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix},\;\ket{g} =\begin{bmatrix}
0 \\
1 \\
0
\end{bmatrix},\;\ket{b} =\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}.$$
These vectors can be mapped onto each other using rotation matrices.
So $F$ doesn't change the magnitude of the vector, it must have determinant 1.
Rotations are also unitary as $RR^{\dagger}=\mathbb{I}$ so these matrices belong in the [special unitary group](Unitary%20and%20Orthogonal%20Operators.md) of 3x3 matrices, $SU(3)$.
There are 9 possible matrices that rotate these colours - the identity and the Gell-Mann matrices.
These form the $SU(3)$ group - it is the symmetry that mediates colour through a diagram.

A similar analogy can be applied to the weak force. Particle types are changed via the $W^{\pm}$ bosons, which changes the charge by $\pm 1$.
![[Pasted image 20250228101934.png]]
These also apply to leptons as well as quarks - an electron can be changed into a neutrino via the weak force. The $Z^{0}$ boson preserves particle type.

The switching of particles via the weak force can be described by 2x2 matrices - with $W^{\pm}$ interchanging particles and $Z^{0}$ being the identity. This is described by the $SU(2)$ group.

For the electromagnetic force - it is only mediated by one uncharged photon so this described by the $U(1)$ group.
![[Pasted image 20250228102431.png]]
Applying the flip operator to the wavefunction that describes this interaction gives
$$\hat{F}\psi(\underline{r}_{1}, \underline{r}_{2})=x\psi(\underline{r}_{2},\underline{r}_{1})$$
$$\hat{F}^2\psi(\underline{r}_{1},\underline{r}_{2})=x^2\psi(\underline{r}_{1},\underline{r}_{2}).$$
As the flip operator belong to $U(1)$, $x^2=1\implies x=\pm 1$.
This means either
$$\psi(\underline{r}_{1},\underline{r}_{2})=\psi(\underline{r}_{2},\underline{r}_{1})$$
which represents bosons or
$$\psi(\underline{r}_{1},\underline{r}_{2})=-\psi(\underline{r}_{2},\underline{r}_{1})$$
which represents fermions.