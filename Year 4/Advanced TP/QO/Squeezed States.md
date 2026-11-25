The [squeeze operator](Quadrature%20Squeezing.md) creates and annihilates photons in pairs. Squeezing moves some uncertainty to a different state. 

The squeezed vacuum decomposition into number states is
$$\ket{\xi} =\sum_{s=0}^{\infty}C_{2s}\ket{2s}\tag{16.1}  .$$
From $(15.19)$,
$$[(\hat{a}-\alpha)\cosh(r)+(\hat{a}-\alpha ^{*})e^{ i\theta }\sinh(r)]\ket{\alpha,\xi} =0\tag{15.19} .$$Hence, $\ket{\alpha,\xi}$ is an eigenstate of $\hat{a}\cosh(r)+\hat{a}^{\dagger}e^{ i\theta }\sinh(r)$ with eigenvalue
$$\alpha \cosh(r)+\alpha ^{*}e^{ i\theta }\sinh(r)\tag{16.2}. $$
Set $\cosh(r)=\mu$, $e^{ i\theta }\sinh(r)=\nu$ in the eigenstate equation
$$(\mu \hat{a}+\nu \hat{a}^{\dagger})\ket{\xi} =(\mu \hat{a}+\nu \hat{a}^{\dagger})\sum_{s=0}^{\infty}C_{2s}\ket{2s} =0\tag{16.3}. $$
The number state decomposition is then
$$\sum_{s=0}^{\infty}[\mu \sqrt{ 2s }C_{2s}\ket{2s-1} +\nu \sqrt{ 2s+1 }C_{2s}\ket{2s+1} ]=0.\tag{16.4} $$
Equating the coefficients for $\ket{2s+1}$ yields
$$C_{2s+1}=-\frac{\nu}{\mu}\sqrt{ \frac{{2s+1}}{2s+2} }C_{2s}\tag{16.5}. $$In particular,
$$C_{2}=-\frac{\nu}{\mu}\sqrt{ \frac{1}{2} }C_{0}\tag{16.6} $$and in general
$$C_{2s}=\left( -\frac{\nu}{\mu} \right)^{s} \frac{\sqrt{ (2s)! }}{s!}C_{0}\tag{16.7}. $$
To normalise this, sum over all populations
$$\sum_{s=0}^{\infty}|C_{2s}|^2=|C_{0}|^2\sum_{s=0}^{\infty} \left\lvert  \frac{\nu}{\mu}  \right\rvert \frac{(2s)!}{(2^{s}s!)^2}=\frac{|c_{0}|^2}{\sqrt{ 1-\left\lvert  \frac{\nu}{\mu}  \right\rvert ^2 }}=1.\tag{16.8} $$
This makes use of the Taylor expansion
$$(1-x)^{-1/2}=\sum_{s=0}^{\infty}x^{s}\left[ \frac{(2s)!}{(2^{s}s!)^{2}} \right]\tag{16.9} .$$
Note that $1-\left\lvert  \frac{\nu}{\mu}  \right\rvert^2=1-\tanh^2(r)=\frac{1}{\cosh^2(r)}$.

Hence, the squeezed vacuum state is
$$\ket{\xi} =\frac{1}{\sqrt{ \cosh(r) }} \sum_{s=0}^{\infty}\left[ \frac{{e^{ i\theta }\tanh(r)}}{2} \right](-1)^{s} \frac{\sqrt{ (2s)! }}{s!}\ket{2s}\tag{16.10}  $$and
$$\ket{\alpha,\xi} =\frac{1}{\sqrt{ \cosh(r) }}\exp\left( \frac{{-|\alpha|^2-\alpha ^{*}e^{ i\theta }\tanh(r)}}{2} \right)\sum_{n=0}^{\infty}\left[ \frac{e^{ i\theta }\tanh(r)}{2} \right]^{n/2} \frac{1}{\sqrt{ n! }}H_{n}\left( \frac{\alpha e^{ i\theta }}{\sqrt{ 2\tanh(r) }}+\alpha ^{*}e^{ -i\theta/2 }\sqrt{ \frac{\tanh(r)}{2} } \right)\ket{n} \tag{16.11}. $$
$H_{n}$ is a Hermite polynomial and for $\alpha=0$,
$$H_{2s}(0)=(-1)^{s} \frac{(2s)!}{s!},\;H_{2s+1}(0)=0.\tag{16.12} $$
For $\alpha=0$, the squeezed coherent state $\ket{\alpha,\xi}$ reverts to the original squeezed vacuum $\ket{\xi}$.

Quadratic squeezing schemes are typically bases on a parametric process using a non-linear optical device. This corresponds to an interaction Hamiltonian quadratic in the field mode's creation and annihilation operators.

In parametric down-conversion, a non-linear medium is pumped by a frequency $\omega_{p}$ field. Some pumped photons $\hat{b}$ convert into pairs of frequency $\omega=\frac{\omega_{p}}{2}$ signal photons $\hat{a}$.
$$\hat{H}=\hbar \omega \hat{a}^{\dagger}\hat{a}+\hbar \omega_{p}\hat{b}^{\dagger}\hat{b}+i\hbar \chi^{(2)}(\hat{a}^2\hat{b}^{^{\dagger}}-\hat{a}^{\dagger{2}}\hat{b})\tag{16.13} $$where $\chi^{(2)}$ is a non-linear second order coefficient.

For the parametric approximation, assume the pump field in a strong coherent state $e^{ -i\hat{b}^{\dagger}\hat{b}\omega_{p}t }\ket{\beta}=\ket{\beta e^{ -i\omega_{p}t }}$. Replacing $\hat{b}^{\dagger},\hat{b}$ by their expectation values $\beta ^{*}e^{ i\omega_{p}t },\beta e^{ -i\omega_{p}t }$ gives
$$\hat{H}=\hbar \omega \hat{a}^{\dagger}\hat{a}+i\hbar \chi^{(2)}(\hat{a}^2\beta ^{*}e^{ i\omega_{p}t }-\hat{a}^{\dagger 2} \beta e^{ -i\omega_{P}t }).\tag{16.14} $$
Let $\eta=\chi^{(2)}\beta$ and transform to the interaction picture $(\hat{U}_{I}=e^{ i\hat{a}^{\dagger}\hat{a}\omega t })$,
$$\hat{H}_{I}=i\hbar(\hat{a}^{\dagger}\eta ^{*}e^{ i(\omega_{p}-2\omega)t }-\hat{a}^{\dagger 2}\eta e^{ -i(\omega_{p}-2\omega)t })\tag{16.15}. $$
The resonance condition is $\omega_{p}=2\omega$, which corresponds to the Hamiltonian
$$\hat{H}_{I}=i\hbar(\hat{a}^2\eta ^{*}-\hat{a}^{\dagger 2}\eta)\tag{16.16} .$$
The time evolution $e^{ -i\hat{H}_{I}t/\hbar }=e^{ \hat{a}\eta ^{*}-\hat{a}^{\dagger 2}\eta }$ gives the squeeze operator with $\xi=2\eta t$.

To detect squeezing, the typical scheme is to mix a squeezed signal field with a strong coherent field (the local oscillator). The experimental configuration is a 50:50 beam splitter with photodetectors behind the output ports. The correlator determines the difference in measured intensities.

![[Pasted image 20251119163206.png]]

The intensity difference is
$$I_{2}-I_{3}=\langle \hat{a}_{2}^{\dagger}\hat{a}_{2}-\hat{a}_{3}^{\dagger}\hat{a}_{3} \rangle =i\langle \hat{a}_{0}^{\dagger}\hat{a}_{1}-\hat{a}_{1}^{\dagger}\hat{a}_{0} \rangle .\tag{16.17} $$
Consider state $\hat{a}_{1}$ to be in a coherent state $\ket{\alpha e^{ -i\omega t }}$ with $\alpha=|\alpha|e^{ i\phi }$. Then, with $\frac{\vartheta}{2}=\phi+\frac{\pi}{2}$,
$$\langle \hat{a}_{2}^{\dagger}\hat{a}_{2}-\hat{a}_{3}^{\dagger}\hat{a}_{3} \rangle =|\alpha|\langle \hat{a}_{0}^{\dagger}e^{ -i\omega t }e^{ i\vartheta/2 }-\hat{a}_{0}e^{ i\omega t }e^{ -i\vartheta/2 } \rangle \tag{16.18}.  $$
For quadrature measurements, the signal light typically has the same frequency $\omega$, typically sourced from the same laser. In the interaction picture, $\hat{a}_{0}\to \hat{a}_{0}e^{ -i\omega t }$, $\hat{a}_{0}^{\dagger}\to \hat{a}_{0}^{\dagger}e^{ i\omega t }$ and
$$I_{2}-I_{3}=2|\alpha|\langle \hat{X}_{1}(\vartheta) \rangle \tag{16.19} $$
where
$$\hat{X}_{1}(\vartheta)=\frac{{\hat{a}e^{ -i\vartheta/2 }+\hat{a}^{\dagger}e^{ i\vartheta /2 }}}{2}\tag{16.20} .$$
