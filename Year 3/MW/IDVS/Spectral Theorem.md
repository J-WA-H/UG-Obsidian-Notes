The spectral theorem states that for any symmetric matrix, we can always find an orthonormal basis.

By being able to diagonalise [[Linear Operators]], it allows the simplification of problems into computations using the corresponding diagonal matrix.

Mathematically, the spectral theorem encompasses all ways to extend the eigenvalue problem of a square matrix to a much wider set of operators that can operate on a variety of mathematical spaces.

Lemma: The eigenvalues of a [unitary operator](Unitary%20and%20Orthogonal%20Operators.md), $U$, are of the form $e^{i\phi}$ for $\phi\in \mathbb{R}$. The eigenvalues corresponding to different eigenvalues are orthogonal.

Proof: Let $\underline{v}$ be an eigenvector of the unitary operator $U$ with eigenvalue $\lambda$.
Taking the inner product of $\underline{v}$ with itself gives
$$(\underline{v},\underline{v})=(U\underline{v},U\underline{v})=\lvert \lambda \rvert^2(\underline{v},\underline{v}) $$
$$\implies \lvert \lambda \rvert^2=1\therefore \lambda=e^{i\phi}\;\forall\;\phi \in \mathbb{R}.$$
Now consider two different eigenvectors $\underline{v}_{1},\underline{v}_{2}$, and take their inner product.
$$(\underline{v}_{1},\underline{v}_{2})=(U\underline{v}_{1},U\underline{v}_{2})=\lambda_{1}^{*}\lambda_{2}(\underline{v}_{1},\underline{v}_{2})=\frac{\lambda_{2}}{\lambda_{1}}(\underline{v}_{1},\underline{v}_{2}).$$
As $\lambda_{2}\neq \lambda_{1}$, $\frac{\lambda_{2}}{\lambda_{1}}\neq 1$ so $(\underline{v}_{1},\underline{v}_{2})=0\;\;\square$.
Note that if we have degenerate eigenvalues, the corresponding eigenvectors are not necessarily orthogonal. This can be rectified using Gram-Schmidt.

Lemma: The eigenvalues of a Hermitian operator, $H$, are real. The eigenvectors corresponding to different eigenvalues are orthogonal.

Proof: Let $\underline{v}$ be an eigenvector of $H$ with eigenvalue $\lambda$.
$$(\underline{v},H\underline{v})=\lambda(\underline{v},\underline{v})$$
$$(H\underline{v},\underline{v})=\lambda^*(\underline{v},\underline{v})=(\underline{v},H^{\dagger}\underline{v})=(\underline{v},H\underline{v})$$
$$\implies \lambda=\lambda^{*}\implies \lambda\in \mathbb{R}.$$
Now consider two different eigenvectors $\underline{v}_{i},\underline{v}_{j}$.
$$(\underline{v}_{i},H\underline{v}_{j})=\lambda_{j}(\underline{v}_{i},\underline{v}_{j})$$
$$(\underline{v}_{i},H\underline{v}_{j})=(H^{\dagger}\underline{v}_{i},\underline{v}_{j})=(H\underline{v}_{i},\underline{v}_{j})=\lambda_{i}(\underline{v}_{i},v_{j}).$$
Since $\lambda_{i}\neq \lambda_{j}$, $(\underline{v}_{i},\underline{v}_{j})=0\;\;\square$.
Note that again that we have assumed non-degenerate eigenvalues.

Taking these two lemmas together establish the fact eigenvectors of a unitary and Hermitian operators form orthonormal sets. Since the number of eigenvectors is $n$, these are [maximal sets](Inner%20Product%20Spaces.md) that form an orthonormal basis of the vector space $V$.
This proves that for the operator $A$ being unitary of Hermitian, the new basis from $RAR^{-1}=A'$ is orthonormal. Here $A'$ is simply made up from the eigenvalues of $A$ placed on the diagonal.
This proves the assumption that eigenvectors form a complete set of vectors for the vector space.