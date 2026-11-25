The master equation for [[Github/Year 4/Advanced TP/QO/Spontaneous Emission|Spontaneous Emission]] is 
$$\tag{19.26} \frac{d\tilde{\rho}_{A}}{dt}=\frac{\Gamma}{2}(2\hat{\sigma}^{-}\tilde{\rho}_{A}\hat{\sigma}^{+}-\tilde{\rho}_{A}\hat{\sigma}^{+}\hat{\sigma}^{-}-\hat{\sigma}^{+}\hat{\sigma}^{-}\tilde{\rho}_{A})$$
where $\Gamma$ is a decay constant. This is expressed in the interaction picture. In the Schrodinger picture, 
$$\frac{d\rho_{A}}{dt}=-i \frac{\omega_{A}}{2}[\hat{\sigma}_{z},\rho_{A}]-\frac{\Gamma}{2}(\hat{\sigma}^{+}\hat{\sigma}^{-}\rho_{A}+\rho_{A}\hat{\sigma}^{+}\hat{\sigma}^{-}-2\hat{\sigma}^{-}\rho_{A}\hat{\sigma}^{+})\tag{20.1} .$$
Note that $\tilde{\rho}_{A}=\hat{U}_{I}\rho_{A}\hat{U}_{I}^{\dagger}$. In general, a master equation is in Linblad form if it looks like
$$\frac{d\rho}{dt}=-\frac{i}{\hbar}[\hat{H},\rho]-\sum_{k} \frac{\chi_{k}}{2}(\hat{C}_{k}^{\dagger}\hat{C}_{k}\rho+\rho \hat{C}_{k}^{\dagger}\hat{C}_{k}-2\hat{C}_{k}\rho \hat{C}_{k}^{\dagger}).\tag{20.2} $$
This is positive and trace preserving. The $\hat{C}_{k}$ operators are jump operators, which can be anything.

In general, if $\rho'=\hat{U}\rho \hat{U}^{\dagger}$,
$$\frac{d\rho'}{dt}=-\frac{i}{\hbar}[\hat{H}'.\rho']-\sum_{k} \frac{\chi_{k}}{2}(\hat{C}'^{\dagger}_{k}\hat{C}'_{k}\rho'+\rho'\hat{C}'^{\dagger}_{k}\hat{C}'_{k}-2\hat{C}'_{k}\rho'\hat{C}_{k}'^{\dagger}).\tag{20.3} $$
Here $\hat{C}_{k}'=\hat{U}\hat{C}_{k}\hat{U}^{\dagger}$ and $\hat{H}'=\left( \hat{U}\hat{H}\hat{U}^{\dagger}+i\hbar \frac{d\hat{U}}{dt} \hat{U}^{\dagger} \right)$.

The spontaneous emission master equation is simple enough to be solved exactly. For simplicity, return to the interaction picture and set
$$\tilde{\rho}_{ee}=\bra{e} \tilde{\rho}\ket{e} ,\;\tilde{\rho}_{eg}=\bra{e} \tilde{\rho}\ket{g} ,\;\tilde{\rho}_{ge}=\bra{g} \tilde{\rho}\ket{e} ,\;\tilde{\rho}_{gg}=\bra{g} \tilde{\rho}\ket{g} .\tag{20.4}  $$
The basic equations of motion are
$$\frac{d\tilde{\rho}_{ee}}{dt}=-\Gamma \tilde{\rho}_{ee},\; \frac{d\tilde{\rho}_{eg}}{dt}=-\frac{\Gamma}{2}\tilde{\rho}_{eg}.\tag{20.5} $$
This gives solutions,
$$\tilde{\rho}_{ee}(t)=e^{ -\Gamma t }\tilde{\rho}_{ee}(0);\;\tilde{\rho}_{eg}(t)=e^{ -\Gamma t/2 }\tilde{\rho}_{eg}(0)\tag{20.6} $$
$$\tilde{\rho}_{gg}(t)=1-e^{ -\Gamma t }(1-\tilde{\rho}_{gg}(0));\; \tilde{\rho}_{ge}(t)=e^{ -\Gamma t/2 }\tilde{\rho}_{ge}(0).\tag{20.7} $$
This shows the decay of the excited state population and coherences. This is an intrinsically statistical description. As time goes on, all states move to the ground state. The master equation describes what happens on average, and not a specific path.

In the Schrodinger picture, these solutions become
$$\rho_{ee}(t)=e^{ -\Gamma t }\rho_{ee}(0),\;\rho_{eg}(t)=e^{ -i\Gamma t/2 }e^{ -i\omega_{A}/2 }\rho_{eg}(0)\tag{20.8} $$
$$\rho_{gg}(t)=1-e^{ -\Gamma t }(1-\rho_{gg}(0)),\;\rho_{ge}(t)=e^{ -\Gamma t/2 }e^{ i\omega_{A}/2 }\rho_{ge}(0).\tag{20.9} $$
This can be used to describe the [[Rabi Model]] with decay. There is a straightforward extension to the master equation,
$$\frac{d\rho_{A}}{dt}=-\frac{i}{2}[\Delta\hat{\sigma}_{z}+\Omega(\hat{\sigma}^{+}+\hat{\sigma}^{-}),\rho_{A}]-\frac{\Gamma}{2}(\hat{\sigma}^{+}\hat{\sigma}^{-}\rho_{A}+\rho_{A}\hat{\sigma}^{+}\hat{\sigma}^{-}-2\hat{\sigma}^{-}\rho_{A}\hat{\sigma}^{+}).\tag{20.10} $$
This is also simple enough to be solved. All the population is initially in the ground state,
$$\rho_{ee}(t)=\frac{\Omega^2}{2\Omega^2+\Gamma^2}\left( 1-e^{ -3\Gamma t/4 }\left[ \cos(\Omega't)+\frac{3\Gamma}{\sqrt{ 16\Omega^2-\Gamma^2 }}\sin(\Omega't) \right] \right)\tag{20.11} $$where $$\Omega'=\sqrt{ \Omega^2-\frac{\Gamma^2}{16} }.\tag{20.12} $$
