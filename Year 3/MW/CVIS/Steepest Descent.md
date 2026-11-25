Consider a strongly peaked function.
![[Pasted image 20250321094256.png]]
For example,
$$I=\int_{-\infty}^{\infty}e^{ -\cosh x }dx.$$
This peaks around $x=0$.
$\cosh x$ can be expanded as a Taylor series,
$$\cosh x\approx 1+\frac{x^2}{2}+\dots$$
$$\therefore I\approx \int_{-\infty}^{\infty} e^{ -1-x^2/2 }dx.$$
Let $x=\sqrt{ 2 }u$, $dx=\sqrt{ 2 }du$.
$$I=\int_{-\infty}^{\infty} \frac{1}{e} e^{-u^2}\sqrt{ 2 }du=\frac{\sqrt{ 2\pi }}{e}.$$
Generally, if a function is peaked around $x=x_{0}$, it can be Taylor expanded around $x_{0}$.
As this is a peak, $f'(x_{0})=0$ so in general,
$$\int_{-\infty}^{\infty}e^{ -f(x) }dx\approx \int_{-\infty}^{\infty} e^{ -f(x_{0})-f''(x_{0})(x-x_{0})^2/2 }dx$$
$$=e^{ -f(x_{0}) }\int_{-\infty}^{\infty}dxe^{ -f''(x_{0})(x-x_{0})^2/2 }.$$
Let $u=x-x_{0}$, $dx=du$.
$$I=e^{ -f(x_{0}) }\int_{-\infty}^{\infty}due^{ -f''(x_{0})u^2/2 }$$
$$=e^{ -f(x_{0}) }\sqrt{ \frac{2\pi}{f''(x_{0})} }.$$
For another case,
$$\int_{-\infty}^{\infty}e^{f(x)}dx\approx \int_{-\infty}^{\infty} dxe^{ f(x_{0})+f''(x_{0})(x-x_{0})^2/2 }=e^{ f(x_{0}) }\int_{-\infty}^{\infty}e^{ -|f''(x_{0})|(x-x_{0})^2/2 }.$$
As $f''(x_{0})<0$ for a maximum, $f''(x_{0})=-|f''(x_{0})|$.
$$\therefore I=e^{ f(x_{0}) }\sqrt{ \frac{2\pi}{|f''(x_{0})|} }.$$
