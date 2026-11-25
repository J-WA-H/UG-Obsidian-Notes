### Anomalies
Mean anomaly grows linearly with time since periapsis at $t=\tau$ and reaches $M=2\pi$ after one period
$$M=\frac{2\pi(t-\tau)}{T}$$
#### Relating true and eccentric anomalies
![[Pasted image 20241015130835.png]]
For an ellipse: $|OF|=ae$
so $FR=r\cos \varphi=a(\cos E-e).$
For an ellipse contained within a circle,
$$\frac{|QR|}{|AR|}=\frac{b}{a}$$
so $r\sin \varphi=(a\sin E)\left( \frac{b}{a} \right)=a\sqrt{ 1-e^2 }\sin E$.
Sum of squares to eliminate $\varphi$
$$r^2=a^2(\cos E-e)^2+a^2(1-e^2)\sin^2E=a^2(1-e\cos E)^2$$
$$\therefore r=a(1-e\cos E).$$
Simultaneous equations:
$$r\cos \phi=a(\cos E-e)$$
$$r=a(1-e\cos E)$$
Can solve via:
$$r(1-\cos \phi)=a(1+e)(1-\cos E)$$
$$r(1+\cos \phi)=a(1-e)(1+\cos E)$$
to give
$$\frac{{1-\cos \phi}}{1+\cos \phi}=\frac{(1+e)(1-\cos E)}{(1-e)(1+\cos E)}$$
which simplifies to
$$\tan\left( \frac{\phi}{2} \right)=\sqrt{\frac{{1+e}}{1-e} }\tan\left( \frac{E}{2} \right)$$

Both mean anomaly and area swept out grow linearly with time so
$$FQP=\frac{\pi ab(t-\tau)}{T}\equiv\frac{abM}{2}$$
Also
$$FQP=\frac{b}{a}(ARP)-FQR$$
$$=\frac{b}{a}(AOP-AOR)-FQR$$
$$\therefore \frac{abM}{2}=\frac{b}{a}\left( \frac{1}{2}a^2E-\frac{1}{2}a^2\sin E\cos E \right)+\frac{1}{2}r^2\sin \phi \cos \phi$$
Eliminating $\phi$:
$$M=E-e\sin E$$
Solving Kepler's equation
$$E_{0}=M$$
$$E_{1}=M+e\sin E_{0}$$
$$E_{i+1}=M+e\sin E_{1}$$
This recurrence relation converges quickly provided eccentricity is low.

True anomaly is measure from the focus but the eccentric and mean anomalies are measured from the centre of mass