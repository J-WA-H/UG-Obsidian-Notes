At a given time, structures can be non-linear while on other scales they can still be linear. The root mean square of density perturbations averaged over spheres of radius $R$ is $\sigma(R,t)$, this gives the typical $|\delta|$ in these regions is of size $\sim R$.

Linear theory is only reasonable for $\sigma(R,t)\lesssim 1$, which breaks down for $\sigma(R,t)\gtrsim 1$. For cold dark matter, $\sigma(R,t)$ decreases monotonically as $R$ increases.
[Recall](Random%20Density%20Fields.md):
- For $P(k)\propto k^{n}$ then $\sigma(R)\propto R^{-(n+3)/2}$
- For CDM, $n=1$ on large scales (inflation) and $n=-3$ on very small scales.

This shows that $\sigma(R,t)$ is approximately constant for small $R$ and $\propto R^{-2}$ for large scales. This implies smaller scales become non-linear first.

 In the present $z=0$ universe, $\sigma(R)\approx 1$ for $R=15\text{ Mpc}$, this corresponds to $M\sim 10^{15}M_{\odot}$, i.e. rich galaxy cluster.

Galaxies like the Milky way with $M\sim 10^{12}M_{\odot}$ typically become non-linear and collapsed as
![[Pasted image 20251207121234.png]]
Linear overdensity $\delta_{L}$ measured in spheres has a Gaussian distribution
$$P(\delta_{L})\propto \exp\left[ -\frac{\delta_{L}}{2\sigma^2} \right]\tag{26.1} .$$
A typical overdense spherical region of mass $M$ has $\delta_{L}\simeq \sigma(M,L)$ according to linear theory. According to the [[Spherical Collapse Model]] collapse model, the density perturbation collapses for $\delta_{L}=\delta_{L,coll}\simeq 1.7$. Hence objects of mass $M$ typically collapse when
$$\sigma(M,t)=\delta_{L,coll}\approx 1.7\tag{26.2} $$Recall for $\delta$ in dark matter at $a>a_{eq}$, 
$$\sigma(M,t)=\left( \frac{D_{+}(t)}{D_{+}(t_{0})} \right)\sigma(M,t_{0})\tag{26.3}. $$
As $\delta_{DM}$ grows as $D_{+}(a)$ independent of scale. The typical collapse time $t_{coll}$ for a dark matter halo of mass $M$ given by
$$\sigma(M,t_{coll})=\left( \frac{D_{+}(t_{coll})}{D_{+}(t_{0})} \right)\sigma(M,t_{0})=\delta_{L,coll}.\tag{26.4} $$
The two use cases are:
- Find typical collapse time of objects of mass $M$
- Find typical mass $M_{coll}$ of perturbations collapsing at time $t$

Recall $P(k)\propto k^{n},\sigma(M)\propto M^{-(n+3)/6}$ which gives
$$\sigma(M,t)=\left( \frac{M}{M_{0}} \right)^{-(n+3)/6}\tag{26.5} $$where $M_{0}$ is defined such that $\sigma(M_{0},t_{0})=1$. For $\Omega=\Omega_{m}=1$, then $D_+\propto t^{2/3}$,
$$\therefore \delta_{L,coll}=\left( \frac{D_{+}(t_{coll})}{D_{+}(t_{0})} \right)\sigma(M,t_{0})=\left( \frac{t_{coll}}{t_{0}} \right)\left( \frac{M}{M_{0}} \right)^{-(n+3)/6}\tag{26.6} .$$
Since $\delta_{L,coll}$ is constant, $t_{coll}\propto M^{(n+3)/4}$.

Provided $n>-3$, the typical collapse time $t_{coll}$ increases monotonically with increasing mass. Small objects form earlier and larger objects form later. This is the so-called hierarchical structure formation sequence. Hierarchical structure formation sequence is derived for $P(k)\propto k^{n}$ and $\Omega_{m}=1$. The same trend of collapse time vs mass applies whenever $\sigma(M)$ decreases monotonically with increasing $M$ since $D_{+}$ always increases monotonically with $t$.
![[Pasted image 20251207144053.png]]
The root mean square $\sigma(M)$ in a sphere of mass $M$ for the cold dark matter power spectrum at $z=0$, according to linear theory. Apart from special cases like spherical collapse, non-linear evolution of structure must be calculated using numerical simulations. Dark matter interacts only via gravity so we use N-body simulations. Baryons interact via gravity + gas pressure + heating + cooling + star formation + … so we use hydrodynamical simulations which are much more complicated. However, given that around 80% of matter is dark matter so N-body simulations can be used to calculate matter distributions on large scales.

For N-body simulations, we have to calculate gravitational forces due to all particles. From direct summation,
$$\ddot{\vec{r}}_{i}=G\sum_{i\neq j} \frac{m_{j}(\vec{r}_{j}-\vec{r}_{i})}{|\vec{r}_{j}-\vec{r}_{i}|^2}.\tag{26.7} $$
This is slow - $\mathcal{O}(N^2)$. There are other methods used to calculate this faster.

Grid methods: Calculate density field and gravitational force on the grid. This is fast, $\mathcal{O}(N\log N)$ per timestep, but the forces are inaccurate for small separations.

Tree methods: Group particles on different scales. This is again fast with $\mathcal{O}(N\log N)$, but the small scale forces are more accurate.

The general features are sheets, filaments, and halos.

For evolution from cold dark matter initial conditions, non-linear structures grow hierarchically-small halos form first, larger halos form later. Large halos form by the merging of smaller halos.

We measure large scale structures in the present day universe from galaxy-redshift surveys, where the distance is estimated from Hubble's law.
![[Pasted image 20251207165124.png]]
Galaxy distribution is expected to trace dark matter distribution on large scales. Use galaxy distributions as a tracer of matter density field. Compare the observed galaxy distribution with dark matter distribution predicted using N-body simulations:
1. Start with specification for the initial spectrum of density fluctuations at very early times, e.g. $P(k)=Ak^{n}$ with $n\approx 1$ for inflation.
2. Use linear perturbation theory to calculate how this spectrum evolves while $\delta\ll 2$ which depends on the nature of dark matter as well as other cosmological parameters.
3. Use N-body simulations to evolve matter distribution into non-linear regimes $\frac{\delta \rho}{\bar{\rho}}\gtrsim 1$, starting from initial conditions given by linear perturbation theory.
4. Compare statistical properties of density field measured in N-body simulations with measurements from galaxy surveys, using $P(k),\xi(r)$ (correlation function) and other measures of clustering.
 
We need to include additional processes for non-linear evolution of baryons:  
- shock heating: when gas streams collide at supersonic velocities, the gas gets heated in shock fronts – non-adiabatic process  
- gas cooling: hot gas can cool down by emitting radiation from atomic transitions star formation: gas which is cold and dense enough can undergo fragmentation and collapse due to its self gravity, forming stars  
- gas heating by stars: stars can heat the surrounding gas, e.g. by emitting ionizing radiation, or by exploding as supernovae  
- formation of black holes: gas in the central regions of galaxies can collapse to form supermassive black holes. Accretion disk around black holes emit energy during the accretion process.
- 