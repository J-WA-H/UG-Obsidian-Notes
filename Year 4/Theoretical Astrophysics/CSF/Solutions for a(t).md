Define the critical density - density for a flat universe
$$\rho_{crit}(t)\equiv \frac{{3}H^2(t)}{8\pi G}.\tag{4.1} $$
This defines the [density parameter](Contents%20of%20the%20Universe.md),
$$\Omega(t)=\frac{\rho(t)}{\rho_{crit}(t)}.\tag{1.1} $$
Substituting this into the [Friedmann equation](Cosmological%20Expansion.md) gives
$$\Omega(t)-1=\frac{kc^3}{H^2(t)a^2(t)}.\tag{4.2} $$
If the universe is spatially flat, $k=0\iff \Omega(t)=1\iff \rho(t)=\rho_{crit}(t)$. More generally,
$$k=\frac{(\Omega_{0}-1)H_{0}^2}{c^2}\tag{4.3} $$where $\Omega_{0}=\Omega(t_{0})$. Current observations give $\Omega_{0}\approx 1$ and $k\approx 0$.

In general, the total density is
$$\rho(t)=\rho_{m}(t)+\rho_{r}(t)+\rho_{v}\tag{4.4}, $$
so
$$\Omega(t)=\Omega_{m}(t)+\Omega_{r}(t)+\Omega_{v}(t).\tag{4.5} $$
Today, $\rho_{crit_{0}}=9.16\times 10^{-27}\text{ kg m}^{-3}$. 

Photons from the CMB show a blackbody with present $T_{\gamma_{0}}=2.73\text{ K}$ and $\Omega_{\gamma_{0}}=5.06\times 10^{-5}$.

Neutrinos, assume three massless types, gives $\rho_{\nu_{0}}=3\times \frac{7}{8} \times \left( \frac{4}{11} \right)^{4/3}\rho_{\gamma_{0}}$ and $\Omega_{\nu_{0}}=3.45\times 10^{-5}$.

Total radiation includes all relativistic particles
$$\Omega_{r_{0}}=\Omega_{\gamma_{0}}+\Omega_{\nu_{0}}=8.51\times 10^{-5}.\tag{4.6} $$
The most accurate estimate of baryons is from the CMB temperature fluctuations, $\Omega_{b_{0}}=0.044-0.049$. We will use the round number $\Omega_{b_{0}}=0.05$.
Assuming cold dark matter, the most accurate estimate is from the CMB, $\Omega_{DM_{0}}=0.21-0.26$ so use the round number $\Omega_{DM_{0}}=0.25$.
The total matter includes all relativistic particles,
$$\Omega_{m_{0}}=\Omega_{b_{0}}+\Omega_{DM_{0}}=0.30\tag{4.7} .$$
The total density and curvature measurements also come from the CMB which gives $1-\Omega_{0}=0.00-0.01$ so we will use $\Omega_{0}=1$.

Dark energy comes from CMB and supernova data which gives $w=-1.1\pm{0}.1$ so assume $w=-1$ so $\rho_{v}\approx\text{const}$.
Assuming $\Omega_{0}=1$,
$$\Omega_{v_{0}}=1-\Omega_{m_{0}}=0.7.\tag{4.8} $$
This gives the Friedmann equation
$$H^2\equiv\left( \frac{\dot{a}}{a} \right)^2=\frac{8\pi G}{3}(\rho_{m_{0}}a^{-3}+\rho_{r_{0}}a^{-4}+\rho_{v_{0}})-\frac{kc^2}{a^2}.\tag{4.9} $$
Since $H=\frac{\dot{a}}{a}$, $\frac{da}{dt}=aH\implies dt=\frac{da}{aH}$ so the Friedmann equation can be solved by
$$t(a)=\int_{0}^{a} \frac{da}{aH(a)}\tag{4.10} $$
with $t=0$ when $a=0$. Assuming $k=0$,
![[Pasted image 20251017111513.png]]
For radiation domination, $\rho \approx \rho_{r}$ and $a<a_{eq}\equiv \frac{\rho_{r_{0}}}{\rho_{m_{0}}}$ where $a_{eq}$ is the epoch of matter-radiation equality. The redshift is given by
$$1+z_{eq}\equiv \frac{1}{a_{eq}}=\frac{\Omega_{m_{0}}}{\Omega_{r_{0}}}=3.53\times 10^{3}.\tag{4.11} $$
For $a\ll a_{eq}$, $H^2(a)=\frac{8\pi G}{3} \rho_{r_{0}}a^{-4}$. Solving this gives $a(t)\propto t^{1/2}$,
$$H=\frac{1}{2t},\;\rho=\frac{3}{32\pi Gt^2}\tag{4.12} .$$
For matter domination, $\rho \approx \rho_{m}$ so
$$a_{eq}<a<a_{DE}\equiv\left( \frac{\rho_{m_{0}}}{\rho_{v_{0}}} \right)^{1/3}\tag{4.13} $$where $a_{DE}$ is the epoch of dark energy-matter equality.
$$1+z_{DE}\equiv \frac{1}{a_{DE}}=\left( \frac{\Omega_{v_{0}}}{\Omega_{m_{0}}} \right)^{1/3}=1.33.\tag{4.14} $$
For $a_{eq}\ll a\ll a_{DE}$, $H^2(a)=\frac{8\pi G}{3}\rho_{m_{0}}a^{-3}$ so $a(t)\propto t^{-2/3}$,
$$H=\frac{2}{3t},\;\rho=\frac{1}{g\pi Gt^2}.\tag{4.15} $$
Vacuum domination is at $a>a_{DE}$ where $\rho \approx \rho_{v}$,
$$H^2(a)=\frac{8\pi G}{3}\rho_{v_{0}}=H_{v}^2=\text{const}.\tag{4.16} $$so $a(t)\propto e^{ H_{v}t }$.

Inflation occurs at very early times, before radiation domination, $p\approx-\rho c^2\approx-V(\phi)$, where the scalar field $\phi$ slowly varying so
$$H^2(a)=\frac{8\pi G}{3} \frac{V(\phi)}{c^2}\equiv H_{\phi}=\text{const}\tag{4.17} $$
so
$$a(t)\approx e^{ H_{\phi}t }.\tag{4.18} $$
![[Pasted image 20251017112929.png]]
