The [[Method of Partial Waves]] can't always be used as it is generally hard to solve the Schrodinger equation or it may need many partial waves.
The integral equation aims to re express the Schrodinger equation for [[Potential Scattering]].
$$[\nabla^2+k^2-U(\underline{r})]\psi=0.$$
This will be expressed using Greens functions:
Rearrange to
$$[\nabla^2+k^2]\psi=U(\underline{r})\psi.$$
We can express the solution to this as
$$\psi(\underline{r})=\psi_{0}(\underline{r})+\int G_{0}(k,\underline{r}-\underline{r}')U(\underline{r}')\psi(\underline{r}')d^3r'$$
where $\psi_{0}$ is the solution to $[\nabla^2+k^2]\psi_{0}=0$ and
$$(\nabla^2+k^2)G_{0}(k,\underline{r}-\underline{r}')=\delta^3(\underline{r}-\underline{r}').$$
Check this is a solution:
$$[\nabla^2+k^2]\psi(\underline{r})=[\nabla^2+k^2]\psi_{0}(\underline{r})+\int(\nabla^2+k^2)G_{0}(k.\underline{r}-\underline{r}')U(\underline{r}')\psi(\underline{r}')d^3r'$$
$$=0+\int\delta^3(\underline{r}-\underline{r}')U(\underline{r}')\psi(\underline{r}')d^3r'=U(\underline{r})\psi(\underline{r})\;\square.$$
To solve this, we first know that $\psi_{0}$ is a plane wave, $\psi_{0\underline{k}}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}$.
$$\psi_{\underline{k}}(\underline{r})=e^{i\underline{k}\cdot \underline{r}}+\int G(k,\underline{r}-\underline{r}')U(\underline{r}')\psi(\underline{r}')d^3r'.$$
Now solve for the Green's function:
$$(\nabla^2+k^2)G_{0}(k,\underline{r}-\underline{r}')=\delta^3(\underline{r}-\underline{r}').$$
Take [[Fourier Transform]]:
$$G_{0}(k,\underline{r}-\underline{r}')=\int \frac{d^3q}{(2\pi)^3}\tilde{G}_{0}(k,\underline{q})e^{i\underline{q}\cdot(\underline{r}-\underline{r}')}.$$
In Fourier space, $\nabla^2=-q^2$ so
$$\int \frac{d^3q}{(2\pi)^3}(k^2-q^2)\tilde{G}_{0}(k,\underline{q})e^{i\underline{q}\cdot(\underline{r}-\underline{r}')}=\int \frac{d^3q}{(2\pi)^3}e^{i\underline{q}\cdot (\underline{r}-\underline{r}')}$$
$$\implies (k^2-q^2)\tilde{G}_{0}(k,\underline{q})=1$$
$$\implies \tilde{G}_{0}(k,\underline{q})=\frac{1}{k^2-q^2}.$$
Perform inverse Fourier transform:
$$G_{0}(k,\underline{r}-\underline{r}')=\int \frac{d^3q}{(2\pi)^3} \frac{1}{k^2-q^2} e^{i\underline{q}\cdot(\underline{r}-\underline{r}')}$$
$$=\int \frac{d^3q}{(2\pi)^3} \frac{1}{k^2-q^2}e^{iq|\underline{r}-\underline{r}'|\cos \theta}=\int_{0}^{2\pi}d\phi \int_{-1}^{1}d\cos \theta \int_{0}^{\infty} \frac{q^2dq}{k^2-q^2} e^{iq|\underline{r}-\underline{r}'|\cos \theta}$$
$$= \frac{2\pi}{(2\pi)^3} \frac{1}{iq|\underline{r}-\underline{r}'|} \int_{0}^{\infty} \frac{q^2dq}{k^2-q^2}[e^{iq|\underline{r}-\underline{r}'|\cos \theta}]_{-1}^{1}$$
$$=\frac{1}{(2\pi)^2i|\underline{r}-\underline{r}'|}\int_{0}^{\infty} \frac{qdq}{k^2-q^2}(e^{iq|\underline{r}-\underline{r}'|}-e^{-iq|\underline{r}-\underline{r}'|}).$$
Consider
$$-\int_{0}^{\infty} \frac{qdq}{k^2-q^2}e^{iq|\underline{r}-\underline{r}'|}.$$
Set $q=-q'$
$$-\int_{0}^{-\infty} \frac{q'dq'}{k^2-q'^2}e^{iq'|\underline{r}-\underline{r}'|}=\int_{-\infty}^{0} \frac{q'dq'}{k^2-q'^2}e^{iq'|\underline{r}-\underline{r}'|}$$
$$\therefore G_{0}(k,\underline{r}-\underline{r}')= \frac{1}{4\pi^2i|\underline{r}-\underline{r}'|}\int_{-\infty}^{\infty} \frac{qdq}{k^2-q^2-i\varepsilon}e^{iq|\underline{r}-\underline{r}'|}$$
where $\varepsilon\to 0$.
Using partial fractions:
$$G_{0}(k,\underline{r}-\underline{r}')=-\frac{1}{4\pi |\underline{r}-\underline{r}'|} \frac{1}{2\pi i}\int_{-\infty}^{\infty} e^{iq|\underline{r}-\underline{r}'|}\left( \frac{1}{q-k-i\varepsilon}+\frac{1}{q+k+i\varepsilon} \right)dq.$$
Using [[Residue Theorem]]:
$$I=-\frac{1}{4\pi |\underline{r}-\underline{r}'|} \frac{1}{2\pi i} \oint_{C} e^{iq|\underline{r}-\underline{r}'|}dq\left( \frac{1}{q-k-i\varepsilon}+\frac{1}{q+k+i\varepsilon} \right).$$
![[Pasted image 20250128193121.png]]
The poles of this function are at $q=\pm(k+i\varepsilon)$.
The only pole contained in the contour is $q=k+i\varepsilon$.
$$\text{Res}\left[ \frac{1}{q^2-k^2+i\varepsilon},k+i\varepsilon \right]=1$$
$$\therefore I=2\pi i\left( -\frac{1}{4\pi} \right) \frac{1}{|\underline{r}-\underline{r}'|} \frac{1}{2\pi i} e^{ik(\underline{r}-\underline{r}')}=-\frac{e^{ik|\underline{r}-\underline{r}'|}}{4\pi |\underline{r}-\underline{r}'|}.$$
This gives the Green's function as
$$G_{0}(k,\underline{r}-\underline{r}')=-\frac{e^{ik|\underline{r}-\underline{r}'|}}{4\pi |\underline{r}-\underline{r}'|}.$$
