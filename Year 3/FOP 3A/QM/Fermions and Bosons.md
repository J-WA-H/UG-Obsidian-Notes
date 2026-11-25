As $\Psi(1,2)$ is an eigenfunction of $\hat{P}_{12}$, we can find the properties of the wavefunctions for bosons and fermions under interchange.
[Bosons](Two%20Particle%20Systems.md) ($\lambda=1$):
$$\hat{P}_{12}\Psi(1,2)=\Psi(1,2)$$
This implies $\Psi$ is symmetric under interchange.

Fermions ($\lambda=-1$):
$$\hat{P}_{12}\Psi(1,2)=-\Psi(1,2)$$
This implies $\Psi$ is antisymmetric under interchange.
For two identical fermions, $\Psi(1,1)=-\Psi(1,1)\implies \Psi(1,1)=0$ which shows the Pauli exclusion principle.
Consequences:
Omit spin and ignore all interactions between the two particles. The wavefunctions for the particles are given by $\phi_1(\underline{r})$, $\phi_{2}(\underline{r})$.
For bosons:
$$\psi(\underline{r},\underline{r}')=\frac{1}{\sqrt{ 2 }}(\phi_{1}(\underline{r})\phi_{2}(\underline{r}')+\phi_{1}(\underline{r}')\phi_{2}(\underline{r})).$$
For fermions:
$$\psi(\underline{r},\underline{r}')=\frac{1}{\sqrt{ 2 }}(\phi_{1}(\underline{r})\phi_{2}(\underline{r}')-\phi_{1}(\underline{r}')\phi_{2}(\underline{r})).$$
Here we can see that the wavefunction for bosons is symmetric and for fermions it is antisymmetric.
For a classical system: $$\psi_{cl}(\underline{r},\underline{r}')\propto \phi_{1}(\underline{r})\phi_{2}(\underline{r}')\text{ or } \psi_{cl}(\underline{r},\underline{r}')\propto \phi_{1}(\underline{r}')\phi_{2}(\underline{r}).$$
The wavefunction for classical particles don't need to be symmetric/antisymmetric as the particles can be labelled individually.

Can 2 particles have the same single particle state?
$$\lambda=1,\;\psi_{+1}(\underline{r},\underline{r}')\propto 2\phi(\underline{r})\phi(\underline{r}')=2\psi_{cl}(\underline{r},\underline{r}')$$
$$\lambda=-1\;\psi_{-1}(\underline{r},\underline{r}')\propto \phi(\underline{r})\phi(\underline{r}')-\phi(\underline{r}')\phi(\underline{r})=0$$
hence, two bosons can occupy the same state but two fermions cannot.
This translates to the probabilities of finding these states in the same position:
$$Pr(\psi_{+}(\underline{r},\underline{r}))=\lvert \psi_{+}(\underline{r},\underline{r}) \rvert^2 =\left\lvert  \frac{1}{\sqrt{ 2 }}(\phi_{1}(\underline{r})\phi_{2}(\underline{r})+\phi_{2}(\underline{r})\phi_{1}(\underline{r}))  \right\rvert^2=2\lvert \phi_{1}(\underline{r}) \rvert^2\lvert \phi_{2}(r) \rvert^2=2\lvert \psi_{cl}(\underline{r},\underline{r}) \rvert^2 $$
$$Pr(\psi_{-}(\underline{r},\underline{r}))=\lvert \psi_{-}(\underline{r},\underline{r}) \rvert^2=\left\lvert  \frac{1}{\sqrt{ 2 }}(\phi_{1}(\underline{r})\phi_{2}(\underline{r})-\phi_{2}(r)\phi_{1}(\underline{r}))  \right\rvert^2=0$$
This shows that two fermions cannot occupy the same quantum state (Pauli exclusion). The vanishing probability can be seen as an effective repulsion, that is a quantum mechanical effect rather than a real force. In the bosonic case the probability of finding 2 particles in the same position in space is double that for distinguishable particles, so there is an effective attraction.

This effective attraction/repulsion is known as an exchange force.