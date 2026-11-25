The first problem is the horizon problem.
The horizon is the physical distance travelled by light from the big bang to time $t$. This is the maximal range of causality.
$$l_{H}(t)=a(t)\int_{0}^{t} \frac{cdt'}{a(t')}.$$
Consider 2 points in the [[Cosmic Microwave Background]]. In the time between the big bang and recombination, the two points haven't had enough time to communicate with each other so there is no explanation as to why it has a uniform temperature.
![[Pasted image 20250311134552.png]]
The circle around the point is the horizon. The angular size of the horizon is given by the [[Angular Diameter Distance]],
$$\Theta=\frac{l_{H}(t_{rec})}{d_{A}(z=0\to z_{rec})}.$$
$$l_{H}=a(t_{rec})\int_{0}^{t_{rec}} \frac{cdt'}{a(t')}.$$
This can be split into the integrals over the matter dominated and radiation dominated eras.
$$l_{H}=a_{rec}\left[ \cancelto{0}{\int_{0}^{t_{eq}} \frac{cdt'}{a_{R}(t')}} +\int_{t_{eq}}^{t_{req}} \frac{cdt'}{a_{M}(t')} \right].$$
The contribution from the radiation era is negligible as $t_{eq}\ll t_{rec}$.
At the matter-radiation equality, it is not exactly described by the matter dominated cosmic scale factor, so this is only an approximation.
Using $a_{M}(t)=\left( \frac{t}{t_{0}} \right)^{2/3}$,
$$l_{H}\approx a_{rec}c\int _{t_{eq}}^{t_{rec}} \frac{dt'}{\left( \frac{t'}{t_{0}} \right)^{2/3}}=a_{rec}ct_{0}^{2/3}\int_{t_{eq}}^{t_{rec}}t'^{-2/3}dt'=a_{rec}ct_{0}^{2/3}[3t^{1/3}]_{t_{eq}}^{t_{rec}}$$
$$=3a_{rec}ct_{0}^{2/3}(t_{rec}^{1/3}-t_{eq}^{1/3})\approx 3a_{rec}ct_{0}^{2/3}t_{rec}^{1/3}.$$
Evaluating $t_{rec}$,
$$a_{rec}=\left( \frac{t_{rec}}{t_{0}} \right)^{2/3}\implies t_{rec}=t_{0}a^{3/2}$$
$$\implies l_{H}=3ct_{0}a_{rec}^{3/2}.$$
Now evaluate $d_{A}$:
$$d_{A}=a_{rec}\int_{t_{rec}}^{t_{0}} \frac{c}{a(t')}dt'=a_{rec}\int_{t_{rec}}^{t_{0}} \frac{c}{\left( \frac{t'}{t_{0}} \right)^{2/3}}dt'=a_{rec}ct_{0}^{2/3}\int_{t_{rec}}^{t_{0}}t'^{-2/3}dt'=4a_{rec}ct_{0}^{2/3}[t_{0}^{1/3}-\cancel{t_{rec}^{1/3}}]$$
$$\approx 3a_{rec}ct_{0}.$$
$$\therefore \Theta=\frac{l_{H}}{d_{A}}=\frac{3ct_{0}a_{rec}^{3/2}}{3ct_{0}a_{rec}}=\sqrt{ a_{rec} }=\sqrt{ \frac{1}{1+z_{rec}} }=\sqrt{ \frac{1}{1+1089} }\ll {1}$$
using the fact that at recombination, $z=1089$.

As $\Theta$ is so small, the two points on the surface of last scattering can't communicate in the given time so there is no explanation to the uniform temperature of the CMB.

Another problem is the flatness problem.
Consider the [[Friedmann Equation]],
$$H^2=\frac{8\pi G}{3}\rho-\frac{kc^2}{a^2}\implies 1=\frac{8\pi G\rho}{3H^2}-\frac{kc^2}{a^2H^2}.$$
The first term is defined as $\Omega(t)$, so we use the second term to define the quantity
$$\Omega_{k}(t)=-\frac{kc^2}{a^2H^2}=-\frac{kc^2}{\dot{a}^2}.$$
Today, $|\Omega_{k_{0}}|\lesssim 10^{-2}$, so the universe is mostly flat.
To calculate this at matter-radiation equality, consider the ratio with the value today.
$$\frac{|\Omega_{k}(t_{eq})|}{|\Omega_{K_{0}}|}=\left[ \frac{\dot{a}(t_{0})}{\dot{a}(t_{eq})} \right]^2$$
Using the matter dominated era, $a(t)\propto t^{2/3}$ so $\dot{a}\propto t^{-1/3}$.
$$=\left( \frac{t_{eq}}{t_{0}} \right)^{2/3}=a_{eq}=4\times 10^{-5}$$
$$\implies |\Omega_{k}(t_{eq})|^2=4\times 10^{-7}.$$
At the Planck time (time of recombination), $t_{P}\sim 10^{-43}\text{ s}$. To calculate $\Omega_{k}(t_{rec})$, consider
$$\frac{|\Omega_{k}(t_{P})|}{|\Omega_{k}(t_{eq})|^2}=\left( \frac{\dot{a}(t_{eq})}{\dot{a}(t_{p})} \right)^2=\frac{t_{P}}{t_{eq}}=\frac{10^{-43}}{t_{eq}}.$$
To evaluate $t_{eq}$:
$$a(t_{rec})=\left( \frac{t_{eq}}{t_{0}} \right)^{2/3}\implies t_{eq}=t_{0}a^{3/2}_{eq}.$$
$$\therefore \frac{t_{p}}{t_{eq}}=\frac{t_{p}}{t_{0}a_{rec}^{3/2}}=\frac{10^{-43}}{3\times 10^{17}\times 4\times 10^{-6}}\cong 5\times 10^{-61}.$$
This predicts the universe to be incredibly flat which is unnatural given the initial conditions of the universe.

The final problem is the relic particle abundance problem.
In the standard model, relativistic species exist as particles and antiparticles. When $k_{B}T<mc^2$, the particle-antiparticle pairs annihilate and inject the resulting energy into the remaining relativistic species.
In Grand unified theories, stable particles of mass  $\sim 10^{15}\text{GeV/c}^2$ exist in the early universe. These particles should have become non relativistic very early on, and quickly turn the universe into the matter dominated era. They would also dominate the density of the universe today, but we know this is not true.