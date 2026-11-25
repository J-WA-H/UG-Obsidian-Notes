In a flat spacetime with $g_{\mu \nu}=n_{\mu \nu}=\mathrm{diag}(+1,-1,-1,-1)$ and $\Gamma^{\mu}_{\nu\sigma}=0$, the string equations of motion [(15.9)](Actions.md) take the form
$$\partial_{a}\left(\sqrt{ -\gamma }\gamma^{ab}x^{\mu}_{,b}\right)=0\tag{16.1}. $$
Since the Nambu action is invariant under coordinate transformations, we are free to choose any parametrisation of the worldsheet. This can be done explicitly, for example, as in the light-cone gauge,
$$\zeta^{0}=t,\;\zeta^{1}=z-t,\tag{16.2} $$
or else by imposing two gauge conditions. A very convenient choice of gauge for a string in flat spacetime is
$$\begin{matrix}
\gamma_{01}=0, & \gamma_{00}+\gamma_{11}=0.\tag{16.3} 
\end{matrix}$$
Using the definition of $\gamma_{ab}$, this can be rewritten as
$$\begin{matrix}
\dot{x}\cdot x'=0, \\
\dot{x}^2+x'^2=0,\tag{16.4} 
\end{matrix}$$
where the dots and primes stand for derivatives with respect to $\zeta^{0}$ and $\zeta^{1}$, respectively. This is known as the conformal gauge because the worldsheet metric takes a conformally flat form
$$\begin{matrix}
\gamma_{ab}=\sqrt{ -\gamma }\eta_{ab}, & \gamma^{ab}=\frac{1}{\sqrt{ -\gamma }}\eta^{ab}.\tag{16.5} 
\end{matrix}$$
$(16.1)$ then becomes the two dimensional wave equation
$$\ddot{x}^{\mu}-x''^{\mu}=0.\tag{16.6} $$
The gauge conditions $(16.4)$ do not fix the gauge completely. There is still the freedom to perform transformations such that $\dot{\zeta}^{1}=\zeta'^{0}$ and $\zeta'^{1}=\dot{\zeta}^{0}$, implying that
$$\ddot{\zeta}^{a}-\zeta''^{a}=0.\tag{16.7} $$
We can remove this residual freedom by setting
$$t\equiv x^{0}=\zeta^{0},\tag{16.8} $$
which is consistent with $(16.6)$. This allows us to write the string trajectory as the three vector $\vec{x}=(\zeta,t)$ where $\zeta=\zeta^{1}$ is the spacelike parameter on the string and the constraints take the form of the transverse gauge,
$$\begin{matrix}
\dot{\vec{x}}\cdot \vec{x}'=0, \\
\dot{\vec{x}}^2+\vec{x}^{2}=1, \\
\ddot{\vec{x}}-\vec{x}''=0.\tag{16.9} 
\end{matrix}$$
The first of these equations implies that the vector $\dot{\vec{x}}$ is perpendicular to the string and thus represents the physically observable velocity. This is called the transverse gauge. The second equation can be written as $d\zeta=(1-\dot{x}^2)^{-1/2}|d\vec{x}|=d\mathcal{E}/\mu$ where
$$\mathcal{E}=\mu \int(1-\dot{\vec{x}})^{-1/2}dl=\mu \int d\zeta \tag{16.10} $$is the energy of the string and $dl=|d\vec{x}|$. This we have chosen $\zeta$ to be proportional to the string energy measured from some arbitrary point on the string. Finally, the third equation implies that the acceleration of a string element in its local rest frame $(\dot{\vec{x}}=0)$ is inversely proportional to the local curvature radius, $R^{-1}=|d^2\vec{x}/dl^2|$. The direction of $\ddot{\vec{x}}$ is such that a curved string tends to straighten. In doing so, it develops a velocity and begins to oscillate. As the third equation is a wave equation, it has the general solution
$$\vec{x}(\zeta,t)=\frac{1}{2}[\vec{a}(\zeta-t)+\vec{b}(\zeta-t)],\tag{16.11} $$with the other two equations giving the constraint $\vec{a}'^2=\vec{b}'^2=1$.
The geometric interpretation of these constraints is that $\zeta$ is the length parameter along the three-dimensional curves $\vec{a}(\zeta)$ and $\vec{b}(\zeta)$. The string energy-momentum tensor in this gauge is then
$$T^{\mu \nu}(\vec{x},t)=\mu \int d\zeta(\dot{x}^{\mu}\dot{x}^{\nu}-x'^{\mu}x'^{\nu})\delta^{(3)}(\vec{x}-\vec{x}(\zeta,t)).\tag{16.12} $$
The total energy of the string is given by
$$\mathcal{E}=\int T^{0}_{\;0}d^3x=\mu \int d\zeta,\tag{16.13} $$which agrees with $(16.10)$. The string momentum and angular momentum are$$\vec{P}=\mu \int d\zeta \;\dot{\vec{x}}(\zeta,t),\tag{16.14}$$$$
\vec{J}=\mu \int d\zeta\;\vec{x}(\zeta,t)\times \dot{x}(\zeta,t).\tag{16.15} $$
The motion of a closed loop of string is described by $(16.11)$ with $0\leq\zeta<L$ where $L=\mathcal{E}/\mu$ is the invariant length of the loop. For a closed loop we need periodicity $\vec{x}(\zeta+L,t)=\vec{x}(\zeta,t)$ or equivalently
$$\vec{b}(\zeta_{+}+L)-\vec{b}(\zeta_{+})=-\vec{a}(\zeta_{-}+L)+\vec{a}(\zeta_{-})\equiv \vec{\Delta}\tag{16.16} $$
with $\zeta_{\pm}=\zeta\pm t$. The vector $\vec{\Delta}$ must be a constant vector independent of $\zeta_{\pm}$ and is directly proportional to the momentum of the loop
$$\vec{P}=\frac{\mu}{2}\int_{0}^{L}d\zeta\;(\vec{b}'-\vec{a}')=\mu\vec{\Delta}.\tag{16.17} $$
In the centre of mass frame of the loop, $\vec{\Delta}=\vec{0}$ and $\vec{a}$ and $\vec{b}$ are periodic functions with period $L$. The motion of the loop must also be periodic in time, $T=L/2$ since
$$\vec{x}\left( \zeta+\frac{L}{2},t+\frac{L}{2} \right)=\vec{x}(\zeta,t).\tag{16.18} $$
The fact that the timescale of the oscillation is comparable to the loop length $L$ indicates that the motion of the loop is relativistic. We can define the mean square string velocity of segments on the loop as
$$v_{av}=\left\langle v^2 \right\rangle^{1/2} \tag{16.19}, $$where $$\left\langle  v^2  \right\rangle=\int_{0}^{T} \frac{dt}{T}\int_{0}^{L} \frac{d\zeta}{L}\dot{\vec{x}}^2. \tag{16.20} $$Integrating by parts we can write
$$\int_{\Sigma}d^2\zeta\; \dot{\vec{x}}^2=\int d^2\zeta\;\vec{x}\cdot \ddot{\vec{x}}=\int d^2\zeta\;\vec{x}\cdot \vec{x}''=\int d^2\zeta\;\dot{\vec{x}}'^2=\int d^2\zeta(1-\dot{\vec{x}}^2),\tag{16.21} $$
where the limits of integration on $\Sigma$ are over one period so $\langle v^2\rangle=0.5$.
