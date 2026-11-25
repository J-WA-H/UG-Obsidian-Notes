The [[Field Tensor]] can be written as
$$F^{\mu \nu}=\partial^{\mu}A^{\nu}-\partial^{\nu}A^{\mu}.$$
Consider the field tensor under [[Gauge Transformations]],
$$F'^{\mu \nu}=\partial^{\mu}(A^{\nu}-c\partial^{\nu}\lambda)-\partial^{\nu}(A^{\mu}-c\partial^{\mu}\lambda)$$
$$=\partial^{\mu}A^{\nu}-\partial^{\nu}A^{\mu}-c\partial^{\mu}\partial^{\nu}\lambda+c\partial^{\nu}\partial^\mu \lambda$$
$$=\partial^{\mu}A^{\nu}-\partial^{\nu}A^{\mu}=F^{\mu \nu}.$$
The field tensor is invariant under a gauge transformation.

For the inhomogeneous Maxwell equations, consider $\partial_{\mu}F^{\mu \nu}$.
$$\partial_{\mu}F^{\mu \nu}=\partial_{\mu}\partial^{\mu}A^{\nu}-\partial_{\mu}\partial^{\nu}A^{\mu}=\partial_{\mu}\partial^{\mu}A^{\nu}-\partial^{\nu}\partial_{\mu}A^{\mu}.$$
The last term goes to zero from the [Lorentz gauge condition](Potentials.md).
This yields
$$\partial_{\mu}F^{\mu \nu}=\partial_{\mu}\partial^{\mu}A^{\nu}.$$
Using the Lorenz gauge gives
$$\partial_{\mu}F^{\mu \nu}=\frac{1}{c\varepsilon_{0}}j^{\nu}.$$
This equation holds Maxwell I and IV.
Proof: For $\nu=0$,
$$\partial_{\mu}F^{\mu 0}=\frac{\partial F^{00}}{\partial(ct)}+\frac{\partial F^{10}}{\partial x}+\frac{\partial F^{20}}{\partial y}+\frac{\partial F^{30}}{\partial z}=\frac{1}{c\varepsilon_{0}}\rho c$$
$$=\frac{\partial E_{x}}{\partial x}+\frac{\partial E_{y}}{\partial y}+\frac{\partial E_{z}}{\partial z}=\underline{\nabla}\cdot \underline{E}=\frac{\rho}{\varepsilon_{0}}.$$
For $\nu=1$:
$$\partial_{\mu}F^{\mu 1}=\frac{\partial F^{01}}{\partial(ct)}+\frac{\partial F^{11}}{\partial x}+\frac{\partial F^{21}}{\partial y}+\frac{\partial F^{31}}{\partial z}=\frac{1}{c\varepsilon_{0}}j_{x}$$
$$=-\frac{\partial E_{x}}{\partial (ct)}+c\frac{\partial B_{z}}{\partial y}-c \frac{\partial B_{y}}{\partial z}=(\underline{\nabla}\times \underline{B})_{x}-\frac{1}{c^2} \frac{\partial E_{x}}{\partial t}=\mu_{0}j_{x}.$$
The dual field tensor in covariant notation is given by
$$\tilde{F}^{\mu \nu}=\frac{1}{2}\epsilon^{\mu \nu \rho\sigma}F_{\rho\sigma}$$
where $\epsilon_{\mu \nu\rho \sigma}$ is the rank-4 [Levi-Civita symbol](Vectors%20and%20Tensors.md), which is anti symmetric.

Consider $$\partial_{\mu}\tilde{F}^{\mu \nu}=\frac{1}{2}\partial_{\mu}\epsilon^{\mu \nu \rho \sigma}F_{\rho \sigma}=\frac{1}{2}\epsilon^{\mu \nu \rho \sigma}\partial_{\mu}(\partial_{\rho}A_{\sigma}-\partial_{\sigma}A_{\rho}).$$The 4-gradiants are symmetric under interchange when the Levi-Civita symbol is anti-symmetric, so the total product of them is zero, $\partial_{\mu}\tilde{F}^{\mu \nu}=0$. This contains Maxwell II and III.

This gives a covariant form of Maxwell's equations
$$\partial_{\mu}F^{\mu \nu}=\frac{1}{c\varepsilon_{0}}j^{\nu}$$
$$\partial_{\mu}\tilde{F}^{\mu \nu}=0.$$
