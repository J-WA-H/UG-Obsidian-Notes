We call an [operator](Linear%20Operators.md) adjoint if
$$(\underline{y},A\underline{x})=(A^{\dagger}\underline{y},\underline{x})$$
All linear operators have a unique linear adjoint operator.
Proof:
A vector $\underline{x}$ can be decomposed as $\underline{x}=\underline{e}_{i}x^{i}$. For an orthonormal basis, $x^{i}=(\underline{e}^{i},\underline{x})$.
$$(\underline{e}_{i},\underline{x})=(\underline{e}_{i},\underline{e}_{j})x^{j}=\delta_{ij}x^{j}=x_{i}.$$
Hence $\underline{x}=\underline{e}_{i}x^{i}=\underline{e}_{i}(\underline{e}_{i},\underline{x})$.
For $A^{\dagger}\underline{y}=\underline{e}_{i}(\underline{e}_{i},A^{\dagger}\underline{y})=\underline{e}_{i}(A^{\dagger}\underline{y},\underline{e}_{i})^*=\underline{e}_{i}(\underline{y},A\underline{e}_{i})^*=\underline{e}_{i}(A\underline{e}_{i},\underline{y})$.

For the matrix representation of the adjoint:
$$A_{ij}=(\underline{e}_{i},A\underline{e}_{j})$$
$$(A^{\dagger})_{ij}=(\underline{e}_{i},A^{\dagger}\underline{e}_{j})=(A\underline{e}_{i},\underline{e}_{j})=(\underline{e}_{j},A\underline{e}_{i})^*=A_{ji}^*.$$
This shows the adjoint operator is the complex transpose of the operator.
$$A^{\dagger}=(A^T)^*=(A^*)^T.$$
A Hermitian or self adjoint matrix is equal to its adjoint
$$A=A^{\dagger}.$$
