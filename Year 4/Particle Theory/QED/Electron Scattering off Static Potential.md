Consider the static potential
$$A^0(x)=-\frac{Ze}{4\pi |x|}\tag{8.1} .$$
![[Pasted image 20260113184313.png]]
The Feynman diagram does not include the propagation of a photon as the potential is static. The interaction Hamiltonian is
$$H_{int}=-ie \int d^4x\; \bar{\psi}_{f}(x)\gamma^\mu \psi_{i}(x)A_{\mu}(x)$$The [transition matrix element](Time%20Evolution.md) is given by, using the LSZ reduction formula,
$$S_{fi}=-ie \int d^4x \;\bar{\psi}_{f}(x)\gamma^\mu \psi_{i}(x)A_{\mu}(x)\tag{8.2} =\frac{iZe^2}{4\pi}\int dt \frac{d^3x}{|x|}\bar{u}_{k}(p_{f})\gamma^0u_{\ell}(p_{i})e^{ i(p_{f}-p_{i})x}=\frac{iZe^2}{4\pi}\int dt \;\bar{u}_{k}(p_{f})\gamma^0u_{\ell}(p_{i}) \frac{4\pi e^{ i(E_{f}-E_{i})t }}{|p_{f}-p_{i}|^2}.$$
We need to obtain $|S_{fi}|^2$ to get the cross-section. Consider
$$\frac{1}{2}\sum_{k,\ell=1}^2 |\bar{u}_{\alpha}^k(p_{f})\gamma^0u^\ell_{\beta}(p_{i})|^2.\tag{8.3} $$Here we are summing over all spin states, and Dirac indices $\alpha,\beta$ are shown.
$$\frac{1}{2}\sum_{k,\ell}^2[\bar{u}_{\alpha}^k(p_{f})\gamma^0_{\alpha\beta}u^\ell_{\beta}(p_{i})\bar{u}^\ell_{\gamma}(p_{i})\gamma^0_{\gamma\delta}u^k_{\delta}(p_{f})].\tag{8.4}$$Given that $u^\ell_{\beta}(p_{i})\bar{u}^\ell_{\gamma}(p_{i})=[p\!\!\!/_{i}+m]_{\beta\gamma}$, and bringing the final term $u^k_{\delta}(p_{f})$ to the front gives
$$\frac{1}{2}\sum_{k,\ell=1}^2[[p\!\!\!/_{f}+m]_{\delta\alpha}\gamma^0_{\alpha\beta}[p\!\!\!/_{i}+m]_{\beta\gamma}\gamma^0_{\gamma\delta}]=\frac{1}{2}\mathrm{Tr}[(p\!\!\!/_{f}+m)\gamma^0(p\!\!\!/_{i}+m)\gamma^0]=2(2p_{f}^0p_{i}^0-(p_{f\mu}p_{i}^{\mu}-m^2)).\tag{8.5} $$
We also need to consider the exponential, which gives a $\delta$-function,
$$\left[ \int dt\;e^{ i(E_{f}-E_{i})t } \right]^2=[2\pi\delta(E_{f}-E_{i})]^2=2\pi\delta(E_{f}-E_{i})2\pi\delta(0)\tag{8.6} $$where $2\pi\delta(0)=T$, the time of the experiment, which is taken to be large. $\delta(0)$ is used as the first $\delta$-function ensures that $E_{f}=E_{i}$. 

The incident flux is given by
$$j^a=\bar{\psi}(x)\gamma^a\psi(x)=\frac{1}{2}\sum_{k}\bar{u}^{(k)}(p_{i})\gamma^au^{(k)}(p_{i})e^{ -ip_{i}x }\tag{8.7} .$$
For $a=z$, $j^z=2|p_{i}|$
$$\therefore \sigma=\frac{P_{i\to f}}{2|p_{i}|T} \frac{Z^2e^4}{2|p_{i}|}\int \frac{d^3p_{f}}{(2\pi)^32p_{f}} \frac{1}{2}\sum_{k,\ell} \frac{|\bar{u}(p_{f})\gamma^0u(p_{i})|^2}{|\vec{p}_{f}-\vec{p}_{i}|^4} \frac{(2\pi)^2\delta(E_{f}-E_{i})^2}{2\pi T}\tag{8.8} $$
$$=\frac{Z^2e^4}{2|p_{i}|}\int \frac{|p_{f}|^2dp_{f}d^2\Omega}{(2\pi)^32E_{f}} \frac{8E_{f}E_{i}-4p_{f}p_{i}+4m^2}{|p_{f}-p_{i}|^4}2\pi\delta(E_{f}-E_{i})\tag{8.9} .$$
Consider $|p_{f}|^2d|p_{F}|d^2\Omega$ element. It is equivalent to $|p_{f}|E_{f}dE_{f}d\phi d\cos \theta$. From momentum conservation, $E_{f}=E_{i}$ which simplifies the integral to an integral over $\cos \theta$, as the $\delta$-function. To evaluate the difference in the momentum,
$$\vec{p}_{f}=|\vec{p}_{i}|\begin{bmatrix}
\sin \theta \\
0 \\
\cos \theta
\end{bmatrix},\;\vec{p}_{i}=|\vec{p}_{i}|\begin{bmatrix}
0 \\
0 \\
1
\end{bmatrix}\tag{8.10} .$$This gives
$$|\vec{p}_{f}-\vec{p}_{i}|^2=|\vec{p}_{i}|^2(\sin^2\theta-(\cos\theta-1)^2)=2-2\cos \theta=2(1-\cos \theta).\tag{8.11} $$
$$\therefore|\vec{p}_{f}-\vec{p}_{i}|^4=4|p_{i}|^4(1-\cos \theta)^2\tag{8.12}. $$
This gives
$$\sigma=\frac{Z^2e^4}{8\pi}\int_{-1}^{\cos \theta_{max}}d\cos \theta \frac{{2E_{i}^2-(E_{i}^2-|p_{i}|^2\cos\theta-m^2)}}{|p_{i}|^4(1-\cos \theta)^2}\tag{8.13} .$$
This gives the differential cross-section
$$\frac{d\sigma}{d\Omega}=\frac{Z^2e^4}{4}\frac{{2E_{i}^2-(E_{i}^2-|p_{i}|^2\cos\theta-m^2)}}{|p_{i}|^4(1-\cos \theta)^2}$$
In general,
$$\sigma=\frac{1}{2|\vec{p}_{i}| T}\int \frac{|\vec{p}_{f}|E_{f}dE_{f}d^2\Omega}{(2\pi)^32E_{f}} \frac{1}{2}\sum_{k,\ell}|S_{fi}|^2\tag{8.14} $$
