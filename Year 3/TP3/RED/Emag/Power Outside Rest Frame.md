For the power outside the particle's rest frame, the relationship between the the radiation emitted is given by
$$\left( \frac{dW}{dt_{r}} \right)_{emit}=\left( \frac{dW}{dt} \right)_{measure} \frac{dt}{dt_{r}}.$$
First calculate $\frac{dt}{dt_{r}}$:
$$R=c(t-t_{r})\implies \underline{R}\cdot \underline{R}=c^2(t-t_{r}).$$
Taking the derivative with respect to time
$$2c^2\left( 1-\frac{dt_{r}}{dt} \right)(t-t_{r})=2\underline{R}\cdot \frac{d\underline{R}}{dt}.$$
The rate of change of $R$ is equivalent to the rate of change of the particles [world line](Fields%20of%20a%20moving%20point%20charge.md),
$$\frac{d\underline{R}}{dt}=-\frac{dw(t_{r})}{dt}=-\frac{dw(t_{r})}{dt_{r}} \frac{dt_{r}}{dt}=-\underline{v} \frac{dt_{r}}{dt}.$$
Substituting this back in gives
$$c\left( 1-\frac{dt_{r}}{dt} \right)=-\underline{R}\cdot \underline{v} \frac{dt_{r}}{dt}\implies cR=\frac{dt_{r}}{dt}(cR-\underline{R}\cdot \underline{v})=\frac{dt_{r}}{dt}R_\nu u^{\nu}.$$
This gives the derivative
$$\frac{dt_{r}}{dt}=\frac{cR}{\underline{u}\cdot \underline{R}}.$$
This gives the relationship between radiation emitted and measured, in terms of the solid angle, is
$$\left( \frac{dP}{d\Omega} \right)_{emit}=\left( \frac{\underline{R}\cdot \underline{u}}{Rc} \right) \left( \frac{dP}{d\Omega} \right)_{measure}.$$
Given that we know the [power emitted](Lienard-Wiechert%20Potentials.md) is $\frac{1}{\mu_{0}c}E_{rad}^2R^2$.
$$\left( \frac{dP}{d\Omega} \right)_{emit}=\left( \frac{\underline{R}\cdot \underline{u}}{Rc} \right) \frac{1}{\mu_{0}c}E_{rad}^2R^2$$
$$=\left( \frac{\underline{R}\cdot \underline{u}}{Rc} \right) \frac{1}{\mu_{0}c} \left( \frac{q}{4\pi\varepsilon_{0}} \right)^2 \frac{R^2}{(\underline{R}\cdot \underline{u})}[\underline{R}\times(\underline{u}\times \underline{a})]^2R^2$$
$$=\left( \frac{q}{4\pi\varepsilon_{0}} \right) \frac{(Rc)^5}{(\underline{R}\cdot \underline{u})^5} \frac{1}{R^2c^6} \frac{1}{\mu_{0}c}[\underline{R}\times(\underline{u}\times \underline{a})]^2$$
$$=\frac{q^2}{16\pi^2\varepsilon_{0}} \frac{1}{c} \frac{1}{(1-\underline{\hat{R}}\times \underline{\beta})^5} \left[ \underline{\hat{R}}\times(\underline{R}-\underline{\beta})\times \frac{d\underline{\beta}}{dt} \right]^2.$$
Integrating through the solid angle gives
$$P_{emit}= \frac{\mu_{0}q^2\gamma^6}{6\pi c}\left( a^2-\frac{{\lvert \underline{v}\times \underline{a} \rvert }}{c^2} \right).$$
This is Lienard's generalisation of [Larmor's formula](Lienard-Wiechert%20Potentials.md).
![[Pasted image 20241126152756.png]]
This can also be derived using [[4-Vectors]].
Consider the [[4-Momentum]] of the radiated energy,
$$p^\mu=\left( \frac{U_{rad}}{c},\underline{p}_{rad} \right).$$
In the rest frame, $d\underline{p}_{rad}=\underline{0},dr'=0$.
![[Pasted image 20241126154040.png]]
For the power outside the rest frame, we do a [[Lorentz Transforms]].
$$P=\frac{dU_{rad}}{dt}=\frac{\gamma(dU'_{rad}+\underline{v}\cdot \cancelto{0}{d\underline{p}_{rad}/c^2}}{\gamma(dt'+\cancelto{0}{\underline{v}\cdot d\underline{r}'/c^2)}}= \frac{dU'rad}{dt'}=\frac{dU_{rad}}{dt}.$$This implies total power radiated is invariant in all rest frames.

Now consider the rate of change of momentum:
$$\frac{d\underline{p}_{rad}}{dt}=\frac{\gamma(\cancelto{0}{d\underline{p}_{rad}}+dU'_{rad} \underline{v}/c^2)}{\gamma(dt'+\underline{v}\cdot \cancelto{0}{dr'/c^2})}=\frac{\underline{v}}{c^2} \frac{dU'rad}{dt'}=\frac{\underline{v}}{c^2} \frac{dU_{rad}}{dt}$$
so total 3-momentum isn't invariant.

In the rest frame,
$$P=\frac{\mu_{0}q^2a^2}{6\pi c}.$$
Using [[4-Acceleration]] in Larmor's formula:
$$a^\mu a_{\mu}=-\alpha^2$$
where $\alpha$ is the proper acceleration.
This gives
$$P(t)= \frac{\mu_{0}q^2}{6\pi c} \frac{1}{m^2} \frac{dp^\mu}{d\tau} \frac{dp_{\mu}}{d\tau}$$
using [[4-Force]].
$$\frac{dp^\mu}{d\tau} \frac{dp_{\mu}}{d\tau}=\frac{1}{c^2}\left( \frac{dE}{d\tau} \right)^2-\frac{d\underline{p}}{d\tau}\cdot \frac{d\underline{p}}{d\tau}$$
$$=(mc\gamma)^2\left[ \left( \frac{d\gamma}{dt} \right)^2-\frac{d(\gamma \underline{\beta})}{dt}\cdot \frac{d(\gamma \beta)}{dt} \right].$$
Considering $p^\mu=m\gamma(c,\underline{v})$,
$$P(t)=\frac{\mu_{0}q^2c}{6\pi}\gamma^6\left[ \left( \frac{d\beta}{dt} \right)^2-\left( \underline{\beta}\times \frac{d\underline{\beta}}{dt} \right)^2 \right]$$
$$=\frac{\mu_{0}q^2}{6\pi c} \frac{\gamma^2}{m^2}\left[ \left( \frac{d\underline{p}}{dt} \right)^2-\beta^2\left( \frac{dp}{dt} \right)^2 \right].$$
This is another form of Lienard's generalisation of Larmor's formula.