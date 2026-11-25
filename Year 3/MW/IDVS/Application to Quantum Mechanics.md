Many areas of linear algebra are used in the mathematical formalisation of quantum mechanics. To do this, we use standard Dirac notation. Here vectors in the [[Hilbert Spaces]] are denoted by $\ket{v}$ and $\bra{v}=\ket{v}^{*}$.

The scalar product is denoted by $\braket{ v | w }$. These bra and ket vectors replace the standard Schrodinger wavefunctions
$$\psi(x)\to \ket{\psi} $$
$$\phi_{n}(x)\to \ket{n} .$$
$$\int \psi_{m}^{*}(x)\psi_{n}(x)dx\to \braket{ m | n } .$$
The operator $F$ s.t. $F\psi_{m}=\psi_{n}$ is $F\ket{m}=\ket{n}$.
Rules for QM:
1. The states in a system are represented by unit vectors $\ket{\psi}$ in a Hilbert space, $\lVert \psi \rVert=1$.
2. Physical quantities are represented by Hermitian operators. Whenever a measurement of this quantity is made, the result is one of the eigenvalues.

The physical state $\ket{\psi}$ is an eigenvector of operator $A$ if
$$A\ket{\psi_{n}}=\lambda_{n}\ket{\psi_{n}}.$$
The basis eigenvectors for any Hermitian operator are orthonormal and complete. 
The completeness relation is given by
$$\sum_{m}\ket{m}\bra{m}=\mathbb{I}.$$
We can write the wavefunction as
$$\psi_{m}(x)=\braket{ m | \psi }. $$
The probability of measuring $\lambda_{m}$ of the observable is described by the Hermitian operator $A$. This is the projection of the physical state onto the corresponding eigenvector of $A$
$$\mathrm{Pr}(\lambda_{m})=\lvert \braket{ m | \psi }   \rvert^2. $$
The expectation value of an observable $A$ is the average result in a given $\ket{\psi}$ state.
$$\braket{  A  } =\sum_{i}\lambda_{i}\mathrm{Pr}(\lambda_{i})=\sum_{i}\lambda_{i}\lvert \braket{ i | \psi }  \rvert^2=\sum_{i}\lambda_{i}\braket{ \psi | i }\braket{ i | \psi }=\braket{ \psi | \lambda_{i} \psi }=\bra{\psi}A\ket{\psi}.$$

