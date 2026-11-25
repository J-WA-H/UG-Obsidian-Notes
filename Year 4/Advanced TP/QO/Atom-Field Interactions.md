Consider an atom in [[Classical EM Fields]]. The dynamics of an atomic valence electron with external fields is given by the Hamiltonian
$$H=\frac{1}{2m}(-i\hbar \vec{\nabla}+q\vec{A})^2+V(r)-q\phi \tag{7.1}. $$The fields are described classically and the particle is described quantum mechanically so the model is semi-classical.
The fields have gauge symmetries where
$$\phi'=\phi-\frac{\partial \chi}{\partial t},\;\vec{A}'=\vec{A}+\vec{\nabla}\chi.\tag{7.2} $$
Define the transformed wavefunction $\ket{\psi'}=\hat{U}\ket{\psi}$ where $i\hbar \frac{d\ket{\psi}}{dt}=\hat{H}\ket{\psi}$. There is a corresponding transformed Hamiltonian defined through
$$i\hbar \frac{d\ket{\psi'}}{dt}=\hat{H}'\ket{\psi}.\tag{7.3}  $$
The equation of motion is then defined for the transformed wavefunction,
$$i\hbar \frac{d\ket{\psi'}}{dt}=\hat{U}i\hbar \frac{d\ket{\psi}}{dt}+{i\hbar} \frac{d\hat{U}}{dt}\ket{\psi} =\left( \hat{U}\hat{H}+i\hbar \frac{d\hat{U}}{dt} \right)\hat{U}^{\dagger}\ket{\psi'}\tag{7.4}  $$
$$\implies \hat{H}'=\left( \hat{U}\hat{H}\hat{U}^{\dagger}+i\hbar \frac{d\hat{U}}{dt}\hat{U}^{\dagger} \right).\tag{7.5} $$
In position space, consider $\psi'(\vec{r},t)=U(\vec{r},t)\psi(\vec{r},t)$ where $U(\vec{r},t)=e^{ iq\chi(\vec{r},t)/\hbar }$ and $\chi$ is a gauge function.
$$U(-i\hbar \vec{\nabla})U^{*}=-i\hbar \vec{\nabla}+q\vec{\nabla}\chi \tag{7.6} $$
$$i\hbar \frac{\partial U}{\partial t}U^{*}=q \frac{\partial \chi}{\partial t}.\tag{7.7} $$
The transformed Hamilton is then
$$H=\frac{1}{2m}(-i\hbar \vec{\nabla}+q\vec{A}'(\vec{r},t))^2+V(r)-q\phi'(\vec{r},t).\tag{7.8} $$
Impose the Coulomb gauge, $\vec{\nabla}\cdot \vec{A}=0$, $\phi=0$ and impose dipole approximation (spatially invariant $\vec{A}$ and $\vec{E}$).
$$H(\vec{r},t)=\frac{1}{2m}[-i\hbar \vec{\nabla}+q\vec{A}(t)]^2+V(r).\tag{7.9} $$
Introduce length gauge function $\chi=\vec{A}(t)\cdot \vec{r}\therefore U(\vec{r},t)=e^{ -iq\vec{A}(t)\cdot \vec{r}/\hbar }$.
$$\therefore\vec{\nabla}\chi=-\vec{A}\tag{7.10} $$
$$\frac{\partial \chi}{\partial t}=\vec{r}\cdot \frac{\partial \vec{A}}{\partial t}=-\vec{r}\cdot \vec{E}.\tag{7.11} $$
This gives the transformed Hamiltonian
$$H'(\vec{r},t)=-\frac{\hbar^2\nabla^2}{2m}+V(r)-\vec{d}\cdot \vec{E}(t)\tag{7.12} $$where $\vec{d}=-q\vec{r}$ is the dipole moment. This is the most common form of the Hamiltonian.

The creation and annihilation operators describing $\hat{A},\hat{E}$ act in a different state space to the atomic $\hat{r},\hat{p}$ operators. Therefore atomic and electromagnetic field operators commute.
The manipulations to achieve the dipole approximation Hamiltonian are therefore essentially unchanged.

For a single field mode, consider 3 Hamiltonians, $\hat{H}=\hat{H}_{A}+\hat{H}_{F}+\hat{H}_{c}$ where $\hat{H}_{A}$ is the atomic Hamiltonian,
$$\hat{H}_{A}=\frac{\hat{p}^2}{2m}+V(\hat{r})\tag{7.13}, $$$\hat{H}_{F}$ is the field Hamiltonian,
$$\hat{H}_{F}=\hbar \omega \hat{a}^{\dagger}\hat{a},\tag{7.14} $$and $\hat{H}_{c}$ is the atom-field coupling Hamiltonian,
$$\hat{H}_{c}=-\hat{d}\cdot \mathcal{\vec{E}}_{0}(\hat{a}-\hat{a}^{\dagger})\tag{7.15} $$where $\mathcal{\vec{E}}_{0}$ is some polarisation vector with$$|\mathcal{\vec{E}}_{0}|=i\sqrt{\frac{\hbar\omega}{2\varepsilon_{0}V} }.\tag{7.16} $$
We can transform $\hat{H}$ via $\hat{U}=e^{ i\hat{H}_{F}t/\hbar }$ to get
$$\hat{H}'=\frac{\hat{p}^2}{2m}+V(\hat{r})-\hat{d}\cdot \mathcal{\vec{E}}_{0}(\hat{a}e^{ -i\omega t }-\hat{a}^{\dagger}e^{ i\omega t })\tag{7.17} $$where $e^{ i\hat{a}^{\dagger}\hat{a}\omega t }\hat{a}e^{ -i\hat{a}^{\dagger}\hat{a}\omega t }=\hat{a}e^{ -i\omega t }$.
We can more directly compare this to the semi-classical description with classical EM fields.

Construct a basis $\ket{\psi_{j},n}=\ket{\psi_{j}}\ket{n}$ from eigenstates $\ket{\psi_{j}}$ of $\hat{H}_{A}$ and $\ket{n}$ of $\hat{H}_{F}$. The joint state is an eigenstate of $\hat{H}_{A}+\hat{H}_{F}$, with eigenvalues $E_{j}+\hbar \omega n$. Note that $\hat{H}_{c}$ changes photon number by $\pm{1}$ only so from an initial state $\ket{\psi_{a},n}$, the only possible couplings are to states $\ket{\psi_{b},n\pm 1}$. This gives that the only non-zero matrix elements of $\hat{H}_{c}$ are
$$\bra{\psi_{b},n-1}\hat{H}_{c}\ket{\psi_{a},n} =-\vec{d}_{ba}\cdot \mathcal{\vec{E}}_{0}\sqrt{ n } \tag{7.17} $$
$$\bra{\psi_{b},n+1} \hat{H}_{c}\ket{\psi_{a},n} =-\vec{d}_{ba}\cdot \mathcal{\vec{E}}_{0}\sqrt{ n+1 }.\tag{7.18} $$
Here $\vec{d}_{ba}=\bra{\psi_{b}}\hat{d}\ket{\psi_{a}}$ is the dipole matrix element.

Coupling also occurs when $n=0$, this is spontaneous emission. We can recast $\hat{H}_{A}$ in terms of its eigenvalues,
$$\hat{H}_{A}=\sum_{j}E_{j}\ket{\psi_{j}} \bra{\psi_{j}}\tag{7.19}  .$$
Similarly, 
$$\hat{d}\cdot \mathcal{\vec{E}}_{0}=\sum_{j\neq j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}}\bra{\psi_{j}}  .\tag{7.20} $$Within a frame defined by $\hat{U}=e^{ i\hat{H}_{F}t/\hbar }$,
$$\hat{H}'=\sum_{j}E_{j}\ket{\psi_{j}} \bra{\psi_{j}}-\sum_{j\neq j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j}}(\hat{a}e^{ -i\omega t }-\hat{a}^{\dagger}e^{ i\omega t })  .\tag{7.21} $$
Transforming $\hat{H}'$ via $\hat{U}_{A}=e^{ i\hat{H}_{A}t/\hbar }$ moves into the interaction picture,
$$\hat{H}_{I}=-\sum_{j\neq j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}e^{ -i(\omega-\omega_{jj'})t } + \sum_{j\neq j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}^{\dagger}e^{ -i(\omega+\omega_{jj'})t } \tag{7.22} $$where
$$\omega_{jj'}=\frac{E_{j}-E_{j'}}{\hbar}.\tag{7.23} $$
This gives the rotating wave approximation,
$$\hat{H}_{I}=-\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}e^{ -i(\omega-\omega_{jj'})t} +\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}^{\dagger}e^{ i(\omega-\omega_{jj'})t}-\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}e^{ -i(\omega+\omega_{jj'})t}+\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}^{\dagger}e^{ i(\omega+\omega_{jj'})t}$$
$(7.24)$.
The approximation eliminates rapidly rotating $e^{ i(\omega+\omega_{jj'}) t}$ terms. These average to zero on any time scale of interest. This is equally valid within semiclassical description for an external field oscillating with frequency $\omega$.
$$\hat{H}_{I}=-\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}e^{ -i(\omega-\omega_{jj'})t} +\sum_{j> j'}\vec{d}_{jj'}\cdot \mathcal{\vec{E}}_{0}\ket{\psi_{j}} \bra{\psi_{j'}}\hat{a}^{\dagger}e^{ i(\omega-\omega_{jj'})t}\tag{7.25}. $$
The interaction picture changes from less to more/more to less energetic state associated with absorption/emission of a photon.
