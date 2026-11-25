The most useful measure of the horizon size for studying the evolution of density perturbations is the Hubble radius, 
$$R_{H}(t)\equiv \frac{c}{H(t)}.\tag{18.1} $$This is the proper length scale with Hubble expansion velocity $v=Hr=c$. Since for $r>R_{H}\implies v>c$, Newtonian mechanics is not needed so general relativity is needed.
Physically, $R_H$ is the maximum physical distance over which causal processes operate over one expansion time.
$$t_{exp}=\frac{a}{\dot{a}}=\frac{1}{H}.\tag{18.2} $$
Effects propagate at speed $\leq c$ so the maximum distance is $\leq ct_{exp}=\frac{c}{H}$. 

Define horizon mass,
$$M_{H}=\frac{4\pi}{3}\bar{\rho}_{m} \left( \frac{R_{H}}{2} \right)^3\tag{18.3} $$where $M_H$ is defined by the matter density so it is the mass of matter within the horizon. 
$R_H$ evolves as
$$R_{H}(t)\propto \frac{1}{H(t)}\propto \begin{cases}
\frac{1}{const}=const & \text{inflation} \\
\frac{1}{1/t}\propto t\propto a^2 & \text{radiation} \\
\frac{1}{1/t}\propto t\propto a^{3/2} & \text{Matter}
\end{cases}.\tag{18.4} $$
The proper wavelength of density perturbations [evolves as](Jean's Length) 
$$\lambda=\lambda_{com}a\propto a\tag{18.5} .$$During inflation, $\delta$ starts with $\lambda<R_{H}$ inside the horizon and evolves to $\lambda>R_{H}$ outside the horizon.

Perturbations leave the horizon at $\lambda(t)=R_{H}(t)$ with $\frac{\lambda}{R_{H}}$ increasing with time. During radiation and matter domination eras, $\delta$ starts with $\lambda>R_{H}$ and evolves to $\lambda<R_{H}$ as $\lambda(t)$ grows smaller than $R_H(t)$. Perturbations re-enter the horizon at $\lambda(t)=R_{H}(t)$ where $\frac{\lambda}{R_{H}}$ is decreasing with time.

Density perturbations are generated inside the horizon during inflation. Then they spend some time outside the horizon between $t_{exit}<t<t_{enter}$, and then they come back into the horizon at time $t_{enter}$.
![[Pasted image 20251114102536.png]]
$\delta \rho$ with a larger $\lambda_{com}$ exits the horizon earlier and re-enter later.

The Hubble radius can be determined from the Friedmann equation for a flat universe,
$$H^2(a)=\frac{8\pi G}{3}\bar{\rho}\approx \begin{cases}
\frac{8\pi G}{3} \bar{\rho}_{r_{0}}a^{-4} & a_{inf}<a<a_{eq} \\
\frac{8\pi G}{3} \bar{\rho}_{m_{9}}a^{-3} & a_{eq}<a<a_{DE}
\end{cases}.\tag{18.6} $$
The perturbation enters the horizon at $a_{enter}$ given by
$$R_{H}(a_{enter})\equiv\lambda \implies \ell_{H}(a_{enter})=\lambda_{com}\tag{18.7} $$with the comoving horizon size 
$$\ell_{H}\equiv \frac{R_{H}}{a}=\frac{c}{aH(a)}\approx \begin{cases}
\ell_{H_{eq}} \left( \frac{a}{a_{eq}} \right) & a_{inf}<a<a_{eq} \\
\ell_{H_{eq}} \left( \frac{a}{a_{eq}} \right)^{1/2} & a_{eq}<a<a_{DE}
\end{cases}\tag{18.8} $$
with $\ell_{H_{eq}}=\frac{R_{H}(a_{eq})}{a_{eq}}$.
This gives
$$a_{enter}(\lambda_{com})\propto \begin{cases}
\lambda_{com} & a_{enter}<a_{eq} & \lambda_{com}<\ell_{H_{eq}} \\
\lambda_{com}^2 & a_{enter}>a_{eq} & \lambda_{com}>\ell_{H_{eq}}
\end{cases}.\tag{18.9} $$
Density perturbations entering the horizon at $a=a_{eq}$ has $\lambda_{com}=\ell_{H_{eq}}$. The characteristic length scale $\ell_{H_{eq}}$ is the comoving horizon size at matter-radiation equality so 
$$\ell_{H_{eq}}=\frac{c}{H_{eq}a_{eq}}\approx\left( \frac{3\bar{\rho}_{r_{0}}}{8\pi G} \right)^{1/2}\left( \frac{c}{\bar{\rho}_{m_{0}}} \right)=130\text{ Mpc}.\tag{18.10} $$
The corresponding mass scale in the present universe is
$$M_{H_{eq}}=\frac{4\pi}{3}\bar{\rho}_{m_{0}}\left( \frac{\ell_{H_{eq}}}{2} \right)^{3}=4.9\times 10^{16}M_{\odot}.\tag{18.11} $$
Gravitationally bound structures in the present day universe have $M\lesssim 10^{15}M_{\odot}$.  The corresponding density perturbations have $a_{enter}<a_{eq}$,

From the proper Jean's length,
$$\lambda_{J}=\sqrt{ \frac{8}{3} }\pi\left( \frac{c_{s}}{c} \right)R_{H}\tag{18.12} .$$For a [[Baryon-Photon Fluid]], $c_{s}\approx \frac{c}{\sqrt{ 3 }}$ so $\lambda_{J}\sim R_{H}$. More generally, $c_{s}\leq c$  for any fluid so $\lambda_{J}\lesssim R_{H}$. Hence, perturbations with $\lambda\gg R_{H}$ have $\lambda\gg\lambda_{J}$ and pressure forces have a negligible effect of density perturbations well outside the horizon.

Recall the [Free-streaming](Free%20Streaming%20of%20Dark%20Matter.md) length $(17.5-6)$
$$\lambda_{FS}(t)=a(t)\int_{0}^{t} \frac{v_{*}(t')dt'}{a(t')}. $$A typical particle has thermal velocity $v_{*}\leq c$ so that
$$\lambda_{FS}\leq a(t)\int_{0}^{t} \frac{cdt'}{a(t')}\tag{18.13} $$
with $a(t)\propto t^{1/2}$ or $t^{2/3}$ and $R_{H}=\frac{c}{H}\propto \frac{1}{t}$ in the radiation and matter dominated eras,
$$\frac{\lambda_{FS}(t)}{R_{H}(t)}\leq \begin{cases}
1 & \text{radiation} \\
2 & \text{matter}
\end{cases}\tag{18.14} $$
so $\lambda_{FS}\lesssim R_{H}$. When dark matter particles are still relativistic, $v_{*}\approx c\implies\lambda_{FS}\sim R_{H}$.

Perturbations with $\lambda\gg R_{H}$ have $\lambda\gg\lambda_{FS}$ so free streaming has one negligible effect on perturbation growth outside the horizon.

- For $\lambda>R_{H}$, Newtonian mechanics is not valid so we need general relativity
- For $\lambda\gg R_{H}$ neither pressure nor free streaming is important so evolution is controlled only by gravity. The evolution is the same for a uniform density spherical perturbations
![[Pasted image 20251114124803.png]]

The evolution of density perturbations $\delta \rho$ with $\lambda>R_{H}$ are the same as the results derived from Newtonian mechanics for $\lambda\ll R_{H}$ and $\lambda\gg\lambda_{J},\lambda_{FS}$. Hence the growing mode solution for density perturbations outside the horizon is
$$D_{+}\propto \begin{cases}
a^2\propto t & \text{radiation} \\
a\propto t^{2/3} & \text{matter}
\end{cases}.\tag{18.15} $$
