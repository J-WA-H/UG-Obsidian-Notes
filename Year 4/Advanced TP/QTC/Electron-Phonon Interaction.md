Using $c_{k},c_{k}^{\dagger}$ for creation/annihilation operators for electrons, and $a_{q},a_{q}^{\dagger}$ for phonons, 
$$H_{D}=\sum_{k}\varepsilon_{k}c_{k}^{\dagger}c_{k}\tag{18.1}+\sum_{q}\sum_{s}\hbar \omega_{qs}a_{qs}^{\dagger}a_{qs} $$
The atom is made of a nucleus and core electrons, valence electrons approximated as [[Jellium]]. There is an interaction between electrons and [phonons](Phonons%20in%203D.md) via a screened potential.

![[Pasted image 20260308145508.png]]
This configuration is the rigid-ion approximation. The potential $V_{eI}(\vec{r}-\vec{\ell}-\vec{y}_{\ell})$ gives the Hamiltonian,
$$H_{eI}=\sum_{i}\sum_{\vec{\ell}}=V_{eI}(\vec{r}_{i}-\vec{\ell}-\vec{y}_{\ell})\tag{18.2} $$
in 1st quantisation. In second quantisation,
$$H_{eI}=\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}\int d^3r\phi_{\vec{k}}^{*}(\vec{r})V_{eI}(\vec{r}-\vec{\ell}-\vec{y}_{\ell})c_{\vec{k}}c_{\vec{k}'}^{\dagger}=\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}\bra{\vec{k}} V_{eI}(\vec{r}-\vec{\ell}-\vec{y}_{\ell})\ket{\vec{k}'}c_{k}^{\dagger}c_{k'}\tag{18.2}  $$
The Fourier transformation of $V_{eI}(\vec{r})$ is
$$V_{k}=\int d^3re^{ -i\vec{k}\cdot \vec{r} }V_{eI}(\vec{r})\implies V_{eI}(\vec{r})=\frac{1}{V}\sum_{\vec{q}}V_{\vec{q}}e^{ i\vec{q}\cdot \vec{r} }\tag{18.3}. $$
This gives
$$\bra{\vec{k}} V_{eI}(\vec{r}-\vec{\ell}-\vec{y}_{\ell})\ket{\vec{k}'} =\int d^3re^{ -i\vec{k}\cdot \vec{r} }\left( \frac{1}{V}\sum_{q}V_{\vec{q}}e^{ i\vec{q}\cdot(\vec{r}-\vec{\ell}-\vec{y}_{\ell}) } \right)e^{ i\vec{k}'\cdot \vec{r} }\tag{18.4}=\frac{1}{V}\sum_{q}V_{\vec{q}}\underbrace{ \int d^3r e^{ i(\vec{q}-\vec{k}+\vec{k}')\cdot \vec{r} } }_{ V\delta_{\vec{q}-\vec{k}+\vec{k}',0} }e^{ -i\vec{q}\cdot(\vec{\ell}+\vec{y}_{\ell}) }.$$
Hence
$$H_{eI}=\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}e^{ i(\vec{k}'-\vec{k})\cdot(\vec{\ell}+\vec{y}_{\ell}) }c_{k}^{\dagger}c_{k}\tag{18.5} $$
When $e^{ i(\vec{k}-\vec{k}')\cdot \vec{y}_{\ell} }$ is small, it is $\approx 1+(\vec{k}'-\vec{k})\cdot \vec{y}_{\ell}$. $H_{eI}$ becomes
$$H_{eI}=\sum_{\ell}\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}e^{ i(\vec{k}'-\vec{k})\cdot \vec{\ell} }e^{ i(\vec{k}'-\vec{k})\cdot \vec{y}_{\ell} }c_{k}^{\dagger}c_{k'}=H_{\text{Bloch}}+H_{e-{p}}.\tag{18.6} $$
The Bloch Hamiltonian is
$$H_{\text{Bloch}}=\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}e^{ i(\vec{k}'-\vec{k})\cdot \vec{\ell} }c_{k}^{\dagger}c_{k'}=\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}c_{k}^{\dagger}c_{k'}\underbrace{ \sum_{\vec{\ell}}e^{ i(\vec{k}'-\vec{k})\cdot \vec{\ell} } }_{ N\sum_{\vec{g}}\delta_{\vec{k}'-\vec{k},\vec{g}} }.\tag{18.7} $$
This gives
$$H_{\text{Bloch}}=\sum_{\vec{k}'}V_{\vec{k}'-\vec{g}-\vec{k}'}c_{k'-g}^{\dagger}c_{\vec{k}'}=N\sum_{\vec{k},\vec{g}}V_{-\vec{g}}c_{\vec{k}-\vec{g}}^{\dagger}c_{\vec{k}}\tag{18.8} .$$
The other part gives
$$H_{e-p}=\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}e^{ i(\vec{k}-\vec{k}')\cdot \vec{\ell} }\left[ i(\vec{k}'-\vec{k}) \frac{1}{\sqrt{ N }}\sum_{q}e^{ i\vec{q}\cdot \vec{\ell} }\vec{Y}_{q} \right] c_{k}^{\dagger}c_{k'} = \frac{1}{\sqrt{ N }}\sum_{\vec{\ell}}\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}{ i(\vec{k}'-\vec{k})\cdot \vec{Y}_{q} }\sum_{\vec{\ell}}e^{ i(\vec{q}+\vec{k}'-\vec{k})\cdot \vec{\ell} }c_{k}^{\dagger}c_{k'}$$
$$=\sqrt{ N }\sum_{\vec{k},\vec{k}'}V_{\vec{k}-\vec{k}'}i(\vec{k}'-\vec{k})\cdot \vec{Y}_{\vec{k}-\vec{k}'}c_{k}^{\dagger}c_{k'}.\tag{18.9} $$
This gives
$$H_{e-p}=i\sqrt{ N }\sum_{\vec{k},\vec{k}'}\sum_{\vec{s}}[(\vec{k}'-\vec{k}) \vec{s}][\vec{s}\cdot Y_{\vec{k}-\vec{k}'}]V_{\vec{k}-\vec{k}'}c_{k}^{\dagger}c_{k'}\tag{18.10}. $$
This gives isotropic phonons. When $\vec{s}\parallel \vec{k}-\vec{k}'$, we get longitudinal phonons, and when $\vec{s}\perp \vec{k}-\vec{k}'$, we get transverse phonons.
Using creation and annihilation operators, we get
$$H_{e-p}=i\sum_{\vec{s}}\sum_{\vec{k},\vec{k}'}\sqrt{ \frac{N\hbar}{2m\omega_{\vec{k}-\vec{k}',s}} }(\vec{k}'-\vec{k})\cdot \vec{s}V_{\vec{k}-\vec{k}'}(a_{\vec{k}-\vec{k}',\vec{s}}+a^{\dagger}_{\vec{k}'-\vec{k},s})c_{k}^{\dagger}c_{k'}\tag{18.11}. $$
From $(\vec{k}'-\vec{k})\cdot \vec{s}$, only the longitudinal terms contribute to the Hamiltonian, so we get
$$H_{e-p}=\sum_{\vec{k},\vec{k}'}M_{\vec{k},\vec{k}'}(a_{\vec{k}-\vec{k}'}+a_{\vec{k}'-\vec{k}}^{\dagger})c_{k}^{\dagger}c_{k'},\qquad M_{\vec{k},\vec{k}'}=i\sqrt{ \frac{N\hbar}{2m\omega_{q}} }|\vec{k}'-\vec{k}|V_{\vec{k}-\vec{k}'}.\tag{18.12} $$
This gives the Frohlich Hamiltonian,
$$H=\sum_{\vec{k}}\varepsilon_{\vec{k}}c_{k}^{\dagger}c_{k}+\sum_{\vec{q}}\sum_{\vec{s}}\hbar \omega_{\vec{q}\vec{s}}a^{\dagger}_{\vec{q}\vec{s}}a_{\vec{q}\vec{s}}+\sum_{\vec{k},\vec{k}'}M_{\vec{k},\vec{k}'}(a^{\dagger}_{\vec{k}'-\vec{k}}+a_{\vec{k}=\vec{k}'})c_{k}^{\dagger}c_{k'}.\tag{18.13} $$
Perform a canonical transformation on the Frohlich Hamiltonian,
$$H'=e^{ -S }He^{ S }=e^{ -S }(H_{0}+H_{e-p})e^{ S }\tag{18.14} .$$
We aim to solve
$$e^{ -S }He^{ S }e^{ -S }\psi=Ee^{ -S }\psi \implies H'\psi'=E\psi'\tag{18.15}. $$
We want to determine the operator $S$. The effect of $S$ is said to be weak so
$$H'=\left( 1-S+\frac{1}{2}S^2+\dots \right)(H_{0}+H_{ep})\left( 1+S+\frac{1}{2}S^2+\dots \right)=\left( 1-S+\frac{1}{2}S^2+\dots \right)\left( H_{0}+H_{0}S+\frac{1}{2}H_{0}S^2+H_{ep}+H_{ep}S+\frac{1}{2}H_{ep}S^2\right)$$
$$=H_{0}+H_{0}S+\frac{1}{2}H_{0}S^2+H_{ep}+H_{ep}S+\frac{1}{2}H_{ep}S^2-SH_{0}-SH_{0}S-SH_{ep}-SH_{ep}S+\frac{1}{2}S^2H_{0}+\frac{1}{2}S^2H_{ep}+\mathcal{O}(S^3)\tag{18.16}$$
$$=H_{0}+[H_{0},S]+H_{ep}+[H_{ep},S]+\frac{1}{2}(H_{0}S^2-2SH_{0}S+S^2H_{0})+\dots$$
Ignore the terms with $S^2$ and $H_{ep}$ and $H_{ep}\sim S$. Choose $S$ s.t. $[H_{0},S]+H_{ep}=0$ so $H_{ep}=-(H_{0}S-SH_{0})$. Try the nested commutator,
$$[[H_{0},S],S]=(H_{0}S-SH_{0})S-S(H_{0}S-SH_{0})=H_{0}S^2-2SH_{0}S+S^2H_{0}\tag{18.17} $$
which gives
$$H'=H_{0}+[H_{ep},S]+\frac{1}{2}[[H_{0},S],S]\tag{18.18}. $$
Given $H_{ep}=-[H_{0},S]$, we get
$$H'=H_{0}-[[H_{0},S],S]+\frac{1}{2}[[H_{0},S],S]=H_{0}+\frac{1}{2}[H_{ep},S].\tag{18.19} $$
