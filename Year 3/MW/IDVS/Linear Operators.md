An operator $A$ is a function mapping vector $\underline{x}$ from a given domain in vector space $X$ to its image in the codomain vector space $Y$.
For $\underline{x}\in X$ and $\underline{y}\in Y$, $A:X\to Y$.
$$\underline{y}=A(\underline{x}).$$
This is independent of coordinate system/[basis](Basis%20of%20Vectors.md). In general $\text{dim}(X)\neq\text{dim}(Y)$ however in most cases we will look at they are equal.

If the map is linear, the operator is linear.
$$A(\underline{x}_{1}+\underline{x}_{2})=A(\underline{x}_{1})+A(\underline{x}_2)\;\forall\;\underline{x}_{1},\underline{x}_{2}\in X.$$

$$\alpha A(\underline{x}_{1})=A(\alpha \underline{x}_{1})\;\forall \;\alpha\in F$$
Examples of linear operators:
Identity operator
$$O(\underline{x})=\underline{x}$$
Null operator
$$E(\underline{x})=\underline{0}.$$
Consider $\text{dim}(X)=n$ and $\text{dim}(Y)=m$, then any linear operator in $\mathbb{R}^n/\mathbb{C}^n$ can be represented by an $m\times n$ matrix.
$$A(\underline{e}_{j})=\underline{\varepsilon}_{i}A^{i}_{\;j}.$$
$A(\underline{e}_{j})$ is a vector in $Y$ that can be expanded in terms of the basis $\{\varepsilon_{j}\}$, with coefficients given by the matrix $A^{i}_{\;j}$.
For any vector $\underline{x}\in X$ it can be written as an expansion of its basis elements $\underline{x}=\underline{e}_{i}x^i$, similarly any vector $\underline{y}\in Y$ can be written as $\underline{y}=\underline{\varepsilon}_{i}y^i$.
Using this we can rewrite
$$A(\underline{x})=A(\underline{e}_{j}x^j)=A(\underline{e}_{j})x^j=\underline{\varepsilon}_{i}A^{i}_{\;j}x^{j}.$$
To emphasise the operator is linear, the brackets are often dropped, $A(\underline{x})=A\underline{x}$.
$$A\underline{e}_{j}=\varepsilon_{i}A^{i}_{\;j}.$$
The coefficients in this expansion are given by
$$A^{i}_{\;j}=(\underline{\varepsilon}_{i},A\underline{e}_{j})$$
