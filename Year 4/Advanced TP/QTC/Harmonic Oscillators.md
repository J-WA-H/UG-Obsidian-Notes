For [bosons](Boson%202nd%20Quantisation.md), we have the Hamiltonian
$$H=\sum_{k}\varepsilon_{k}a_{k}^{\dagger}a_{k}=\sum_{i}\varepsilon_{i}\hat{n}_{i}\tag{14.1} .$$
For free bosons, $\phi_{i}(\vec{r})=V^{-1/2}\exp[i\vec{k}\cdot \vec{r}]$, and $\varepsilon_{k}=\frac{\hbar^2k^2}{2m}$.

For fermions, the number of particles $N$ is constant in time, but not for bosons, e.g. the number of phonons increases by raising temperature because vibrations with higher energies are excited. In other systems, like ${}^{4}_{2}He$, $N$ is conserved and they behave like pseudo-bosons as the quasiparticles are approximately described by boson commutation relations.

Example: 3D simple harmonic oscillator,
$$H_{0}=\left( \frac{1}{2}p_{x}^2+\frac{1}{2}\omega_{x}^2x^2 \right)+\left( \frac{1}{2}p_{y}^2+\frac{1}{2}\omega_{y}^2y^2 \right)+\left( \frac{1}{2}p_{z}^2+\frac{1}{2}\omega_{z}^2z^2 \right)\tag{14.2}. $$
We have the commutation relations
$$[x,p_{x}]=[y,p_{y}]=[z,p_{z}]=i\tag{14.3}.$$
Define creation and annihilation operators
$$a_{x}=\frac{1}{\sqrt{ 2\omega_{x} }}(\omega_{x}x+ip_{x}),\;a_{x}^{\dagger}=\frac{1}{\sqrt{ 2\omega_{x} }}(\omega_{x}x-ip_{x})\tag{14.4}. $$
This gives 
$$x=\frac{{a_{x}+a_{x}^{\dagger}}}{\sqrt{ 2\omega_{x} }},\qquad ip_{x}=\sqrt{ \frac{\omega_{x}}{2} }(a_{x}-a_{x}^{\dagger})\tag{14.5} $$
From this,
$$\frac{\omega_{x}^2}{2}x^2=\frac{\omega_{x}^2}{2} \frac{1}{2\omega_{x}}(a_{x}+a_{x}^{\dagger})^2=\frac{\omega_{x}}{4}(a_{x}^2+(a_{x}^{\dagger})^2+a_{x}a_{x}^{\dagger}+a_{x}^{\dagger}a_{x})$$
$$-\frac{1}{2}p_{x}^2=\frac{\omega_{x}}{4}(a_{x}-a_{x}^{\dagger})^2=\frac{\omega_{x}}{4}(a_{x}^2+(a_{x}^{\dagger})^2-a_{x}a_{x}^{\dagger}-a_{x}^{\dagger}a_{x})\tag{14.6} $$
$$\implies \frac{1}{2}p_{x}^2+\frac{1}{2}\omega_{x}^2x^2=\frac{\omega_{x}}{4}(2a_{x}a_{x}^{\dagger}+2a_x^{\dagger}a_{x})\tag{14.7} .$$Using the commutator relation $[a_{x},a_{x}^{\dagger}]=1$,
$$\frac{1}{2}p_{x}^2+\frac{1}{2}\omega_{x}^2x^2=\frac{\omega_{x}}{2}(1+2a_{x}^{\dagger}a_{x})=\omega_{x}\left( a_{x}^{\dagger}a_{x}+\frac{1}{2} \right)\tag{14.8}. $$
This gives the full Hamiltonian
$$H_{0}=\omega_{x}\left( a_{x}^{\dagger}a_{x}+\frac{1}{2} \right)+\omega_{y}\left( a_{y}^{\dagger}a_{y}+\frac{1}{2} \right)+\omega_{z}\left( a_{z}^{\dagger}a_{z}+\frac{1}{2} \right)\tag{14.9}=\sum_{i=1}^{3}\omega_{i}\left( a_{i}^{\dagger}a_{i}+\frac{1}{2} \right). $$
When $\omega_{i}=\omega$, 
$$H_{0}=\omega \sum_{i=1}^{3}\left( a_{i}^{\dagger}a_{i}+\frac{1}{2} \right)\tag{14.10}. $$
This commutes with the number operator.

The boson quantum state with quantum numbers $n_{x},n_{y},n_{z}$ gives
$$\ket{n_{x},n_{y},n_{z}}=A(a_{x}^{\dagger})^{n_{x}}(a_{y}^{\dagger})^{n_{y}}(a_{z}^{\dagger})^{n_{z}}\ket{n_{x},n_{y},n_{z}}\tag{14.11}    $$
Applying the Hamiltonian gives
$$\sum_{i=1}^{3}\left( a_{i}^{\dagger}a_{i}+\frac{1}{2} \right)\omega \ket{n_{x},n_{y},n_{z}}=E_{n_{x},n_{y},n_{z}} \tag{14.12} \ket{n_{x},n_{y},n_{z}} .$$
The energy is
$$E_{n_{x},n_{y},n_{z}}=(n_{x}+n_{y}+n_{z})\omega \tag{14.13} .$$
Another example is the anharmonic oscillator,
$$H=H_{0}+\beta x^3\tag{14.14}, $$
$$\beta x^3=\beta  \frac{1}{(2\omega_{x})^{3/2}}(a_{x}+a_{x}^{\dagger})^{3}.\tag{14.15} $$
This gives the total Hamiltonian
$$H=\omega_{x}\left( a_{x}^{\dagger}a_{x}+\frac{1}{2} \right)+\omega_{y}\left( a_{y}^{\dagger}a_{y}+\frac{1}{2} \right)+\omega_{z}\left( a_{z}^{\dagger}a_{z}+\frac{1}{2} \right)+\frac{\beta}{(2\omega_{x})^{3/2}}(a_{x}+a_{x}^{\dagger})^3\tag{14.16}. $$
This Hamiltonian does not commute with the number operator.

