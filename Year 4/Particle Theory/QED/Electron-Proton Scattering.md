Consider the Feynman diagram for an electron scattering off a proton
![[Pasted image 20260120140742.png]]
the points $x,y$ give the interactions, each contributing $-iee_{f}\gamma^\mu$ from Feynman rules and using the [[Photon Propagator]] to represent the internal line. The transition element is
$$S_{fi}=\int d^4xd^4y\,j^{(e)}_{\mu}(x)j^{(p)}_{\nu}(y)D^{\mu \nu}(x-y)\tag{9.1} $$$$=ie^2e_{e}e_{f} \frac{g^{\mu \nu}}{q^2} \bar{u}(p_{3})\gamma_{\mu}u(p_{1})\bar{u}(p_{4})\gamma_{\nu}u(p_{2})(2\pi)^4\delta^{(4)}(p_{1}+p_{2}-p_{3}-p_{4})\tag{9.2} $$
To square the matrix element, first consider the spinors. For the electron node, with polarisations $\lambda_{e}$,
$$\frac{1}{2}\sum_{\lambda_{e}}|\bar{u}(p_{3})\gamma_{\mu}u(p_{1})|^2=_{m_{e}=0} \frac{1}{2}\mathrm{Tr}[p\!\!\!/_{3}\gamma_{\mu}p\!\!\!/_{1}\gamma_{\mu'}]=2(p_{3\mu}p_{1\mu'}+p_{3\mu'}p_{1\mu}-g_{\mu \mu'}(p_{1}p_{3}))\tag{9.3} $$
For the proton node,
$$\frac{1}{2}\sum_{\lambda_{p}}|\bar{u}(p_{4})\gamma_{\nu}u(p_{2})|^2=_{m_{p}=0} \frac{1}{2}\mathrm{Tr}[p\!\!\!/_{4}\gamma_{\nu}p\!\!\!/_{3}\gamma_{\nu'}]=2(p_{4\nu}p_{2\nu'}+p_{4\nu'}p_{2\nu}-g_{\nu \nu'}(p_{2}p_{4}))\tag{9.4}. $$
Combining these gives
$$2(p_{3}p_{4})(p_{1}p_{2})+2(p_{1}p_{4})(p_{2}p_{3})+(4-4)(p_{1}p_{3})(p_{2}p_{4}).\tag{9.5} $$
This is contacted by $g^{\mu \nu}g^{\mu'\nu'}$.
$$\therefore \sum_{\lambda}|S_{fi}|^2=2e^4e_{e}^2e_{p}^2[(p_{1}p_{2})(p_{3}p_{4})+(p_{1}p_{4})(p_{2}p_{3})](2\pi)^4\delta(p_{1}+p_{2}-p_{3}-p_{4})\tag{9.6} $$
The second $\delta$-function $\delta(0)$ is neglected as it will cancel out later.

For the incident flux, consider the product of the currents,
$$j_{e}(x)j_{p}(x)=\bar{\psi}_{e}(x)\gamma^3\psi_{e}(x)\bar{\psi}_{p}(x)\gamma^3\psi_{p}(x)=m_{p}|\vec{p}_{1}|\tag{9.7} .$$
This assumes the proton is stationary and the electron is aligned along the $z$-axis.
To make this Lorentz invariant,
$$m_{p}|\vec{p}_{1}|=\sqrt{ E_{1}^2E_{2}^2-m_{1}^2m_{2}^2 }=\sqrt{ (p_{1}p_{2})^2-\underbrace{p_{1}^2p_{2}^2}_{\sim 9} }.\tag{9.8} $$
This gives the cross-section
$$d\sigma=\frac{(2\pi)^4\delta^{(4)}(p_{1}+p_{2}-p_{3}-p_{4})}{4\sqrt{ (p_{1}p_{2})^2-p_{1}^2p_{2}^2 }} \frac{d^3p_{3}}{(2\pi)^32E_{3}} \frac{d^3p_{4}}{(2\pi)^32E_{4}}\sum_{\lambda}|S_{fi}|^2\tag{9.9}.$$
This has mass dimension $[m^{-2}]$. Consider the centre of mass system,
$$p_{1,2}=\begin{bmatrix}
E_{1,2}=\sqrt{ p_{z}^2+m_{1,2}^2 } \\
0 \\
0 \\
\pm p_{z}
\end{bmatrix};\;\;p_{3,4}=\begin{bmatrix}
E_{3,4} \\
\pm |\vec{p}|\sin \theta \cos \phi \\
\pm |\vec{p}|\sin \theta \sin \phi \\
\pm |\vec{p}|\cos \theta
\end{bmatrix}.\tag{9.10} $$
Consider the $\delta$-function and the volume element,
$$(2\pi)^{\cancel{4}^1}\delta(E_{1}+E_{2}-E_{3}-E_{4})\cancel{\delta^{(3)}(\vec{p}_{1}+\vec{p}_{2}-\vec{p}_{3}-\vec{p}_{4})} \frac{d^3p_{3}}{\cancel{(2\pi)^3}2E_{3}} \frac{\cancel{d^3p_{3}}}{(2\pi)^32E_{4}}\tag{9.11} .$$From the $\delta$-function, $\vec{p}_{4}=\vec{p}_{1}+\vec{p}_{3}-\vec{p}_{3}=-\vec{p}_{3}$ in the centre of mass frame. We can rewrite $d^3p_{3}=d^2\Omega_{3}d|\vec{p}_{3}|$ and $d|\vec{p}_{3}|=|\vec{p}_{3}|E_{3}dE_{3}$.
$$(2\pi)\delta(E_{1}+E_{2}-E_{3}-E_{4}) \frac{d^2\Omega_{3}}{(2\pi)^3} \frac{\cancel{E_{3}}|\vec{p}_{3}|}{2\cancel{E_{3}}E_{4}}dE_{3}\tag{9.12}. $$
This gives $E_{3}=E_{1}+E_{2}-E_{4}=E_{1}+E_{2}-\sqrt{ |\vec{p}_{3}|^2+m_{4}^2 }=E_{1}+E_{2}-\sqrt{ E_{3}^2-m_{3}^2+m_{4}^2 }\implies 2E_{3}=E_{1}+E_{2}$.