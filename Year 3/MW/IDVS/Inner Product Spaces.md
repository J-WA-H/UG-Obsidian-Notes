An inner product space is a [vector space](Vector%20Spaces.md) equipped with an [inner product](Scalar%20Products.md). 
Consider an n-dimension [basis](Basis%20of%20Vectors.md) of orthonormal vectors
$$\{\underline{\hat{e}}_{1},\underline{\hat{e}}_{2},\dots,\underline{\hat{e}}_{n}\}.$$
where $(\underline{\hat{e}}_{i},\underline{\hat{e}}_{j})=\delta_{ij}$.

This set of n orthogonal vectors in n-dimensional space is a maximal set of orthonormal vectors
This set isn't unique, as a [rotation](Rotations.md) will map this set to another maximal set of orthonormal vectors.

The set $\{\underline{\hat{e}}_{i}\}$ is complete since any vector $\underline{x}\in E$ can be decomposed into a linear combination of $\underline{\hat{e}}_{i}.$ 
$$\underline{x}=\sum_{i=1}^{n}x^{i}\underline{\hat{e}}_{i}$$
where $x^{i}$'s are coordinates of $\underline{x}$ in the basis.

In coordinate representation, we can represent the inner product
$$(\underline{x},\underline{y})=\left( \sum_{i=1}^{n}x^{i}\underline{\hat{e}}_{i},\sum_{j=1}^{n}y^{j}\underline{\hat{e}}_{j} \right)=\sum_{i=1}^{n}x^{i}\sum_{j=1}^{n}y^{j}(\underline{\hat{e}}_{i},\underline{\hat{e}}_{j})=\sum_{i=1}^{n}\sum_{j=1}^{n}x^{i}y^{j}\delta_{ij}=\sum_{i=1}^{n}x_{i}y_{i}$$
In a more general case (where the basis isn't orthonormal), the inner product is defined by a metric $g_{ij}$. 
More generally
$$(\underline{x},\underline{y})=\sum_{i=1}^{n}\sum_{j=1}^{n}g_{ij}x^{i}y^{j}.$$
$\delta_{ij}$ is the simplest form of a metric,
$$(\underline{x},\underline{y})=\sum_{i=1}^{n}\sum_{j=1}^{n}\delta_{ij}x^{i}y^{j}=\sum_{j=1}^{n}x_{j}y^{j}.$$
$$x_{i}=\sum_{j=1}^{n}\delta_{ij}x^{j},\;x^{i}=\sum_{j=1}^{n}\delta^{ij}x_{j}.$$
$$\delta_{ij}=\delta^{ij}=\delta^{i}_{\;j}=\mathbb{I}.$$
