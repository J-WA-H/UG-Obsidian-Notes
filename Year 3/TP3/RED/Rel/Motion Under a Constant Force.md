Classically, a particle moving under a constant force that starts at rest undergoes motion $x(t)=\frac{at^2}{2}.$ 
In the relativistic regime, $\underline{F}=\frac{d}{dt}(m\gamma \underline{v})$. Integrating this gives
$$m\gamma \underline{v}=\underline{F}t$$
$$\implies \frac{mv}{\sqrt{ 1-\frac{v^2}{c^2}}} =Ft$$
$$v(t)=\frac{\left( \frac{F}{m} \right)t}{\sqrt{ 1+\left( \frac{Ft}{mc} \right)^2 }}.$$
In the limit as $t\to \infty$:
$$\lim_{ t \to \infty } \frac{\left( \frac{F}{m} \right)t}{\sqrt{ 1+\left( \frac{Ft}{mc} \right)^2 }}= \frac{\left( \frac{F}{m} \right)t}{\left( \frac{Ft}{mc} \right)} =c.$$
This shows that we cannot travel faster than the speed of light.

We can solve this for $x(t)$.
$$x(t)=\int_{0}^tv(t')dt'=\frac{F}{m}\int_{0}^tdt' \frac{t'}{\sqrt{ 1+\left( \frac{Ft}{mc} \right)^2 }}=\frac{mc^2}{F}\left( \sqrt{ 1+\left( \frac{Ft}{mc} \right)^2 }-1 \right)$$
Relativistic particles undergo hyperbolic motion.
![[Pasted image 20241026170949.png]]

The work applied over the particle is
$$W=\int \underline{F}\cdot d\underline{l}=E_{rel_{f}}-E_{rel_{0}}.$$
