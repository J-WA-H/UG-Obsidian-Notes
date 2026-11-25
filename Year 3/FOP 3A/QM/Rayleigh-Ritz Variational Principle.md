The Rayleigh-Ritz variational principle states that for a normalised wavefunction $\Psi(\underline{r})$, the expectation of the Hamiltonian is greater than or equal to the ground state:
$$\bra{\Psi}\hat{H}\ket{\Psi} \geq \epsilon_{0}$$
$$\int d^3r\Psi^*(\underline{r})\hat{H}\Psi(\underline{r})\geq \epsilon_{0}$$Proof:
$$\langle\Psi|\Psi\rangle=1\implies \sum_{n,m}c_{m}^*c_{n}\langle\psi_{m}|\psi_{n}\rangle=\sum_{n,m}c^*_{m}c_{n}\delta_{nm}\implies\sum_{n}|c_{n}|^2=1$$
$$\bra{\Psi}\hat{H}\ket{\Psi}-\epsilon_{0}=\sum c_{m}^*\bra{\psi_{m}}\hat{H}\ket{\psi_{n}}c_{n}-\epsilon_{0}$$
$$=\sum_{n,m}c_{m}^*c_{n}\epsilon_{n}\langle\psi_{m}|\psi_{n}\rangle-\epsilon_{0}\cdot 1$$
$$=\sum_{n}|c_{n}|^2\epsilon_{n}-\epsilon_{0}\sum_{n}|c_{n}|^2$$
$$=\sum_{n}|c_{n}|^2(\epsilon_{n}-\epsilon_{0})\geq 0$$
as $\epsilon_{n}\geq \epsilon_{0}$.

Rayleigh-Ritz is used to approximate the lower bound on the ground state for a Hamiltonian that cannot be solved easily.

Example: (Potential well)
$$V(x)=\begin{cases}
0 & 0\leq x\leq L \\
\infty & \text{elsewhere}
\end{cases}$$
$$\hat{H}=-\frac{\hbar^2}{2m} \frac{d^2}{dx^2}.$$
This has wavefunctions and energy levels
$$\psi_{n}(x)=A\sin\left( \frac{n\pi x}{L} \right)$$
$$E_{n}=\frac{\hbar^2\pi^2n^2}{2mL^2}.$$
Define trial (unnormalised) wavefunction:
$$\phi(\lambda,x)=\begin{cases}
x(L-x)\left[ 1+\lambda\left( x-\frac{L}{2} \right)^2 \right] & 0\leq x\leq L \\
0 & \text{elsewhere}
\end{cases}$$
Take
$$E(\lambda)=\frac{\bra{\phi}\hat{H}\ket{\phi}}{\langle\phi|\phi\rangle}\geq \epsilon_{0}$$
$$-\frac{\frac{\hbar^2}{2m}\int_{0}^Ldx\;x(L-x)\left[ 1+\lambda\left( x-\frac{L}{2} \right)^2 \right] \frac{d^2}{dx^2}\left( x(L-x)\left[ 1+\lambda\left( x-\frac{L}{2} \right)^2 \right] \right)}{\int_{0}^Ldx'\left[ x'(L-x')\left[ 1+\lambda\left( x'-\frac{L}{2} \right)^2 \right] \right]^2}$$
$$\implies E(\lambda)=\frac{3\hbar^2}{mL^2} \frac{11a^4\lambda^2+14a^2+35}{a^4\lambda^2+6a^2\lambda+21}.$$
The ground state is where $E(\lambda)$ is minimised:
$$\frac{dE}{d\lambda}=\frac{3\hbar^2}{mL^2} \frac{13a^2\lambda^2+98a^2\lambda+21}{(\dots)^2}=0$$
where $a=\frac{L}{2}$, and we take $L=1$. As we are minimising $E(\lambda)$, the denominator doesn't matter so it hasn't been evaluated.
$$13a^2\lambda^2+98a^2\lambda+21=0$$
Solving for $\lambda$ gives
$$\lambda_{+}=\frac{-49+\sqrt{ 2128 }}{13a^2}\approx-0.883$$
$$\lambda_-=\frac{-49-\sqrt{ 2128 }}{13a^2}\approx-29.3.$$
Substituting these solutions into $E(\lambda)$ gives:
$$E(\lambda_{+})=\frac{4.9\hbar^2}{mL^2};\;E(\lambda_{-})=\frac{51.1\hbar^2}{mL^2}.$$
The true energy level is $$E=\frac{\hbar^2\pi^2}{2mL^2}=\frac{4.9\hbar^2}{mL^2}\approx E(\lambda_{+})$$
