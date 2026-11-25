Global strings have a Goldstone boson field extending beyond the core, giving a non-zero energy-momentum tensor throughout space.

Consider a global $U(1)$-string described by the scalar field ansatz
$$\phi=f(r)e^{ i\theta },\tag{21.1} $$
with $f(0)=0$ and $f(r)\approx \eta$ for $r\gg\delta$, where $\delta$ is the thickness of the string core. The global string spacetime has the same symmetries as that of a gauge string, and the metric can still be written in the form
$$ds^2=e^{ A(r) }(dt^2-dz^2)-dr^2-e^{ B(r) }d\theta^2.\tag{21.2} $$
Outside the core, the energy-momentum tensor is given by
$$T^{0}_{\;0}=T^{z}_{\;z}=T^{r}_{\;r}=-T^{\theta}_{\;\theta}=\eta^2e^{ -B(r) },\tag{21.3} $$
where the functions $A(r),B(r)$ obey the Einstein equations
$$\begin{matrix}
A''+A'^2+\frac{1}{2}A'B'=16\pi G\left( T^t_{\;t}-\frac{1}{2}T \right), \\
B''+\frac{1}{2}B'^2+A'B'=16\pi G\left( T^\theta_{\;\theta}-\frac{1}{2}T \right), \\
2A''+B''+A'^2+\frac{1}{2}B'^2=16\pi G\left( T^r_{\;r}-\frac{1}{2}T \right),
\end{matrix}\tag{21.4} $$where $T=T^\nu_{\;\nu}$.

Studying the [linearised Einstein equations](Linearised%20Gravity) with $T^\nu_{\;\mu}$ in $(21.3)$ gives the solution,
$$ds^2=[1-4G\mu(r)](dt^2-dz^2)-dr^2-[1-8G\mu(r)]r^2\theta^2,\tag{21.5} $$where $\mu(r)$ is the string mass per unit length out to a distance scale $r$ from the core,
$$\mu(r)\simeq \int_{\delta}^{r}T^0_{\;0}2\pi rdr\simeq{2}\pi \eta ^2\ln\left( \frac{r}{\delta} \right).\tag{21.6} $$
Note two qualitative differences between the metrics of global and gauge strings: (i) the effective deficit angle for a global string
$$\Delta(r)=8\pi G\mu(r),\tag{21.7} $$increases logarithmically with distance from the core, while the gauge string deficit angle remains constant; and (ii) a global string has a repulsive gravitational potential. A non-relativistic test particle at a distance $r$ from the string experiences a gravitational acceleration away from the string,
$$\ddot{r}=\frac{4\pi G\eta}{r}\tag{21.8}. $$The linear approximation to the Einstein equations breaks down at $G\mu(r)\gtrsim 1$. The metric must develop a singularity at a finite distance from the string axis. A solution of the Einstein equations $(21.4)$ with $T^\nu_{\;\mu}$ from $(21.3)$ gives
$$ds^2=\left( \frac{u}{u_{0}} \right)(dt^2-dz^2)-r_{0}^2\left( \frac{u_{0}}{u} \right)^{1/2}e^{ (u_{0}-u^2/u_{0}) }(du^2+d\theta^2),\tag{21.9} $$
where $u_{0}=\frac{1}{8\pi G\eta^2}$ and $r_{0}$ is an integration constant. The only approximation made in deriving this was to set $f(r)\approx \eta$ so that $T^\nu_{\;\mu}$ has the form in $(21.3)$.
For $\eta\ll m_{pl}$, $u_{0}$ is a large parameter. To leading order in $\frac{1}{u_{0}}$, the relation between the coordinate $u$ and the radial coordinate $r$ in the linearised metric $(21.5)$ is 
$$u\approx u_{0}-\ln\left( \frac{r}{r_{0}} \right)\tag{21.10} .$$
The two metrics agree if we set $r_{0}\sim \delta$. Hence, $u\sim u_{0}$ corresponds to the vicinity of the string core. The values of $u\gtrsim u_{0}$ are in the core interior $r\lesssim\delta$, where the approximation for $f(r)$ is violated, and the metric $(21.9)$ is no longer valid.
Large values of $r$ correspond to small values of $u$. When $\frac{r}{r_{0}}$ becomes comparable to $\exp(u_{0})$, the linearised metric can no longer be used. The exact solution $(21.9)$ is singular at $u=0$, and it can be verified that this is a true geometric singularity. In the vicinity of $u=0$, the metric can be transformed to 
$$ds^2=\xi^{4/3}(dt^2-dz^2)-d\xi^2-\xi^{-2/3}d\theta^2,\tag{21.11} $$
with $\xi \propto u^{3/4}$. In the nonlinear regime, the deficit angle ceases to grow with $r$. Instead, it starts decreasing and turns into an excess angle which blows up at the singularity.

From $(21.11)$, the singularity occurs at a finite proper distance from the string core. This distance is of order $r_{max}\sim \delta \exp(u_{0})$ which can be very large for $\eta\ll m_{pl}$. In particular, curvature singularities are of little concern for global strings with $\eta<2\times 10^{17}\text{ GeV}$ in a cosmological context, since $r_{max}$ would be greater than the present horizon.