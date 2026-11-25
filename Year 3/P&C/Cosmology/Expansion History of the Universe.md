We can find expressions for the [[Cosmic Scale Factor]] for each [era](Standard%20Cosmological%20Model.md) of the universe.
Consider the radiation era where $a\ll a_{eq}$, $\rho_{R}\gg \rho_{M},\rho_{\Lambda}$.
$$\frac{H^2}{H_{0}^2}=\Omega_{R_{0}}a^{-4}\implies a(t)=(2H_{0}\sqrt{ \Omega_{R_{0}} }t)^{1/2}\implies H(t)=\frac{1}{2t}.$$
This is the same result as the radiation only universe [cosmological mode](Cosmological%20Models.md).

Now consider the matter dominated era where $a_{eq}\ll a\ll a_{eq}^{M\Lambda}$.
$$\frac{H_{0}^2}{H_{0}^2}=\Omega_{M_{9}}a^{-3}\implies a(t)=\left( \frac{3}{2}H_{0}\sqrt{ \Omega_{M_{0}} }t \right)^{2/3}\implies H(t)=\frac{2}{3t}.$$
Now for the $\Lambda$ dominated era:
$$\left( \frac{\dot{a}}{a} \right)^2=H_{0}^2(\Omega_{M_{0}}a^{-3}+\Omega_{\Lambda_{0}})\;\times a^{6}$$
$$a^4\dot{a}^2=H_{0}^2(\Omega_{M_{0}}a^{3}+\Omega_{\Lambda_{0}}a^6)\;\sqrt{  }$$
$$a^2\dot{a}=H_{0}\sqrt{ \Omega_{\Lambda_{0}} }\left( a^6+\frac{\Omega_{M_{0}}}{\Omega_{\Lambda_{0}}}a^3 \right)^{1/2}$$
$$\frac{1}{3}\frac{d}{dt}(a^3)=H_{0}\sqrt{\Omega_{\Lambda_{0}} }\sqrt{ \left( a^3+\frac{\Omega_{M_{0}}}{\Omega_{\Lambda_{0}}} \right)^2-\frac{\Omega_{M_{0}}^2}{4\Omega_{\Lambda_{0}}^2} }.$$
Let $\xi=\frac{\Omega_{M_{0}}}{2\Omega_{\Lambda_{0}}}$:
$$\frac{1}{3} \frac{d}{dt}(a^3+\xi)=H_{0}\sqrt{ \Omega_{\Lambda_{0}} }[(a^3+\xi)^2-\xi^2]^{1/2}$$
Let $x=a^3+\xi$:
$$\frac{1}{3} \frac{dx}{dt}=H_{0}\sqrt{ \Omega_{\Lambda_{0}} }\sqrt{ x^2-\varepsilon^2 }$$
$$\int \frac{dx}{\sqrt{ x^2-\xi^2 }}=\int 3H_{0}\sqrt{ \Omega_{\Lambda_{0}} }dt$$
$$\cosh ^{-1}\left( \frac{x}{\xi} \right)=3H_{0}\sqrt{ \Omega_{\Lambda_{0}} }t+c$$
As we want a big bang, $a(0)=0$ so $c=0$
$$x=\xi \cosh(3H_{0}\sqrt{ \Omega_{\Lambda_{0}} }t)$$
$$a^3=\xi[\cosh(3H_{0}\sqrt{ \Omega_{\Lambda_{0}} }t)-1]$$
$$=2\xi\sinh^2\left( \frac{3}{2}H_{0} \sqrt{ \Omega_{\Lambda_{0}} }t\right)$$
$$\therefore a(t)=\left( \frac{\Omega_{M_{0}}}{\Omega_{\Lambda_{0}}} \right)^{1/3}\sinh^{3/2}\left( \frac{3}{2}H_{0} \sqrt{ \Omega_{\Lambda_{0}} }t\right).$$
For the region where $a\gg a_{eq}^{M\Lambda}$,
$$a(t)\approx\left( \frac{\Omega_{M_{0}}}{4\Omega_{\Lambda_{0}}} \right)^{1/3}\exp(H_{0}\sqrt{ \Omega_{\Lambda_{0}}}t).$$
The age of the universe depends on the model.
$$t(1\to 2)=\int_{t_{1}}^{t_{2}}dt=\int_{a_{1}}^{a_{2}} \frac{dt}{da}da=\int_{a_{1}}^{a_{2}} \frac{da}{aH(a)}$$
$$=\int_{a_{1}}^{a_{2}} \frac{da}{aH_{0}\sqrt{ \Omega_{R_{0}}a^{-4}+\Omega_{M_{0}}a^{-3}+\Omega_{\Lambda_{0}} }}=\frac{1}{H_{0}}\int_{a_{1}}^{a_{2}} \frac{da}{\sqrt{ \Omega_{R_{0}}a^{-2}+\Omega_{M_{0}}a^{-1}+\Omega_{\Lambda_{0}}a^{2} }}.$$
Solving this gives $t_{0}\approx 0.95H_{0}^{-1}$.
