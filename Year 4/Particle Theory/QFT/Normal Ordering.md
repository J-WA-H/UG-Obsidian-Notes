In general, we can have an operator ordering ambiguity. Rewriting a general operator $\hat{O}$ in terms of [creation and annihilation](Quantisation%20of%20Fields.md ) operators, normal ordering moves all creation operators left and all annihilation operators right, for example
$$:\hat{a}\hat{a}^{\dagger}:\;=\;:\hat{a}^{\dagger}\hat{a}:\;=\hat{a}^{\dagger}\hat{a}.\tag{5.1} $$
This can be used to fix the issue with the infinite term in the Hamiltonian $(4.18)$,
$$:\hat{H}:\;=\int \frac{d^3k}{(2\pi)^32E_{k}}E_{k} \frac{1}{2}:(\hat{a}^{\dagger}_{k}\hat{a}_{k}+\hat{a}_{k}\hat{a}_{k}^{\dagger}):\tag{5.2} $$
Evaluating this gives
$$\hat{H}\to\;:\hat{H}:\;=\int \frac{d^3k}{(2\pi)^32E_{k}}E_{k}\hat{a}_{k}^{\dagger}\hat{a}_{k}.\tag{5.3} $$
The commutator relations are then
$$\begin{matrix}
[\hat{H},\hat{a}^{\dagger}_{k}]=E_{k}\hat{a}^{\dagger}_{k} \\
[\hat{H},\hat{a}_{k}]=-E_{k}\hat{a}_{k}
\end{matrix}\tag{5.4}. $$
If we rake a state $\ket{\psi_{n}}$ from the Hilbert space of states with relation $\hat{H}\ket{\psi_{n}}=E_{n}\ket{\psi_{n}}$. Consider $\hat{a}^{\dagger}_{k}\ket{\psi_{n}}$,
$$\hat{H}\circ \hat{a}^{\dagger}_{k}\ket{\psi_{n}} =\hat{a}_{k}^{\dagger}\hat{H}\ket{\psi_{n}}+E_{k}\hat{a}^{\dagger}_{k}\ket{\psi_{n}} = \hat{a}^{\dagger}_{k}(E_{n}+E_{k})\ket{\psi_{n}}  .\tag{5.5} $$
This shows that $\hat{a}^{\dagger}$ raises the energy of a state by $E_{k}$, or equivalently creates a particle of energy $E_{k}$ so $\hat{a}^{\dagger}$ is a creation operator. It is then trivial to show that $\hat{a}$ is the annihilation operator.

The Hilbert space of multiparticle states is known as a Fock space $\mathcal{H}$.
1. Define the vacuum state (ground state) as $\ket{0}\in \mathcal{H}$. $\forall\;\vec{k}$, $\hat{a}_{k}\ket{0}=0$ and $\braket{ 0 | 0 }=1$.
2. Construct a 1-particle state $\ket{1}=\hat{a}^{\dagger}_{k}\ket{0}$. Another way to denote this is $\ket{1}\equiv \ket{\vec{k}}$.
$$\hat{H}\ket{1} = \int \frac{d^3p}{(2\pi)^32E_{p}}E_{p}(\hat{a}^{\dagger}_{p}\hat{a}_{p})\hat{a}^{\dagger}_{k}\ket{0} =\int \frac{d^3p}{(2\pi)^32E_{p}}E_{p}(\cancelto{0}{\hat{a}^{\dagger}_{k}\hat{a}_{p}}+2E_{k}(2\pi)^3\delta^{(3)}(\vec{p}-\vec{k}))\hat{a}^{\dagger}_{p}\ket{0} \tag{5.6} .$$Simplifying this gives
$$=\int d^3pE_{k}\delta^{(3)}(\vec{p}-\vec{k})\hat{a}^{\dagger}_{p}\ket{0}=E_{k}\hat{a}^{\dagger}_{k}\ket{0} = E_{k}\ket{1} .\tag{5.7} $$
A similar process can be used to find an $n$ particle state
$$\ket{n} =\hat{a}^{\dagger}_{k_{1}}\hat{a}^{\dagger}_{k_{2}}\dots \hat{a}^{\dagger}_{k_{n}}\ket{0} .\tag{5.8} $$
CHECK HOW TO NORMALISE