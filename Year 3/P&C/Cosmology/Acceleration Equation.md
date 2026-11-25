Starting with differentiating the [[Friedmann Equation]]:
$$\frac{d}{dt}\left( \left( \frac{\dot{a}}{a} \right)^2 \right)=\frac{d}{dt}\left[ \frac{8\pi G\rho}{3}-\frac{kc^2}{a^2} \right]$$
$$\implies\frac{\dot{a}}{a} \frac{d}{dt}\left( \frac{\dot{a}}{a} \right)=\frac{8\pi G\dot{\rho}}{3}+2 \frac{kc^2}{a^2}\left( \frac{\dot{a}}{a} \right)$$
$$2 \frac{\dot{a}}{a}\left[ \frac{\ddot{a}}{a}-\left( \frac{\dot{a}}{a} \right)^2 \right]=-\frac{8\pi G}{3}\left[ 3 \frac{\dot{a}}{a}\left( \rho+ \frac{P}{c^2} \right) \right]+\frac{2kc^2}{a^2} \frac{\dot{a}}{a}$$
$$\frac{\ddot{a}}{a}-\left( \frac{\dot{a}}{a} \right)^2=-4\pi G\left( \rho+\frac{P}{c^2} \right)+\frac{kc^2}{a^2}.$$
Plugging the Friedmann equation into this:
$$\frac{\ddot{a}}{a}=\frac{8\pi G}{3}\rho-\frac{kc^2}{a^2}-4\pi G\left( \rho + \frac{P}{c^2} \right)+\frac{kc^2}{a^2}$$
$$\implies \frac{\ddot{a}}{a}=-\frac{4\pi G}{3}\left( \rho+\frac{3P}{c^2} \right).$$
This is the acceleration equation.

For $P(t)>-\frac{1}{3}\rho(t)c^2$, $\ddot{a}<0$ so the universe is decelerating.
For $P(t)<-\frac{1}{3} \rho(t)c^2$ there is an accelerated expansion.

The equation of state is given by
$$w\equiv \frac{P}{\rho c^2}$$
where
$$w=\begin{cases}
0 & \text{matter} \\
\frac{1}{3} & \text{radiation} \\
-1 & \text{cosmological constant}
\end{cases}$$
This gives the [matter and radiation pressure](Pressure%20of%20the%20Universe.md).
Using this the [[Fluid Equation]] becomes
$$\dot{\rho}+3 \frac{\dot{a}}{a}[(1+w)\rho]=0$$
$$\dot{\rho}=-3(1+w) \frac{\dot{a}}{a}$$
$$\frac{{d\ln \rho}}{dt}=-3(1+w) \frac{{d\ln a}}{dt}$$
$$\ln \rho=-4(1+w)\ln a+c$$
$$\implies \rho(t)=\rho_{0}a^{-3(1+w)}.$$
This gives
$$\rho_{R}\propto a^{-4};\;\rho_{M}\propto a^{-3};\;\rho_{\Lambda}=\text{const}.$$
