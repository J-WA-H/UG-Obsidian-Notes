We live in 3 spatial dimensions so problems often require a multi-dimensional integral.
Example: Gaussian Integral
$$I=\int_{-\infty}^{\infty}e^{ -x^2 }dx$$
$$I^2=\int_{-\infty}^{\infty}e^{-x^2}dx \int_{-\infty}^{\infty} e^{ -y^2 }dy=\int_{-\infty}^{\infty}dx \int_{-\infty}^{\infty}dye^{ -(x^2+y^2) }.$$
Rewrite in polar coordinates.
The area element is $da=dxdy$.
This integration is over all area elements.
In polar coordinates,
![[Pasted image 20250321093524.png]]
Here, $da=rdrd\theta$.
$$\therefore \int da=\int_{0}^{R}rdr\int_{0}^{2\pi}d\theta=\pi R^2.$$
The factor of $r$ comes from the Jacobian.
The Jacobian is defined by
$$J=\begin{vmatrix}
\frac{ \partial x }{ \partial r }  & \frac{ \partial x }{ \partial \theta } \\
\frac{ \partial y }{ \partial r }  & \frac{ \partial y }{ \partial \theta }  
\end{vmatrix}.$$
In polar coordinate, $x=r\cos\theta$, $y=r\sin\theta$.
$$\frac{ \partial x }{ \partial r } =\cos\theta;\; \frac{ \partial x }{ \partial \theta } =-r\sin\theta ;\; \frac{ \partial y }{ \partial r } =\sin\theta;\; \frac{ \partial y }{ \partial \theta } =r\cos\theta.$$
$$\therefore J=\begin{vmatrix}
\cos\theta & -r\sin\theta \\
\sin\theta & r\cos\theta
\end{vmatrix}=r\cos^2\theta+r\sin^2\theta=r.$$

Going back to the integral,
$$I^2=\int_{0}^{\infty}r dr\int_{0}^{2\pi}d\theta e^{ -r^2 }=2\pi \int_{0}^{2\pi}drre^{-r^2}=2\pi\left[ -\frac{1}{2}e^{-r^2} \right]_{0}^{\infty}=\pi$$
$$\implies I=\sqrt{ \pi }.$$
