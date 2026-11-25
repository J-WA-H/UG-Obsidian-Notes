Matrix $A^{i}_{\;j}$ uniquely defines a [linear transformation](Linear%20Transforms%20and%20Symmetries.md). Vectors transform as
$$x'^{i}=A^{i}_{\;j}x^{j}.$$
This is the definition of a vector if all of its components transform like this where A has to be an orthogonal matrix $\underline{\underline{A}}\in O(n)$.

A vector is not just some object with indices, it must transform appropriately too under a matrix transformation.

A tensor is an object with multiple indices that transforms under particular symmetries.
A rank-n tensor has n indices - $T^{i_{1}i_{2}\dots i_{3}}$.
They transform as
$$T'^{i_{1}i_{2}\dots i_{3}}=A^{i_{1}}_{\;j_{1}}A^{i_{2}}_{\;j_{2}}\dots A^{i_{n}}_{\;j_{n}}T^{i_{1}i_{2}\dots i_{n}}.$$
The [metric](Inner%20Product%20Spaces.md) tensor is the simplest form that raises and lowers indices
$$x_{i}=g_{ij}x^{j},\;x^{i}=g^{ij}x_{j}.$$
In the case of vectors and tensors in an orthonormal basis in 3-dimensional Euclidean geometry, $g_{ij}=\delta_{ij}$.

We need to distinguish upper and lower indices.
We call $x^{i}$ contravariant (Row vector) and $x_{i}$ covariant (Column vector).

An example of a rank-3 tensor is the Levi-Civita symbol
$$\epsilon_{ijk}=\begin{cases}
+1 & (ijk)=(123),(231),(312) \\
-1 & (ijk)=(132),(321),(213) \\
0 & \text{any two indices equal}
\end{cases}.$$
