We aim to show $(\phi,c\underline{A})$ is a [4-vector](4-Vectors.md). To do this, we will first have to show that $(\rho c,\underline{j})$ is a 4-vector. This can be done from the continuity equation for charge conservation
$$\underline{\nabla}\cdot \underline{j}+\frac{\partial \rho}{\partial t}=0\implies \partial_{\mu}(\rho c,\underline{j})=0.$$
Let's call $j^\mu=(\rho c,\underline{j})$ so $\partial_{\mu}j^\mu=0$.
Wee need to check $j^\mu$ is a 4-vector.
Assume $j'^\mu=L^\mu_{\;\nu}j^\nu$:
From invariance:
$$\partial'_{\mu}j'^\mu=\Lambda_{\mu}^{\;\nu}L^\mu_{\;\rho}\partial_{\nu}j^\rho=\partial_{\nu}j^\nu.$$
Thus, the relation between $\Lambda_{\mu}^{\;\nu}$ and $L^\mu_{\;\rho}$ is
$$\Lambda_{\mu}^{\;\nu}L^\mu_{\;\rho}=\delta^\mu_{\;\rho}\implies L^\mu_{\;\rho}=\Lambda^\mu_{\;\rho}.$$
So as $j^\nu$ transforms to $j'^\mu$ under a Lorentz transformation, it is a contravariant 4-vector.
From this we can use [[D'Alembert Operator]] definition of potential relating $(\phi,c\underline{A})$ and $(\rho c,\underline{j})$:
$$\partial^\mu \partial_{\mu}(\phi,c\underline{A})=j^\mu.$$
Since we have shown $j^\mu$ is a 4-vector and that $\partial^\mu \partial_{\mu}$ is a scalar, $(\phi,c\underline{A})$ is therefore a 4-vector, which we will call the 4-potential
$$A^\mu=(\phi,c\underline{A})$$
