Consider Young's double slit experiment
![[Pasted image 20251031105936.png]]
Light travels from $\vec{r}_{j}$ to $\vec{r}$ in time $t_{j}=\frac{s_{j}}{c}$. We write the field at $\vec{r},t$ as a superposition of fields at earlier times. A polarised light source gives a scalar field,
$$E(\vec{r},t)=K_{1}E(\vec{r}_{1},t)+K_{2}E(\vec{r}_{2},t)\tag{10.1} $$
For a source of frequency bandwidth $\Delta \omega$, and path difference $\Delta s=|s_{1}-s_{2}|$, it is a necessary condition that
$$\Delta s\leq \frac{c}{\Delta \omega}\tag{10.2} .$$
The coherence length $\Delta s_{c}$ is the path difference beyond which coherence is lost. 

The coherence time
$$\Delta t_{c}=\frac{\Delta s_{c}}{c}\tag{10.3} $$defines where interference fringes, $\Delta t_{c}\Delta \omega \simeq 1$.

For a Lorentzian optical spectrum with $\Delta \omega$ the half-width half-maximum (HFHM), the coherence length and time are
$$\Delta s_{c}=\frac{c}{\Delta \omega},\;\Delta t_{c}=\frac{\Delta s_{c}}{c}=\frac{1}{\Delta \omega}.\tag{10.4} $$
Long detector response times mean we measure time-averaged light intensity $I(\vec{r})=\langle |E(\vec{r},t)|^2 \rangle$ where
$$\langle f(t) \rangle =\lim_{ T \to \infty } \frac{1}{T}\int_{0}^{T}dtf(t).\tag{10.5} $$
Assume the time average is stationary - independent of when we start averaging.

Defining
$$I_{1}=|K_{1}|^2\langle |E(\vec{r}_{1},t_{1})|^2 \rangle,\; I_{2}=|K_{2}|^2\langle |E(\vec{r}_{2},t_{2})|^2 \rangle \tag{10.6}  ,$$
we get
$$I(\vec{r})=I_{1}+I_{2}+2\mathrm{Re}[K_{1}^{*}K_{2}\langle E^{*}(\vec{r}_{1},t_{1})E(\vec{r}_{2},t_{2}) \rangle ].\tag{10.7} $$
It is seen that $I\propto E^2$.

Let $x_{j}$ collectively refer to $\vec{r}_{j}$ and $t_{j}$. The first order normalised classical coherence function is given by
$$\gamma^{(1)}(x_{1},x_{2})=\frac{{\langle E^{*}(x_{1})E(x_{2}) \rangle}}{\sqrt{ \langle |E(x_{1})|^2 \rangle \langle |E(x_{2})|^2 \rangle  }}\tag{10.8}. $$
The intensity at the screen in terms of the coherence function is
$$I(\vec{r})=I_{1}+I_{2}+2\sqrt{ I_{1}I_{2} }|\gamma^{(1)}(x_{1},x_{2})|\cos(\phi_{12}-\phi_{1}+\phi_{2})\tag{10.9} $$
where $\phi_{1},\phi_{2},\phi_{12}$ are the phases of the complex quantities $K_{1},K_{2},\gamma^{(1)}(x_{1},x_{2})$ respectively.

Interference occurs when $|\gamma^{(1)}(x_{1},x_{2})|>0$.
$|\gamma^{(1)}(x_{1},x_{2})|=1$ is complete coherence
$|\gamma^{(1)}(x_{1},x_{2})|=0$ is complete incoherence
$0<|\gamma^{(1)}(x_{1},x_{2})|<1$ is partial coherence.

For complete coherence, $|\langle E^{*}(x_{1},x_{2})E(x_{1},x_{2}) \rangle|=\sqrt{ \langle |E(x_{1})|^2 \rangle }\sqrt{ \langle |E(x_{2})| \rangle }.$

Consider $E(z,t)=E_{0}e^{ i(kz-\omega t) }$, which implies
$$\langle E^{*}(z,t)E(z,t+\tau) \rangle=\langle E^{*}(t)E(t+\tau) \rangle = |E_{0}|^2e^{ -i\omega \tau }\tag{10.10} $$
$$\langle |E(t)|^2 \rangle =|E_{0}|^2=\langle |E(t+\tau)|^2 \rangle .\tag{10.11} $$
Hence $|\gamma^{(1)}(\tau)|=1$ which gives complete coherence.

Consider $E(z,t)=E_{0}e^{ i(kz-\omega t) }e^{ i\phi(t) }$ where $\phi(t)$ changes randomly every $t=n\tau_{0}$. 
For $\tau>\tau_{0}$, the autocorrelation function has decayed to zero
For $\tau<\tau_{0}$,
$$\gamma^{(1)}(\tau)=\left( 1-\frac{\tau}{\tau_{0}} \right)e^{ -i\omega t }.\tag{10.12} $$
