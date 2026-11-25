The weak coupling limit is when the strength of the effective interaction $V$ times the density of states $g(\varepsilon)$ at the Fermi energy is much smaller than $\varepsilon_{F}$: 
$$V\times g(\mu)<\mu \tag{20.1} $$
In this limit the [equation for](BCS%20Superconductivity.md) $\Delta$ becomes
$$1=\frac{V}{2}g(\mu)\int_{\mu-\omega_{D}}^{\mu+\omega_{D}} \frac{d\varepsilon}{\sqrt{ \Delta^2+(\varepsilon-\mu)^2 }}\tag{20.2} $$
$$1=Vg(\mu)\sinh ^{-1}\left( \frac{\omega_{D}}{\Delta} \right)\implies\Delta=\frac{\omega_{D}}{\sinh\left( \frac{1}{Vg(\mu)} \right)}\simeq 2\omega_{D}e^{ 1/Vg(\mu) }\tag{20.3} .$$
The solution to the gap equation cannot be expanded in a power series around $V=0$, so perturbation theory cannot be used.

We can now find the difference in total energy between the BCS and the normal state. For $\theta_{\vec{k}}=0$, the normal state is
$$\bra{\Psi_{n}}H_{red}-\mu \hat{N}\ket{\Psi_{n}} = 2\sum_{\varepsilon_{\vec{p}}<\mu}(\varepsilon_{\vec{p}}-\mu)\tag{20.4} $$
The difference is
$$\Delta E=\bra{\Psi_{BCS}}H_{red}-\mu \hat{N}\ket{\Psi_{BCS}}-\bra{\Psi_{n}}H_{red}-\mu \hat{N}\ket{\Psi_{n}}=-g(\mu)\omega_{D}[\sqrt{ \omega_{D}^2+\Delta^2 }-\omega_{D}]\simeq -g(\mu)\omega_{D}^2\left[ \sqrt{ 1+\frac{\Delta^2}{\omega_{D}^2} }-1 \right]=-g(\mu) \frac{\Delta^2}{2}.     $$
$(20.5)$

