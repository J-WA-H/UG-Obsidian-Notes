### Complex functions
A complex function is a function that maps a set on the complex plane to another set
$$f:\mathbb{C}\rightarrow\mathbb{C}.$$
Functions are of the form $f(z)=u(x,y)+iv(x,y)$, where $u(x.y)$, $v(x,y)$ are real functions.

### Branch Points
A branch point is a point where rotating the function by $2\pi$ gives a different function.
	Example:
	$$\text{Consider } f(z)=z^{1/2}$$
	$$z=re^{i\phi}=re^{\phi+2\pi} \implies f(z)=r^{1/2}e^{i\phi/2}=r^{1/2}e^{i\phi/2}e^{i\pi}=-r^{1/2}e^{i\phi/2}$$
This shows that a rotation about the origin changes the sign of the function, so $z=0$ is a branch point.
	Example:
	$$\text{Check if z=1 is a branch point}$$
	$$z=1+\epsilon e^{i\theta}, \text{ where epsilon is small, it traces a small circle around z=1}$$
	$$f(z)=z^{1/2}=(1+\epsilon e^{i\theta})^{1/2}\approx 1+\frac{\epsilon}{2} e^{i\theta}$$
	$$\text{For } \theta=0,\text{ } f(z)=1+\frac{\epsilon}{2}$$
	$$\text{For } \theta=2\pi,\text{ } f(z)=1+\frac{\epsilon}{2}$$
	Rotation around $z=1$ preserves the function so it is not a branch point.

### Complex Logarithms
The inverse of the complex exponential is the complex logarithm, defined by
$$\ln z=\ln|z|+i\arg{z}.$$
Unlike the real log, this function is multi-varied as there are infinitely many values for the argument of $z$, as angles that have a phase of $2\pi n$ are equivalent. Normally we use the principle value of the argument where $n=0$.
	Example:
	
	$$\ln(2+2i):$$
	$$|2+2i|=\sqrt{2^2+2^2}=2\sqrt{ 2 },\text{ }\arg(2+2i)=\arctan\left( \frac{2}{2} \right)=\frac{\pi}{4}+2\pi n$$
	$$\therefore \ln(2+2i)=\ln(2\sqrt{ 2 })+\frac{i\pi}{4}+2i\pi n.$$
### Branch Cuts
To make a multi valued function single valued, branch cuts are made from the branch points to prevent a full rotation being made.
	Example:
	$$f(z)=\sqrt{ z^2-1 }$$
	The branch points appear when the function vanishes, so $z=\pm 1$, so two possible branch cuts are
	![[Pasted image 20241008165951.png]]
### Hyperbolic Functions
Consider a purely imaginary number $z=iy$.
$$\cos(z)=\frac{{e^{i(iy)}+e^{-i(iy)}}}{2}=\frac{{e^{-y}+e^y}}{2}=\cosh y$$
$$\sin z=\frac{{e^{i(iy)}-e^{-i(iy)}}}{2i}=\frac{{e^{-y}-e^y}}{2i}=i\sinh y$$
