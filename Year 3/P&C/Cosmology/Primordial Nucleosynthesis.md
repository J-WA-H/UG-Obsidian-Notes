Primordial/big bang nucleosynthesis (BBN) describes how light elements formed in the early universe.
Some observations are that light elements distribute more homogeneously than they would be if produced by stars.
Deuterium is destroyed rather than created in stars, but it is observed cosmologically so it must be produced by some other process.
The observed abundance of $^4\text{He}$ is larger than what can be synthesised in stars.

There are 3 main stages in BBN:
Stage 1: ($k_{B}T>0.7\text{ MeV}$)
This involves weak interactions:
$$n\leftrightarrow p+e^{-}+\bar{\nu}_{e}$$
$$e^{+}+n\leftrightarrow p+\bar{\nu}_{e}$$
$$\nu_{e}+n\leftrightarrow p+e^{-}.$$
This stage is from equilibrium to freeze-out.
These interactions show there is frequent conversions between neutrons and protons.
The fraction between the number of protons and neutrons is
$$\frac{N_{n}}{N_{p}}=\exp\left[ -\frac{\Delta mc^2}{k_{B}T} \right].$$
This relation holds until freeze-out where $k_{B}T=0.7\text{ MeV}$.

[Recall](Cosmic%20Microwave%20Background.md) for fermions
$$n(\nu,T)d\nu=\frac{8\pi \nu^2}{c^3} \frac{d\nu}{\exp\left[ \frac{h\nu}{k_{B}T} \right]}+1$$
and the relativistic energy is
$$E^2=p^2c^2+m^2c^4>mc^2\gg k_{B}T.$$
$$\therefore n(E,T)dE\propto E^2e^{-E/k_{B}T}dE.$$
$$N(T)\propto \exp\left[ -\frac{mc^2}{k_{B}T} \right].$$
For neutrons
$$N_{n}(T)\propto \exp\left[ -\frac{m_{n}c^2}{k_{B}T} \right]$$
$$N_{p}(T)\propto \exp\left[ -\frac{m_{p}c^2}{k_{B}T} \right].$$
$$\therefore \frac{N_{n}}{N_{p}}=\exp\left[ -\frac{\Delta mc^2}{k_{B}T} \right]$$
where $\Delta m=m_{n}-m_{p}\approx 1.3\text{ MeV/c}^2$.

Freeze-out occurs when $k_{B}T\approx 0.7\text{ MeV}$ which keeps $\frac{N_{n}}{N_{p}}$ constant.
$$\left( \frac{N_{n}}{N_{p}} \right)_{FO}=\exp\left[ -\frac{1.3}{0.7} \right]=0.156.$$
Stage 2: Free neutron decay ($0.1\text{ MeV}<k_{B}T<0.7\text{ MeV}$)
$$n\to p+e^{-}+\bar{\nu}_{e}$$
$$n+p\leftrightarrow D+\gamma.$$
Neutrons and protons already start to form deuterium but deuterium bottleneck means means that $D$ cannot exist in large amounts.
$$D+D\leftrightarrow\; ^3He+n$$
$$D+D\leftrightarrow\; ^{3}H+p$$
$$^{3}H+D\to\;^{4}He+n$$
When $k_{B}T>0.1\text{ MeV}$ there are plenty of high energy photons in the exponential tail of the black body spectrum which can destroy newly formed deuterium. This is the deuterium bottleneck.

Stage 3: Nucleosynthesis ($k_{B}T\approx 0.1\text{ MeV}$)

$$D+D\leftrightarrow\; ^3He+n$$
$$D+D\leftrightarrow\; ^{3}H+p$$
$$^{3}H+D\to\;^{4}He+n$$
The final production needs energy of $17.6\text{ MeV}$. The synthesis of $^{4}He$ has a large binding energy so it is stable once formed. This turns nearly all neutrons into $^{4}He$.

There is an abundance of of helium in BBN. This $^{4}He$ abundance is expressed as the mass fraction of helium in all baryons - denoted by $Y$.

At the end of BBN, nearly all neutrons end up in helium-4 - each nucleus contains 2 neutrons and 2 protons.
$$\therefore N_{He}=\frac{N_{n}}{2}.$$
$$Y=\frac{N_{He}m_{He}}{N_{n}m_{n}+N_{p}m_{p}}.$$
Since $m_{n}\approx m_{p}$ and $m_{He}=4m_{p}$,
$$Y\approx \frac{\frac{N_{n}}{2}4\cancel{m_{P}}}{N_{n}\cancel{m_{p}}+N_{p}\cancel{m_{p}}}=\frac{2N_{n}}{N_{n}+N_{p}}.$$
$$Y=\frac{\frac{2N_{n}}{N_{p}}}{1+\frac{N_{n}}{N_{p}}}$$
where $\frac{N_{n}}{N_{p}}$ is the value at freeze-out, $0.156\therefore Y_{He}=0.27$.
Using the half life of this reaction $\approx 10\text{ mins}$ becomes
$$\frac{N_{n}}{N_{p}}=\exp\left[ -\frac{1.3}{0.7} \right]\left( \frac{1}{2} \right)^{t/T_{1/2}}\therefore Y_{He}=0.24.$$
This gives a good agreement with the true value.

Consider the interaction
$$e^{+}+n\to p+\bar{\nu}_{e}.$$
The weak interaction time scale is given by $\tau_{weak}\propto T^{-5}$, and considering the [expansion of the universe](Expanding%20Universe.md), $\tau_{exp}\propto T^{-2}$,
Freeze out occurs when $\tau_{exp}\approx \tau_{weak}$ to make sure the expansion doesn't change the paths of the colliding particles which causes the interaction to not happen.
$$\tau_{weak}\propto T^{-5};\;\tau_{exp}=\frac{a}{\dot{a}}=\frac{1}{H^2}.$$
Using the [[Friedmann Equation]],
$$H^2=\frac{8\pi G}{3} \frac{g_{*}}{2} \frac{4\sigma T^4}{c^3}.$$
$$\therefore T_{exp}\propto g_{*}T^{-2}.$$
Plotting the two time scales gives freeze out at $k_{B}T=0.7\text{ MeV}$. Freeze out is the point where the weak interaction can no longer keep equilibrium.
![[Pasted image 20250219160655.png]]
