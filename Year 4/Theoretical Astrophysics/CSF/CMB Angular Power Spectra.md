Baryons recombine when $T\approx 3000\text{ K}$ at $z_{rec}\approx 1000$. Here the universe becomes transparent to CMB photons which [free-stream](Free%20Streaming%20of%20Dark%20Matter.md). 

Density fluctuations at recombination cause perturbations $\frac{\Delta T(\theta,\phi)}{\bar{T}}$ in the CMB temperature that can be measured by us today. The tiny $\frac{\Delta T}{\bar{T}}$ was predicted in the 1960s and observed in 1992.

When the CMB is measured, we get a uniform temperature of $2.73\text{ K}$ as fluctuations are of order $\sim 10^{-4}$.
![[Pasted image 20251128124030.png]]

First, we get to the second diagram by adjusting for $\frac{\Delta T}{\bar{T}}\sim 10^{-3}$ and adjusting for the relative motion of the Earth and our galaxy, we get diagram 3 and we get diagram 4 after the galactic foreground subtraction, which gives$$\frac{\Delta T}{\bar{T}}\sim 10^{-5}\tag{23.1} .$$
![[Pasted image 20251128124402.png]]

The $\frac{\Delta T}{\bar{T}}<0$ fluctuations are in blue and the $\frac{\Delta T}{\bar{T}}>0$ fluctuations are in red.

We can expand $\Delta T(\theta,\phi)$ in spherical harmonics,
$$\frac{\Delta T(\theta,\phi)}{\bar{T}}=\frac{{T(\theta,\phi)-\bar{T}}}{\bar{T}}=\sum_{\ell=0}^{\infty}\sum_{m=-\ell}^{\ell}a_{\ell m}Y_{\ell m}(\theta,\phi).\tag{23.2} $$This is analogous to a Fourier transform with $(\theta,\phi)$ - angles in polar coordinates.
$$Y_{\ell m}(\theta,\phi)\propto e^{ im\phi }P_{\ell}^{m}(\cos \theta).\tag{23.3} $$
The set $\{ Y_{\ell m}(\theta,\phi) \}$ form a complete basis. $Y_{\ell m}$ has a total angular wavelength $\approx \frac{2\pi}{\ell}$ and produces features on the sky of angular size $$\theta=\frac{\pi}{\ell}\text{ rad}=\frac{180^{\circ}}{\ell}.\tag{23.4} $$
$\ell=0$ is a monopole (mean over the sky). $\ell=1$ is a dipole (due to our motion relative to the CMB). $\ell=2$ is produced by density fluctuations, at recombination on last scattering surface (primary anisotropy) or the line of sight after recombination (secondary anisotropy).
![[Pasted image 20251128125346.png]]
Each panel shows the contribution to $\frac{\Delta T}{\bar{T}}$ from a multipole $\ell$,
$$\sum_{m=-\ell}^{\ell}a_{\ell m}Y_{\ell m}(\theta,\phi)\tag{23.5} .$$
Larger values of $\ell$ are sensitive to smaller angular scales.

The angular power spectrum is defined as
$$C_{\ell}=\frac{1}{2\ell+1}\sum_{m=-\ell}^{\ell}|a_{\ell m}|^2\tag{23.6} .$$$C_{\ell}$ measures the mean contribution to $\left\langle  \left( \frac{\Delta T}{\bar{T}} \right)^2  \right\rangle$ from spherical harmonics $Y_{\ell m}(\theta,\phi)$ with angular wavenumber $\ell$ and averaged over $m$.
$|a_{\ell m}|$ depends on the orientation of the spherical coordinate system while $C_{\ell}$ does not. $\langle |a_{\ell m}|^2 \rangle$ is independent of $m$ for fixed $\ell$, when averaged over observers in a statistically homogeneous and isotropic universe. $C_{\ell}$ provides a complete statistical description of $\frac{\Delta T}{\bar{T}}$ for an isotropic universe with Gaussian fluctuations. 

The angular power spectrum is usually plotted as $\frac{\ell(\ell+1)C_{\ell}}{2\pi}$ which is the contribution to $\left\langle  \left( \frac{\Delta T}{\bar{T}} \right)^2  \right\rangle$ per $\ln \ell$.
![[Pasted image 20251128142511.png]]
The y-axis is $\frac{\ell(\ell+1)}{2\pi}$ for $\Delta T$ in $\mu K$. Note the non-linear stretch in the angular wavenumber $\ell$ on the x-axis.

The angular diameter distance $d_{A}$ relates proper size to the line of sight to the angle,
$$d_{A}(a)\equiv \frac{L_{p}}{\theta}\tag{23.7}$$
with angular size $\theta$ in radians.
![[Pasted image 20251128142855.png]]
For $a_{rec}\ll 1$, $d_{A}(a_{rec})\approx \left( \frac{2c}{H_{0}} \right)a_{rec}\kappa(\Omega_{m_{0}},\Omega_{v_{0}})$ where $\kappa(\Omega_{m_{0}},\Omega_{v_{0}})$ is a dimensionless function, $\Omega_{m_{0}}=1,\Omega_{v_{0}}=0\implies \kappa=1$.

A perturbation with proper wavelength $\lambda$ at recombination has an apparent angular wavelength
$$\lambda_{\theta}\approx \frac{\lambda}{d_{A}(a_{rec})}\tag{23.8} .$$
![[Pasted image 20251128143331.png]]

As $\lambda_{\theta}\approx \frac{2\pi}{\ell}$ gives that the wavenumber $\ell$ is related to proper wavelength $\lambda$ by
$$\frac{2\pi}{\ell}\approx \frac{\lambda}{d_{A}(a_{rec})}\tag{23.9} .$$
The horizon size at recombination is
$$R_{H}(a_{rec})=\frac{c}{H(a_{rec})}.\tag{23.10} $$
For a matter-dominated universe at recombination,
$$H(a_{rec})\approx \frac{H_{0}\Omega_{m_{0}}^{1/2}}{a_{rec}^{3/2}}\implies R_{H}(a_{rec})=\frac{c}{H_{0}} \frac{a_{rec}^{3/2}}{\Omega^{1/2}_{m_{0}}}\tag{23.11} .$$
Thus, $R_H$ corresponds to the angular size
$$\theta_{H}(a_{rec})=\frac{R_{H}(a_{rec})}{d_{A}(a_{rec})}\approx \frac{\frac{c}{H_{0}} \frac{a_{rec}^{3/2}}{\Omega_{m_{0}}^{1/2}}}{\left( \frac{2c}{H_{0}} \right) a_{rec}\kappa(\Omega_{m_{0}},\Omega_{v_{0}})}=\frac{a_{rec}^{1/2}}{2\Omega_{m_{0}}^{1/2}\kappa(\Omega_{m_{0}},\Omega_{v_{0}})}\tag{23.12} .$$
For a flat universe, $\Omega_{m_{0}}+\Omega_{v_{0}}=1\implies \kappa \approx \Omega_{m_{0}}^{-1/2}$ with $z_{rec}=10^{3}$,
$$\theta_{H}\approx 0.91^{\circ} \implies \ell \approx \frac{\pi}{\theta_{H}}\approx 200. \tag{23.13} $$
