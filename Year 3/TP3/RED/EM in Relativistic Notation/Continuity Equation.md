The continuity equation describes the conservation of charge and current.
Consider Maxwell I:
$$\underline{\nabla}\cdot \underline{E}=\frac{\rho}{\varepsilon_{0}}.$$
$$\frac{\partial}{\partial t}(\underline{\nabla}\cdot \underline{E})=\frac{1}{\varepsilon_{0}} \frac{\partial \rho}{\partial t}\implies \underline{\nabla}\cdot\left( \frac{\partial\underline{E}}{\partial t} \right)=\frac{1}{\varepsilon_{0}} \frac{\partial \rho}{\partial t}$$
Consider Maxwell IV:
$$\underline{\nabla}\times \underline{B}=\mu_{0}\underline{j}+\mu_{0}\varepsilon_{0} \frac{\partial\underline{E}}{\partial t}.$$
$$\underline{\nabla}\cdot\left( \frac{\partial \underline{E}}{\partial t} \right)=\underline{\nabla}\cdot\left( \frac{1}{\mu_{0}\varepsilon_{0}}\underline{\nabla}\times \underline{B}-\frac{1}{\varepsilon_{0}}\underline{j} \right)=-\frac{1}{\varepsilon_{0}}\underline{\nabla}\cdot \underline{j}$$
$$\implies \underline{\nabla}\cdot \underline{j}+\frac{\partial \rho}{\partial t}=0.$$
This is the continuity equation.

Using the definition of charge and current density as a [4-vector](4-Potential.md), $j^{\mu}=(\rho c,\underline{j})$, the continuity equation can be written in relativistic notation as
$$\partial_{\mu}j^{\mu}=0.$$
