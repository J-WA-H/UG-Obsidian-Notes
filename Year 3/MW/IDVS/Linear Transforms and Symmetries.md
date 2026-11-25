Consider an n-dimensional [vector space](Vector%20Spaces.md) $E$ over the field of real numbers $F=\mathbb{R}$. A linear transformation that acts on this vector space is defined as
$$\underline{\underline{A}}\underline{x}=\underline{x}'\;\forall \;\underline{x},\underline{x}'\in E.$$
Linearity: $\underline{\underline{A}}(\alpha \underline{x}_{1}+\beta \underline{x}_{2})=\alpha \underline{\underline{A}}\underline{x}_{1}+\beta \underline{\underline{A}}\underline{x}_{2};\;\alpha,\beta\in \mathbb{R}\;\forall\;\underline{x}_{1},\underline{x}_{2}\in E$.

To specify linear transformations, look at how it acts on components of $\underline{x}$:
- Choose orthonormal basis $\{\underline{\hat{e}}_{i}\}$
The transformation can be described as $x'^{i}=A^{i}_{\;j}x^{j}$ where $x'^{i}$ is the coordinates of the transformed vector in the same basis.

If the scalar product is invariant, a linear transformation is a symmetric transformation.
$$(\underline{x}',\underline{y}')=(\underline{x},\underline{y})$$
$$\delta_{ij}x'^{i}y'^{j}=\delta_{ij}A^{i}_{\;k}x^{k}A^{j}_{\;l}y^{l}=\delta_{ij} x^{i}y^{j}$$
$$\implies \delta_{ij}A^{i}_{\;k}A^{j}_{\;l}=\delta_{kl}\implies \delta_{kl}x^{k}y^{l}=\delta_{ij}x^{i}y^{j}.$$
