Like with [[Trigonometric Integrals]], we can use complex methods to evaluate integrals over the real line,
$$I=\int_{-\infty}^{\infty}f(x)dx=\oint_{C}f(z)dz$$
where $C$ is a semicircle in the upper $\mathbb{C}$ plane where $\lvert R \rvert\to \infty$. We use a semicircle as the contour must go along the real line as these are the boundaries of the real integral.
![[Pasted image 20241107124306.png]]
As we are integrating over the real line, we want the integral over the arc to go to zero. For this condition, we need $f$ to be a vanishing function.
The condition for a vanishing function is:
	$\lvert f(z) \rvert$ vanishes faster than $\frac{1}{\lvert z \rvert}$.

$$\lvert f(z) \rvert \to 0 \text{ faster than } \frac{1}{\lvert z \rvert }\to 0 \text{ as }\lvert z \rvert\to \infty. $$
The half of the plane we choose to integrate in is the half of the plane in which $f$ is vanishing. For example $e^{z}$ vanishes when $x>0$ so the top half of the right half plane would be used to integrate over. Note that if we are integrating in the lower half plane, the final answer from residue theorem needs to be multiplied by -1.

Example: 
$$I=\int_{-\infty}^{\infty} \frac{1}{x^2+1}dx.$$
Complexify the function
$$f(z)=\frac{1}{z^2+1}=\frac{1}{(z+i)(z-i)}.$$
Here we can see the poles are at $z=\pm i$. Take $C$ to be the semicircle in the upper half plane, so the only pole enclosed by $C$ is $z=i$.
We can now evaluate the integral by [[Residue Theorem]]:
$$\text{Res}[f,i]=\lim_{ z \to i } (z-i) \frac{1}{(z+i)(z-i)}=\lim_{ z \to i } \frac{1}{z+i}=\frac{1}{2i}.$$
$$\oint_{C} \frac{1}{z^2+1}dz=2\pi i\text{Res}[f,i]=\frac{2\pi i}{2i}=\pi.$$
This answer is real as expected.

If it is not clear which half of the plane to integrate over, like if the integrand is not a decaying function, so we use the closing contour
![[Pasted image 20241107151548.png]]
Example:
$$I=\int_{-\infty}^{\infty} \frac{{x\sin (\pi x)}}{1+x^{2}}dx.$$
Complexifying the function and writing $\sin$ in terms of exponentials gives
$$I=\oint_{C} \frac{z}{1+z^{2}}\left( \frac{{e^{i\pi z}-e^{-i\pi z}}}{2i} \right)dz.$$
It can be seen that for $e^{i\pi z}$,
$$\lim_{ z \to \infty } e^{i\pi z}=\lim_{ x,y \to \infty } e^{i\pi(x+iy)}=\lim_{ x,y \to \infty } e^{i\pi x}e^{-\pi y}=0$$
as $e^{-\pi y}$ goes to zero as $y\to \infty$, so is decaying in the upper half plane. However for $e^{-i\pi z}$, it does not vanish in the upper half plane - so that term has to be integrated over in the lower half plane.
$$I=\oint_{C_{+}}f_{+}dz+\oint_{C_{-}}f_{-}dz$$
where
$$f_{+}=\frac{ze^{i\pi z}}{2i(1+z^{2})};\;f_{-}=\frac{ze^{-i\pi z}}{2i(1+z^{2})}.$$
Like the last example, the poles are at $z\pm i$.
$$\text{Res}[f_{+},i]=\lim_{ z \to i } (z-i) \frac{ze^{i\pi z}}{2i(z-i)(z+i)}=\lim_{ z \to i } \frac{ze^{i\pi z}}{2i(z+i)}=-\frac{ie^{-\pi}}{4}$$
$$\text{Res}[f_{-},-i]=\lim_{ z \to -i }(z+i) \frac{ze^{-i\pi z}}{2i(z-i)(z+i)}=\lim_{ z \to -i } \frac{ze^{-i\pi z}}{2i(z-i)}=\frac{ie^{-\pi }}{4}.$$
$$\oint_{C} \frac{z\sin(\pi z)}{z^{2}+1}dz=2\pi i(\text{Res}[f_{+},i]-\text{Res}[f_{-},-i])=2\pi i\left( -\frac{ie^{-\pi}}{4}-\frac{ie^{-\pi}}{4} \right)=-\pi e^{-\pi}.$$
