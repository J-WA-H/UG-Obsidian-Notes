Consider the Schrodinger equation
$$\left( -\frac{\hbar^2}{2m}\nabla^2+V(\underline{r}) \right)\psi=E\psi.$$
For a crystal, $V(\underline{r})$ is periodic so can be expressed as a Fourier series
$$V(\underline{r})=\sum_{\underline{G}'}V_{G'}e^{i\underline{G}'\cdot \underline{r}}.$$
Ansatz:
$$\psi(\underline{r})=\sum_{\underline{G}}C_{G}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}.$$
$$\nabla^2\psi=\sum_{\underline{G}}-C_{G}\lvert \underline{k}+\underline{G} \rvert^2 e^{i(\underline{k}+\underline{G})\cdot \underline{r}}. $$
Substituting this into the Schrodinger equation gives
$$\sum_{\underline{G}}\left( \frac{\hbar^2}{2m}|\underline{k}+\underline{G}|^2-E \right)C_{G}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}+\sum_{\underline{G},\underline{G}'}V_{G'}C_{G}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}e^{i\underline{G}'\cdot \underline{r}}=0$$
Shifting $\underline{G}\to \underline{G}-\underline{G}'$:
$$\sum_{\underline{G}}\left( \frac{\hbar^2}{2m}|\underline{k}+\underline{G}|^2-E \right)C_{G}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}+\sum_{\underline{G},\underline{G}'} V_{G'}C_{G-G'}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}=0$$
$$\implies \sum_{\underline{G}}\left\{ \left( \frac{\hbar^2}{2m}|\underline{k}+\underline{G}|^2-E \right)C_{G}+\sum_{G'}V_{G'}C_{G-G'} \right\}e^{i(\underline{k}+\underline{G})\cdot \underline{r}}=0$$
$$\implies \left( \frac{\hbar^2}{2m}|\underline{k}+\underline{G}|^2-E \right)C_{G}+\sum_{G'}V_{G'}C_{G-G'}=0.$$
This is the Characteristic Bloch wave equation.

Implications:
$$\psi(\underline{r})=\sum_{G}C_{G}e^{o(\underline{k}+\underline{G})\cdot \underline{r}}=\left[ \sum_{G}e^{i\underline{G}\cdot \underline{r}} \right]e^{i\underline{k}\cdot \underline{r}}=U(\underline{r})e^{i\underline{k}\cdot \underline{r}}$$
$$\therefore \psi(\underline{r})=U(\underline{r})e^{i\underline{k}\cdot \underline{r}}$$
where $U(\underline{r})$ is known as the atomic part
Consider the translation vector $\underline{T}$:
$$U(\underline{r}+\underline{T})=\left[ \sum_{G}C_{G}e^{i\underline{G}\cdot \underline{r}} \right]e^{i\underline{G}\cdot \underline{T}}=U(\underline{r})e^{i\underline{G}\cdot T}.$$
$\underline{G}\cdot \underline{T}=2n\pi \implies e^{i\underline{G}\cdot \underline{T}}=e^{i(2n\pi)}=1$
$$\therefore U(\underline{r}+\underline{T})=U(\underline{r}).$$
$U(\underline{r})$ is a periodic function with the same periodicity as the lattice - hence why it is known as the atomic part.

A Bloch wave can travel over large distances as it is not a decaying function.