The [Minkowski norm](Lorentz%20Transforms.md) can be written as $$x^\mu x_{\mu}=(x^0)^2-(x^1)^2-(x^2)^2-(x^3)^2$$which is invariant under a Lorentz transform.
With this invariance we can define the Lorentz transform
$$x^\mu x_{\mu}=x'^\mu x'_{\mu}$$
$$(\Lambda^\mu_{\;\nu}x^\nu)(\Lambda^{\;\rho}_{\mu}x_{\rho})=(\Lambda^\mu_{\;\nu}\Lambda^{\;\rho}_{\mu})x^\nu x_{\rho}$$
As the Minkowski norm is invariant under a Lorentz transformation, the product of the two LTs are the identity
$$\Lambda^\mu_{\;\nu}\Lambda^{\;\rho}_{\mu}=\delta_{\nu}^{\;\rho}$$
This is the definition of the Lorentz group
##### Properties of LG
1. Associativity
2. Closure
	$$\Lambda^\nu_{\;\alpha}\Lambda^\mu_{\;\nu}\Lambda_{\mu}^{\;\rho}\Lambda_{\rho}^{\;\beta}=\Lambda^\nu_{\;\alpha}\delta_{\nu}^{\;\rho}\Lambda_{\rho}^{\;\beta}=\Lambda^\rho_{\;\alpha}\Lambda_{\rho}^{\;\beta}=\delta_{\alpha}^{\;\beta} \text{ so in Lorentz group}.$$
	
3. Inverse
	$$\Lambda^\mu_{\;\nu}\Lambda_{\mu}^{\;\rho}=\delta_{\nu}^{\;\rho}$$
	Define $\underline{\underline{M_{1}}}=\Lambda^\mu_{{\;\nu}}$ and $\underline{\underline{M_{2}^T}}=\Lambda_{\mu}^{\;\rho}$ and take the determinants, using the fact that $\delta_{\nu}^{\;\rho}$ is the [identity](Index%20and%20Tensor%20Notation.md). 
	$$\det(\delta_{\nu}^{\;\rho})=\mathbb{I}=1$$
	$$\det(\underline{\underline{M_{1}}}\underline{\underline{M_{2}^T}})=\det(\underline{\underline{M_{1}}})\det(\underline{\underline{M_{2}^T}})=1$$
	As $\det(\underline{\underline{M_{2}^T}})=\det(\underline{\underline{M_{2}}})$,
	$$\det(\underline{\underline{M_{1}}})\det(\underline{\underline{M_{2}}})=1$$
	As $\delta^{\;\rho}_{\nu}$ is the identity, $\underline{\underline{M_{1}}}^{-1}=\underline{\underline{M_{2}^T}}$ so $\det(\underline{\underline{M_{1}}})=\det(\underline{\underline{M_{2}}})$ which gives
	$$\det(\underline{\underline{M_{1}}})^2=1$$
	$$\therefore \det(\underline{\underline{M_{1}}})=\pm 1.$$
	As $\det(\underline{\underline{M_{1}}})\neq 0$, $\exists$ $\underline{\underline{M_{1}}}^{-1}$.

4. Identity
	$$\Lambda^{\;\sigma}_{\mu}=\frac{\partial x'_{\mu}}{\partial x_{\sigma}}$$
	As $\Lambda^\mu_{\;\nu}\Lambda_{\mu}^{\;\rho}=\delta_{\nu}^{\;\rho}$,
	$$\frac{\partial x'^\mu}{\partial x^\nu} \frac{\partial x^\rho}{\partial x'^\mu}=\frac{\partial x^\rho}{\partial x^\mu}=\delta_{\nu}^{\;\rho}.$$
	This shows there is an existence of an identity.

If a contravariant vector $y^\mu$ transforms like $x^\mu$, then $y^\mu x_{\mu}$ is invariant under a Lorentz transformation:
$$y'^\mu x'_{\mu}=(\Lambda^\mu_{\;\nu }y^\nu)(\Lambda_{\mu}^{\;\sigma}x_{\sigma})=(\Lambda^\mu_{\;\nu}\Lambda_{\mu}^{\;\sigma})y^\nu x_{\sigma}=\delta_{\nu}^{\;\sigma}y^\nu x_{\sigma}=y^\nu x_{\nu}.$$
For this proof it does not matter which vector is contravariant as
$$y^\mu x_{\mu}=y^\mu(g_{\mu \nu}x^\nu)=(y^\mu g_{\mu \nu})x^\nu=y_{\nu}x^\nu=y_{\mu}x^\mu.$$
This is the Minkowski scalar product.
This allows us to rewrite the laws of physics in terms of quantities that undergo a Lorentz transformation with the correct properties. The types of quantities are:
- Scalar: A quantity that is invariant under a Lorentz transformation. Has rank 0 since it has $4^0=1$ entry
- 4-Vector: An entity that transforms under a Lorentz transformation. It has rank 1 since it has $4^1=4$ entries
- Tensor of rank 2: A quantity with two indices and $4^2=16$ entries

The rank of a quantity can be seen by the number of free indices. For example, with a Minkowski norm $x^\mu x_{\mu}$, there is only one index, which is repeated, so there are no free indices and hence the result has a rank of 0 (scalar), or a Lorentz transformation $\Lambda^\mu_{\;\nu}x^\nu$, there are two indices, with one index repeated, $\nu$, so $\mu$ is a free index so the result has a rank of 1 (4-vector).