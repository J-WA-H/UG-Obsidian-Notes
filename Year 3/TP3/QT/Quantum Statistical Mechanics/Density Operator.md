Consider an ensemble of $N$ subsystems, $\alpha=1,2,\dots ,N$. Each system is in a normalised [pure state](Pure%20and%20Mixed%20States.md), $\ket{\alpha}$ s.t. $\braket{ \alpha | \alpha }=1$.

In a pure state, all subsystems are in the same state. 

In a mixed state, the subsystems are in different states.

Take the complete state of basis states $\ket{n}$ s.t. $\braket{ n | n' }=\delta_{nn'}$ or $\delta(n-n')$ if $n$ is continuous.
For a complete basis,
$$\mathbb{I}=\sum_{n}\ket{n}\bra{n}.$$
This can be used to expand $\ket{\alpha}$:
$$\ket{\alpha} =\sum_{n}\ket{n}\braket{ n | \alpha }=\sum_{n}c_{n}^{\alpha}\ket{n}   $$
where $c_{n}^{\alpha}=\braket{ n | \alpha }$ and 
$$\sum_{n}|c_{n}^{\alpha}|^2=1.$$
The expectation value of an operator $\hat{A}$ on a state is given by
$$\langle A \rangle_{\alpha}=\bra{\alpha}A\ket{\alpha}=\sum_{nn'}c_{n'}^{\alpha*}\bra{n'}A\ket{n}c^{\alpha}_{n}=\sum_{nn'}\braket{ n | \alpha }\braket{ \alpha | n' } \bra{n'} A\ket{n}.$$
This is only the expectation value of one subsystem so for all subsystems,
$$\langle A \rangle =\sum_{\alpha=1}^{N}W_{\alpha}\langle A \rangle _{\alpha}.$$
$W_{\alpha}$ is the statistical weight of the pure state - the probability of finding the whole system in state $\ket{\alpha}$.
$$\langle A \rangle =\sum_{\alpha=1}^{N}W_{\alpha}\sum_{nn'}\braket{ n | \alpha } \braket{ \alpha | n' }\bra{n'} A \ket{n}=\sum_{\alpha=1}^{N}\sum_{nn'}\braket{ n | \alpha } W_{\alpha}\braket{ \alpha | n' } \bra{n'} A \ket{n}.$$
This defines the density operator
$$\rho=\sum_{\alpha=1}^{N}\ket{\alpha}W_{\alpha}\bra{\alpha}.$$
This allows us to rewrite $\langle A \rangle$,
$$\langle A \rangle =\sum_{nn'}\bra{n}\rho \ket{n'}\bra{n'}A\ket{n}=\sum_{nn'}\bra{n}\rho A\ket{n}=\text{Tr}(\rho A).$$
This gives the the expectation as a trace.
$$\langle A \rangle =\text{Tr}(\rho A).$$
The density operator:
- Allows us to calculate ensemble averages
- If $A=\mathbb{I}$, $\langle \mathbb{I} \rangle=1=\text{Tr}(\rho\mathbb{I})=\text{Tr}(\rho)$. The density operator is normalised such that $\text{Tr}(\rho)=1$.

If the states are not normalised, 
$$\langle A \rangle =\frac{\text{Tr}(A\rho)}{\text{Tr}(\rho)}.$$
We can express it in terms of the density matrix,
$$\rho_{nn'}=\bra{n}\rho \ket{n'} \sum_{\alpha=1}^N\braket{ n | \alpha } W_{\alpha}\braket{ \alpha | n' } =\sum_{\alpha=1}^NW_{\alpha}c_{n'}^{\alpha*}c_{n}^{\alpha}.$$
