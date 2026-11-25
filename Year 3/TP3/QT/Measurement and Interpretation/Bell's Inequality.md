Generalise the [[Einstein-Podolsky-Rosen Paradox]] so the spin detectors are in arbitrary directions.
Consider the electron spin with respect to $\underline{a}$ and the positron with spin with respect to $\underline{b}$.

Measure the quantum mechanical average of the product of the two spins, In the EPR case, $\underline{a}=\underline{b}=\underline{\hat{z}}$.
$$\mathrm{Pr}(\underline{a},\underline{b})=-1$$
If $\underline{a}=-\underline{b}$,
$$\mathrm{Pr}(\underline{a},\underline{b})=1.$$
In general, for arbitrary directions, $\mathrm{Pr}(\underline{a},\underline{b})=-\underline{a}\cdot \underline{b}$.

Consider a general hidden variable theory we have wavefunction $\psi$ and hidden variable $\lambda$:
$A(\underline{a},\lambda)$ result of measuring the electron spin relative to $\underline{a}$.
$B(\underline{b},\lambda)$ result of measuring the positron spin with respect to $\underline{b}$.

The average of the product of the spins is
$$\mathrm{Pr}(\underline{a},\underline{b})=\int \rho(\lambda)A(\underline{a},\lambda)B(\underline{b},\lambda)d\lambda.$$
$\rho(\lambda)$ is the unknown probability density satisfied by $\lambda$.

For $B(\underline{b},\lambda)=-A(\underline{b},\lambda)$,
$$\mathrm{Pr}(\underline{a},\underline{b})=-\int d\lambda \rho(\lambda)A(\underline{a},\lambda)A(\underline{b},\lambda)$$
If we take another direction $\underline{c}$,
$$\mathrm{Pr}(\underline{a},\underline{b})-\mathrm{Pr}(\underline{b},\underline{c})=-\int d\lambda \rho(\lambda)(A(\underline{a},\lambda)A(\underline{b},\lambda)-A(\underline{a},\lambda)A(\underline{c},\lambda))$$
$|A(\underline{b},\lambda)|^2=1$ so
$$=-\int \rho(\lambda)d\lambda A(\underline{a},\lambda)A(\underline{b},\lambda)(1-A(\underline{b},\lambda)A(\underline{c},\lambda))$$
so we can write
$$|\mathrm{Pr}(\underline{a},\underline{b})-\mathrm{Pr}(\underline{a},\underline{c})|\leq \int d\lambda \rho(\lambda)(1-A(\underline{a},\lambda)A(\underline{c},\lambda))\leq 1-\mathrm{Pr}(\underline{b},\underline{c}).$$
This is Bell's inequality:
$$|\mathrm{Pr}(\underline{a},\underline{b})-\mathrm{Pr}(\underline{a},\underline{c})|\leq 1-\mathrm{Pr}(\underline{b},\underline{c}).$$
Quantum mechanics does not satisfy this
$$|\underline{a}\cdot \underline{b}-\underline{a}\cdot \underline{c}|\leq 1-\underline{b}\cdot \underline{c}.$$
Consider that $\underline{a},\underline{b},\underline{c}$ in a plane where $\underline{a}\perp \underline{b}$ and $\underline{c}$ is at $45^{\circ}$.
$$|0-1.\sqrt{ 2 }|\leq 1-\frac{1}{\sqrt{ 2 }}$$
This predicts $0.707\leq 0.29$ which is not true.

This implies hidden variable theory and quantum mechanics give different predictions and all measurements agree with quantum mechanics and not hidden variable theory.
