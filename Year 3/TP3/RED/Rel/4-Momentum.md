4-momentum is defined by
$$p^\mu=mu^\mu=m\gamma(c,\underline{v}).$$
The temporal component is the total energy.

The kinetic energy is given by
$$T=\int \underline{F}\cdot d\underline{x}=\int \frac{d\underline{p}}{dt}\cdot d\underline{x}=\int \frac{d}{dx}(m\gamma \underline{v})\cdot d\underline{x}=\int\left( m \frac{d\gamma}{dt}\underline{v}+m\gamma  \frac{d\underline{v}}{dt} \right)\cdot d\underline{x}$$
$$\frac{d\gamma}{dt}=-\frac{1}{2}\left( 1-\frac{v^2}{c^2} \right)^{-3/2}\left( -\frac{2v}{c^2} \frac{dv}{dt} \right)=\frac{v}{c^2} \frac{1}{\left( 1-\frac{v^2}{c^2} \right)^{3/2}} \frac{dv}{dt}.$$$$T=\int\left[ m \frac{v^2}{c^2} \frac{1}{\left( 1-\frac{v^2}{c^2} \right)^{3/2}} \frac{d\underline{v}}{dt} +m \frac{1}{\sqrt{ 1-\frac{v^2}{c^2} }} \frac{d\underline{v}}{dt} \right]\cdot \underline{v}dt$$
$$=\int \frac{m}{\left( 1-\frac{v^2}{c^2} \right)^{3/2}}\left( \frac{v^2}{c^2}+1-\frac{v^2}{c^2} \right) \frac{d\underline{v}}{dt}\cdot \underline{v}dt=\int mc^2 \frac{d\gamma}{dt}dt=mc^2(\gamma-1).$$
This shows for a particle that starts at rest, $T=mc^2(\gamma-1)$.

In the non-relativistic regime, $v<<c$ so we can expand $\gamma$ as a Taylor series:
$$\gamma=\left( 1-\frac{v^2}{c^2} \right)^{-1/2}=1+\frac{v^2}{2c^2}+\mathcal{O}\left( \frac{v^4}{c^4} \right)$$
$$\implies T\approx mc^2\left( 1+\frac{v^2}{2c^2}-1 \right)=\frac{1}{2}mv^2.$$
We can find the total energy by summing the kinetic energy with the rest mass
$$E=T+E_{0}=mc^2(\gamma-1)+mc^2=\gamma mc^2.$$
Using this we can rewrite $p^\mu$ as
$$p^\mu=\left( \frac{E}{c}, \underline{p} \right)=(m\gamma c,m\gamma \underline{v}).$$
Minkowski norm:
$$p^\mu p_{\mu}=\frac{E^2}{c^2}-p^2$$
using the rest frame we can evaluate the norm:
$$p^\mu p_{\mu}=m^2c^2$$
From this we get the result
$$E^2=p^2c^2+m^2c^4.$$
