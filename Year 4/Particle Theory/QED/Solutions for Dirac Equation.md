With the covariant form of the [[Dirac Equation]],
$$(i\partial \!\!\!/-m)\psi=0\tag{1.8}, $$it can be solved in a similar way to the [Klein-Gordon equation](Hamiltonian%20Formulism.md),
$$\psi_{\eta}(x)=\int \frac{d^3p}{(2\pi)^3}[e^{ -ip_{\mu}x^{\mu} }u_{\eta}(\vec{p})+e^{ ip_{\mu}x^{\mu} }v_{\eta}(\vec{p})]\tag{2.1} $$
with spinor index $\eta=1,2,3,4$.

Recall $\partial \!\!\!/=\partial_{\mu}\gamma^{\mu}$ this implies the Fourier transform of $i\partial \!\!\!/\to p_{\mu}\gamma^{\mu}=p\!\!\!/$. When $\vec{p}=0$, $p_{\mu}=\vec{0}$, $p_{\mu}\gamma^{\mu}=E\gamma^{0}=m\gamma^{0}$. For a particle at rest, this gives the Dirac equation,
$$m(\gamma^{0}-1)u_{\eta}(\vec{p}=\vec{0})=0.\tag{2.2} $$
$$(\gamma^{0}-1)u_{\eta}=\left(\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & -1 & 0 \\
0 & 0 & 0 & -1
\end{bmatrix}-\begin{bmatrix}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0 \\
0 & 0 & 1 & 0 \\
0 & 0 & 0 & 1
\end{bmatrix}\right)u_{\eta}=0\tag{2.3} .$$
Solving this gives a positive and negative spin state $+/-$,
$$u_{\eta}^{(+)}(0)=\begin{bmatrix}
1 \\
0 \\
0 \\
0
\end{bmatrix},\;u_{\eta}^{(-)}(0)=\begin{bmatrix}
0 \\
1 \\
0 \\
0
\end{bmatrix}.\tag{2.4} $$
For the negative energy states/antiparticles $v_{\eta}$, the equation becomes $m(\gamma^{0}+1)v_{\eta}=0$ so the solutions are
$$v_{\eta}^{(+)}(0)=\begin{bmatrix}
0 \\
0 \\
1 \\
0
\end{bmatrix},\;v_{\eta}^{(-)}(0)=\begin{bmatrix}
0 \\
0 \\
0 \\
1
\end{bmatrix}.\tag{2.5} $$
Consider $(p\!\!\!/-m)u_{\eta}=0$. Multiplying both sides by $p\!\!\!/+m$ gives$$(p\!\!\!/+m)(p\!\!\!/-m)u_{\eta}(\vec{p}\neq 0)=0\tag{2.6}. $$Expanding the brackets gives $p^2-m^2=0$ from the Klein-Gordon equation so $(2.6)$ is trivially satisfied. This shows that
$$u_{\eta}(\vec{p}\neq 0)=(p\!\!\!/+m)u_{\eta}(\vec{p}=0).\tag{2.7} $$
Forming $p\!\!\!/+m$ as a matrix and evaluating this gives
$$u^{(1)}(p)=\begin{bmatrix}
1 \\
0 \\
\frac{p_{z}}{E+m} \\
\frac{{p_{x}+ip_{y}}}{E+m}
\end{bmatrix},\;u^{(2)}(p)=\begin{bmatrix}
0 \\
1 \\
\frac{{p_{x}-ip_{y}}}{E+m} \\
-\frac{p_{z}}{E+{m}}
\end{bmatrix}.\tag{2.8} $$
This shows that some of the particle wavefunction goes to the antiparticle wavefunction.

Consider the product of these spinor,
$$\bar{u}^{(i)}(\vec{p})u^{(j)}(\vec{p})=u^{\dagger(i)}(\vec{p})\gamma^{0}u^{(j)}(\vec{p})=2m\delta_{ij}=-\bar{v}^{(i)}(\vec{p})v^{(j)}(\vec{p}).\tag{2.9} $$
The negative sign is there as $v,\bar{v}$ are negative energy solutions. $i,j=1,2=+,-$.
For the reverse,
$$\sum_{i=1}^{2}u^{(i)}_{\alpha}\bar{u}^{(j)}_{\beta}=(p\!\!\!/+m)_{\alpha\beta}\tag{2.10}. $$Similarly,
$$\sum_{i=1}^{2}v^{(i)}_{\alpha}\bar{v}^{(j)}_{\beta}=(p\!\!\!/-m)_{\alpha\beta}.\tag{2.11} $$
