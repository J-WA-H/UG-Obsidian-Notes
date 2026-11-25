Consider the two main pictures of quantum mechanics. The Heisenberg picture has the time evolution in the operator $\hat{O}=\hat{O}(t)$ while the Schrodinger picture has the time evolution in the wavefunction $\ket{\psi(t)}$.
You can move between the 2 pictures using the evolution operator,
$$\hat{U}(t,t_{0})=\exp\left[-i\int_{t_{0}}^{t}dt\hat{H}\right]\tag{8.1} .$$
There is also an interaction picture where the evolution operator follows the equation
$$i\frac{d}{dt} \hat{U}_{I}(t,t_{0})=\hat{H}_{int}(t)\hat{U}_{I}(t,t_{0})\tag{8.2} $$where$$\hat{H}_{int}(t)=e^{ i\hat{H}_{0}t }\hat{H}_{int}e^{ -i\hat{H}_{0}t }.\tag{8.3} $$
Solving this gives an integral equation,
$$\hat{U}_{I}(t)=1-i \int_{-\infty}^{\infty}dt_{1}\hat{H}_{int}(t_{1})\hat{U}_{I}(t_{1})\tag{8.4} .$$
This can be approximated by substituting $\hat{U}_{I}$ into the integral,
$$\hat{U}_{I}(t)=1-i\int_{-\infty}^{\infty}dt_{1} \hat{H}_{int}(t_{1})\left(1-i\int_{-\infty}^{\infty} dt_{2} \hat{H}_{int}(t_{2})\hat{U}_{I}(t_{2})\right)\tag{8.5} .$$
In general, the nth term approximation gives
$$\hat{U}_{I}(t)\approx (1-i)^{n}\int_{-\infty}^{t}dt_{1}\int_{-\infty}^{t_{1}}dt_{2}\dots \int_{-\infty}^{t_{n-1}}dt_{n}\hat{H}_{int}(t_{1})\hat{H}_{int}(t_{2})\dots \hat{H}_{int}(t_{n})\cancelto{1}{\hat{U}_{I}(t_{n})}.\tag{8.6} $$
If the Hamiltonians don't commute, the ordering matters so use [time ordering](Feynman%20Propagator.md) which gives$$\hat{U}_{I}(t_,t_{0})=T\left(\exp\left[-i \int_{-\infty}^{t} dt'\hat{H}_{int}(t') \right]\right).\tag{8.7} $$This is the Dyson formular, which expanding out gives the Dyson formula, e.g.
![[Pasted image 20251028194521.png]]
$\hat{U}_{I}(t)$ can be used to transform between the Heisenberg and interaction pictures,
$$\hat{\phi}_{I}(\vec{x},t)=\hat{U}_{I}(t)\hat{\phi}_{H}(\vec{x},t)\hat{U}_{I}^{\dagger}(t).\tag{8.8} $$
$\hat{U}_{I}$ can also give the [S-matrix](Interacting%20Fields.md),
$$\hat{U}_{I}(t\to \infty)=\hat{S}\tag{8.9}. $$
This gives
$$\hat{S}=T\left[ \exp\left( -i \int_{-\infty}^{\infty} \hat{H}_{int} (t')dt' \right) \right].\tag{8.10} $$
The matrix element is also 
$$S_{fi}=\braket{ k_{1},\dots,k_{n};out | p_{1},p_{2};in } = \bra{k_{1},\dots ,k_{n};out} \hat{a}^{\dagger}_{in}(p_{1})\ket{p_{2};in} .\tag{8.11} $$
Substitute in the expression for $\hat{a}^{\dagger}$ in terms of $\hat{\phi}$, [(4.12)](Quantisation%20of%20Fields.md),
$$S_{fi}=i\int d^4x_{1}e^{ -ip_{1}^{\mu}x_{1\mu} }(\square_{x_{1}}+m^2)\bra{k_{1},\dots,k_{n};out}\hat{\phi}_{H}(x_{1})\ket{p_{2};in} \tag{8.12}  .$$
This is the prototype of the LSZ formula, which is obtained by eliminating the momentum Fock states,$$S_{fi}=(i)^{n+2}\int d^4x_{1}\int d^4x_{2}\int d^4y_{1}\dots \int d^4y_{n}e^{ (-ip_{1}^\mu x_{1\mu} -ip_{2}^{\mu}x_{1\mu}+ik_{1}^{\mu}y_{1\mu}+\dots+ik_{n}^{\mu}y_{n\mu})}(\square_{x_{1}}+m^2)(\square_{x_{2}}+m^2)(\square_{y_{1}}+m^2)\dots(\square_{y_{n}}+m^2)\bra{0;out} $$$$T(\hat{\phi}_{H}(y_{1})\dots \hat{\phi}_{H}(y_{n})\hat{\phi}_{H}(x_{1})\hat{\phi}_{H}(x_{2}))\ket{0;in} .\tag{8.13} $$
The [[Feynman Propagator]] is defined by operators in the Heisenberg picture, while it can be useful to express it in operators in the interaction picture,
$$G_{n}=\bra{0} T(\hat{U}^{\dagger}(t_{1})\hat{\phi}_{I}(x_{1})\hat{U}_{I}(x_{1})\hat{U}^{\dagger}_{I}(t_{2})\hat{\phi}_{I}(x_{2})\hat{U}_{I}(t_{2})\dots \hat{U}_{I}^{\dagger}(t_{n})\hat{\phi}_{I}(x_{n})\hat{U}_{I}(t_{n}))\ket{0}.\tag{8.14}  $$
Note that
$$\hat{U}_{I}(t_{1})\hat{U}^{\dagger}_{I}(t_{2})\equiv \hat{U}_{I}(t_{1},t_{2}).\tag{8.15} $$
This means $G_{n}$ can be further rewritten is
$$G_{n}=\bra{0} \hat{U}_{I}^{\dagger}(t_{1})T(\hat{\phi}_{I}(t_{1})\dots\hat{\phi}_{I}(t_{n})\hat{U}_{I}(t_{1},t_{n})) \ket{0}.\tag{8.16}  $$Sending $t_{1}\to \infty$, $t_{n}\to -\infty$ gives $\hat{U}_{I}(t_{1},t_{n})\to \hat{S}$.

We have a time ordered Greens function where the braket is $G_{n+1}(y_{1},y_{2},x_{1},\dots,x_{n})$,
$$G_{n}(x_{1},\dots,x_{n})\equiv \bra{0} T(\hat{\phi}(x_{1}),\dots,\hat{\phi}(x_{n}))\ket{0} = \frac{{\bra{0} T(\hat{\phi}_{I}(x_{1}),\dots,\hat{\phi}_{I}(x_{n}))\hat{S}\ket{0} }}{\bra{0} \hat{S}\ket{0} }.\tag{8.14} $$
