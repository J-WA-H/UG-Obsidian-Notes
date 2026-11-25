The Hamiltonian for a system of electrons and nuclei is ($i$ enumerates electrons and $\alpha$ counts nuclei),
$$H(\{ \vec{r}_{i},\vec{p}_{i};\vec{R}_{\alpha},\vec{P}_{\alpha} \})=-\frac{1}{2}\sum_{i}\nabla_{i}^2+\frac{1}{2}\sum_{i\neq j} \frac{1}{|\vec{r}_{i}-\vec{r}_{j}|}-\sum_{i,\alpha} \frac{Z_{\alpha}}{|\vec{r}_{i}-\vec{R}_{\alpha}|}-\sum_{\alpha} \frac{1}{2M_{\alpha}}\nabla^2_{\alpha}+\frac{1}{2}\sum_{\alpha\neq\beta} \frac{Z_{\alpha}Z_{\beta}}{|\vec{R}_{\alpha}-\vec{R}_{\beta}|}\tag{2.1}. $$
This makes use of atomic units $m=|e|=\hbar=4\pi\varepsilon_{0}=1$. The aim is to solve
$$H(\{ \vec{r}_{i},\vec{p}_{i};\vec{R}_{\alpha},\vec{P}_{\alpha} \})\psi(\vec{r}_{1},\dots ,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})=E\psi(\vec{r}_{1},\dots,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})\tag{2.2}. $$
However, for a large atom, solving this is impossible. There is a large difference in the mass between electrons and nuclei$$\frac{m}{M_{
\alpha}}=\frac{1}{M_{\alpha}}\ll 1\;\forall\;M_{\alpha}\tag{2.3}. $$The Born-Oppenheimer (adiabatic) approximation sets the nuclear kinetic energy operator to zero
$$H(\{ \vec{r}_{i},\vec{p}_{i};\vec{R}_{\alpha},\vec{P}_{\alpha} \})=-\frac{1}{2}\sum_{i}\nabla_{i}^2+\frac{1}{2}\sum_{i\neq j} \frac{1}{|\vec{r}_{i}-\vec{r}_{j}|}-\sum_{i,\alpha} \frac{Z_{\alpha}}{|\vec{r}_{i}-\vec{R}_{\alpha}|}+\frac{1}{2}\sum_{\alpha\neq\beta} \frac{Z_{\alpha}Z_{\beta}}{|\vec{R}_{\alpha}-\vec{R}_{\beta}|}\tag{2.4}. $$
This is an electronic only Hamiltonian. It depends only on the nuclear positions so nuclei are frozen. 

Consider the 1D harmonic oscillator with this approximation
$$-\cancelto{0}{\frac{1}{2M} \frac{d\phi}{dx}}+\frac{1}{2}k^2x^2\phi=E\phi.\tag{2.5} $$This is solved with $\phi(x)=\sqrt{ \delta(x-x_{0}) }$ so $\int_{-\infty}^\infty |\phi(x)|^2dx=1$. This has an infinite kinetic energy so these results are not physical, so are not in the Hilbert space. Applying this to the BO approximation shows that the BO solutions are not in the full Hilbert space pf the atom. but are in the Hilbert space for just electrons.

To find the solutions, we find the eigenfunctions of the BO Hamiltonian. These are electronic only wavefunctions,
$$H_{[R_{\alpha}]}\Phi_{R_{1},\dots,R_{N_{n}},k}(\vec{r}_{1},\dots ,\vec{r}_{N})=\varepsilon_{k}(\vec{R}_{1},\dots,\vec{R}_{N_{n}})\Phi_{R_{1},\dots ,R_{N_{n}},k}(\vec{r}_{1},\dots,\vec{r}_{N})\tag{2.6} $$with $k\in \mathbb{N}$. Because $\Phi_{R_{1},\dots R_{N_{n}},k}$ are electronic states, their norm is
$$\braket{ \Phi_{R_{1},\dots,R_{N_{n}},k} | \Phi_{R_{1},\dots,R_{N_{n}},k} } =\int d^3r_{1}\int d^3r_{2}\dots \int d^3r_{N}|\Phi_{R_{1},\dots ,R_{N_{n}},k}(\vec{r}_{1},\dots,\vec{r}_{N})|^2=1\;\forall\;R_{i}\tag{2.7}. $$
This is the first step in the Born-Oppenheimer approximation.

The second step is approximating just the ground state.
$$\psi^{BO}(\vec{r}_{1},\dots ,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})=\Phi_{R_{1},\dots ,R_{N_{n}},k}(\vec{r}_{1},\dots,\vec{r}_{N})\chi(\vec{R}_{1},\dots,\vec{R}_{N_{n}})\tag{2.8} $$but we do not know $\chi$ so we use Rayleigh-Ritz to determine it
$$\int dR^{3N_{n}}\int dr^{3N}\psi^{BO\,*}(\vec{r}_{1},\dots,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})H\psi^{BO}(\vec{r}_{1},\dots,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})-\lambda \int dR^{3N_{n}}\int dr^{3N}|\psi^{BO}|^2\tag{2.9}. $$
Using
$$|\psi^{BO}(\vec{r}_{1},\dots ,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})|^2=|\Phi_{R_{1},\dots ,R_{N_{n}},k}(\vec{r}_{1},\dots,\vec{r}_{N})|^2|\chi(\vec{R}_{1},\dots,\vec{R}_{N_{n}})|^2\tag{2.10} $$
and $$\int d^{3N_{n}}R\int d^{3N}r =\int d^3R_{1}\int d^3R_{2}\dots \int d^3R_{N_{n}}\int d^3r_{1}\int d^3r_{2}\dots \int d^3r_{N}\tag{2.11} .$$
This gives $$\int d^{3N_{n}}R\int d^{3N}r|\psi^{BO}(\vec{r}_{1},\dots ,\vec{r}_{N};\vec{R}_{1},\dots,\vec{R}_{N_{n}})|^2=|\Phi_{R_{1},\dots ,R_{N_{n}},k}(\vec{r}_{1},\dots,\vec{r}_{N})|^2|\chi(\vec{R}_{1},\dots,\vec{R}_{N_{n}})|^2=\int d^3R_{1}\dots \int d^3R_{N_{n}}|\chi|=1.\tag{2.12} $$
This shows that $\chi$ is normalised to 1. Now return to the minimisation,
$$\int d^3R_{1}\dots \int d^3R_{N_{n}}\chi ^{*}\int d^3r_{1}\dots\int d^3r_{N}\Phi ^{*}_{R_{1},\dots,R_{N_{n}}}\left[ -\sum_{\alpha} \frac{\nabla^2_{\alpha}}{2M_{\alpha}} \right]\Phi_{R_{1},\dots,R_{N_{n}}}\chi-\lambda \int d^3R_{1}\dots \int d^3R_{N_{N}}|\chi|^2 \tag{2.13} .$$
Using $H_{[R_{\alpha}]}\Phi_{R_{1},\dots,R_{N_{n}}}(r_{1},\dots,r_{N})=\varepsilon_{0}(R_{1},\dots R_{N_{n}})\Phi_{R_{1},\dots,R_{N_{n}}}(r_{1},\dots,r_{N})$, minimise with respect to $\chi$.
$$\int d^3R_{1}\dots \int d^3R_{N_{n}}\chi ^{*}\int d^3r_{1}\dots\int d^3r_{N}\Phi ^{*}_{R_{1},\dots,R_{N_{n}}}\left[ -\sum_{\alpha} \frac{\nabla^2_{\alpha}}{2M_{\alpha}}+H_{[R_{\alpha}]} \right]\Phi_{R_{1},\dots,R_{N_{n}}}\chi-\lambda \int d^3R_{1}\dots \int d^3R_{N_{N}}|\chi|^2 \tag{2.14} .$$
Note $\nabla^2\Phi_{R_{1},\dots,R_{N_{n}}}\chi=\chi(\nabla^2_{\alpha}\Phi_{R_{1},\dots,R_{N_{n}}})+\Phi_{R_{1},\dots,R_{N_{n}}}\nabla^2_{\alpha}\chi+2(\vec{\nabla}_{\alpha}\cdot \Phi_{R_{1},\dots,R_{N_{n}}})(\vec{\nabla}_{\alpha}\cdot \chi)$. This gives$$\left[ -\sum_{\alpha} \frac{\nabla^2_{\alpha}}{2M_{\alpha}}+\varepsilon_{0}(R_{1},\dots,R_{N_{n}})+\sum_{\alpha} \frac{\int |\vec{\nabla}_{\alpha}\Phi_{R_{1},\dots,R_{N_{n}}}|^2d^3r_{1}\dots d^3r_{N}}{2M_{\alpha}} \right]\chi(R_{1},\dots,R_{N_{n}})=E\chi(R_{1},\dots,R_{N_{n}}) \tag{2.15} .$$
This is the effective equation for $\chi$ in the Born-Oppenheimer approximation.  Normally, the operator $\nabla_{\alpha}^2\Phi_{R_{1},\dots,R_{N_{n}}}$ is small, so has a weak effect, so it is normally set to zero.
$$\left[ -\sum_{\alpha} \frac{\nabla^2_{\alpha}}{2M_{\alpha}}+\varepsilon_{0}(R_{1},\dots,R_{N_{n}}) \right]\chi(R_{1},\dots,R_{N_{n}})=E\chi(R_{1},\dots,R_{N_{n}})\tag{2.16}. $$
This is a Schrodinger-like equation for $\chi$ in the Born-Oppenheimer approximation. Classically, we can take the potential energy to the nuclei $\varepsilon_{0}(R_{1},\dots,R_{N_{n}})$ to find the forces $\vec{F}=-\vec{\nabla}_{\alpha}\varepsilon_{0}$.
