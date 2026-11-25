The main properties of the [[Density Operator]] are:
- The diagonal elements, $$\rho_{nn}=\bra{n}\rho\ket{n}=\sum_{\alpha=1}^NW_{\alpha}|c_{n}^{\alpha}|^2.$$
	Since $W_{\alpha}$ is the probability of the system being in state $\alpha$, and $c_{n}^{\alpha}$ is the probability of the state $\alpha$ being in state $n$.
	This means that $\rho_{nn}$ is the probability of the while system being in the state $n$.
- The density matrix is Hermitian, $\bra{n}\rho \ket{n'}=\bra{n'}\rho \ket{n}$ so it can be diagonalised by a unitary operator.
- If $\rho$ is diagonalised, $\rho_{kk'}=\rho_{kk}\delta_{kk'}\implies\text{Tr}(\rho^2)\leq\text{Tr}(\rho)$.
	$$\text{Tr}(\rho)=\sum_{k=1}^n\rho_{kk};\;\text{Tr}(\rho^2)=\sum_{k=1}^n\rho_{kk}^2.$$
	As $\rho_{kk}<1$, $\rho_{kk}^2\leq \rho_{kk}\implies\text{Tr}(\rho^2)\leq\text{Tr}(\rho)$.
In any representation,
$$\sum_{nn'}|\rho_{nn'}|^2\leq 1.$$
If the whole system is in a [pure state](Pure%20and%20Mixed%20States.md), $\rho^{\lambda}=\ket{\lambda}\bra{\lambda}$.
Consider the projection onto $\ket{\lambda}$,
$$(\rho^{\lambda})^2=\rho^{\lambda}\implies\text{Tr}(\rho)=1.$$
If we are in a pure state then $\langle A \rangle=\bra{\lambda}A\ket{\lambda}$ and $\rho^{\lambda}_{kk'}=\delta_{k\lambda}\delta_{\lambda k'}$.

In a pure state the matrix can be written such that one diagonal element is 1 and the rest are 0.

If there is more than one non-zero diagonal element, there is a rotation to give only one non-zero diagonal element.

Often we are only interested in some subset of variables, e.g. spin, so we omit the dependence on $\rho$ of the other variables. This gives the reduced density matrix.
