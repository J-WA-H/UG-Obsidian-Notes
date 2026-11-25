4-acceleration is defined by
$$a^\mu=\frac{d^2x^\mu}{d\tau^2}=\frac{du^\mu}{d\tau}$$
Like [4-velocity](4-Velocity.md), 4-acceleration is contravariant as $a'^\mu=\Lambda^\mu_{\;\nu}a^\nu.$ 
It can be expressed as
$$a^\mu=\frac{du^\mu}{d\tau}=\gamma\frac{d}{dt} (\gamma c,\gamma\underline{v})=\gamma\left( c \frac{d\gamma}{dt}, \frac{d\gamma}{dt}\underline{v}+\gamma \underline{a} \right)$$
In the rest frame, $a^\mu=(0,\underline{\alpha})$ where $\underline{\alpha}$ the the 3-acceleration in the rest frame.

Minkowski norm:
$$a^\mu a_{\mu}=-\alpha^2.$$
Now take the product of 4-velocity and 4-acceleration
$$u^\mu a_{\mu}=\gamma^2\left( c^2 \frac{d\gamma}{dt}-\frac{d\gamma}{dt}v^2-\gamma \underline{a}\cdot \underline{v} \right)=\gamma^2\left( \frac{d\gamma}{dt}(c^2-v^2)-\gamma \underline{a}\cdot \underline{v} \right)=\gamma^2\left( \frac{v}{c^2}\gamma^3a(c^2-v^2)-\gamma \underline{a}\cdot \underline{v} \right)$$
$$=\gamma^3\underline{a}\cdot \underline{v}\left( \frac{1}{c^2}\gamma^2(c^2-v^2)-1 \right)=\gamma^3\underline{a}\cdot \underline{v}\left( \frac{1}{c^2} \frac{{c^2-v^2}}{1-\frac{v^2}{c^2}}-1 \right)=0.$$
This shows that the scalar product $u^\mu a_{\mu}=0$.