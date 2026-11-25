Light intensity is measured by detecting photons. Consider a single atom idealised detector, absorbed light ionises the atom and the resulting photoelectron is detected.

It is often convenient to divide the [quantised electric field](Creation%20and%20Annihilation%20Operators.md) into positive and negative frequency parts,
$$\hat{E}(\vec{r})=\hat{E}^{+}(\vec{r})+\hat{E}^{-}(\vec{r})\tag{11.1} $$
$$\hat{E}^{+}(\vec{r})=i\sum_{\vec{k},s}\sqrt{ \frac{\hbar \omega_{k}}{2\varepsilon_{0}V} }\vec{e}_{\vec{k}s}\hat{a}_{\vec{k}s}e^{ i\vec{k}\cdot \vec{r} }\tag{11.2} $$
Assuming the [dipole coupling Hamiltonian](Atom-Field%20Interactions.md) $\hat{H}_{c}$.

Absorptive transitions from an atom and field state $\ket{I}=\ket{g}\ket{i}$ to $\ket{F}=\ket{e}\ket{f}$ must involve a photon annihilation, hence
$$\bra{F} \hat{H}_{c}\ket{I}=-\bra{e} \hat{d}\ket{g} \cdot \bra{f} \hat{E}^{+}(\vec{r})\ket{i} \tag{11.3} $$
For the field transition probability, the key consideration in photodetectors is essentially 
$$|\bra{f} \hat{E}^{+}(\vec{r})\ket{i} |^2=\bra{i} \hat{E}^{-}(\vec{r})\ket{f} \cdot \bra{f} \hat{E}^{+}(\vec{r})\ket{i} \tag{11.4}.$$Summing over all possible final states gives
$$\sum_{i}\bra{i} \hat{E}^{-}(\vec{r})\ket{f} \cdot \bra{f} \hat{E}^{+}(\vec{r})\ket{i} =\bra{i} \hat{E}^{-}(\vec{r})\ket{i} \tag{11.5} .$$
The initial field state is not generally perfectly known so describe the probability of detection more generally in terms of the field [[Density Operators]],$$\mathrm{Tr}(\rho_{F}\hat{E}^{-}(\vec{r},t)\cdot\hat{E}(\vec{r},t)).\tag{11.6} $$Here we are working in the Heisenberg picture.

Simplify to a single polarisation and $x=\vec{r},t$, we define the quantum first order correlation function,
$$G^{(1)}(x_{1},x_{2})=\mathrm{Tr}[\rho_{F}\hat{E}^{-}(x_{1})\hat{E}^{+}(x_{2})]\tag{11.7}. $$
Here $G^{(1)}(x,x)$ is the intensity of light $I(\vec{r},t)$ at $x=\vec{r},t$.

We obtain an expression similar to the [classical case](Coherence%20Functions.md) for light intensity on the screen in Youngs double slits,
$$I(\vec{r})=G^{(1)}(x,x)=|K_{1}|^2G^{(1)}(x_{1},x_{1})+|K_{2}|^2G^{(1)}(x_{2},x_{2})+2\mathrm{Re}[K_{1}^{*}K_{2}G^{(1)}(x_{1},x_{2})]\tag{11.8}. $$
The normalised quantum coherence function is
$$g^{(1)}(x_{1},x_{2})=\frac{G^{(1)}(x_{1},x_{2})}{\sqrt{ G^{(1)}(x_{1},x_{1})G^{(1)}(x_{2},x_{2}) }}\tag{11.9} .$$
$|g^{(1)}(x_{1},x_{2})|=1$: complete coherence
$|g^{(1)}(x_{1},x_{2})|=0$: complete incoherence
$0<|g^{(1)}(x_{1},x_{2})|<1$: partial coherence.

Consider a single mode plane wave field $\hat{E}^{+}(x)=iK\hat{a}e^{ i(\vec{k}\cdot \vec{r}-\omega t) }$. The field is in a number state $\ket{n}$.
$$G^{(1)}(x_{1},x_{1})=G^{(1)}(x_{2},x_{2})=K^2n\tag{11.10} $$
$$G^{(1)}(x_{1},x_{2})=K^2ne^{ i\vec{k}\cdot[\vec{r}_{1}-\vec{r}_{2}]-\omega[t_{1}-t_{2}] }\tag{11.11} $$$|g^{(1)}(x_{1},x_{2})|=1$: complete coherence which is the same as the classical case.