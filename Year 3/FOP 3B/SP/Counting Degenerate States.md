With classical particles we can count particles in degenerate states as if they were distinguishable, but with quantum particles they are indistinguishable.
Consider 3D infinite potential well where
$$\varepsilon=\frac{\hbar^{2}}{2m}(k_{x}^2+k_{y}^2+k_{z}^2).$$
We can see that the energy levels of this system are degenerate, and we can plot these degeneracies.
![[Pasted image 20241107191454.png]]
For this discrete distribution we call $g$ degeneracy.

![[Pasted image 20241107192120.png]]
The continuous distribution is called the density of states.

If we have $n(k)$ states at $k$ and $n(k+dk)$ states at $k+dk$ then $g(k)dk=n(k+dk)-n(k)$
$$\implies g(k)=\frac{dn}{dk}.$$
Now plot all possible states:
![[Pasted image 20241107192556.png]]
We have a spherical shell of radius $k$, and at $k+dk$. The number of states between these shells are the volume of the shell divided by the volume of the quantum state, $\frac{\pi^3}{a^3}$.
$$g(k)dk=\frac{1}{8} \frac{4\pi k^2dk}{\left( \frac{\pi}{a} \right)^3}=\frac{1}{8} \frac{4k^2a^3dk}{\pi^2}.$$
We can see that $g(k)\propto k^2$. We can change variables to energy to momentum $p=\hbar k$.
$$\varepsilon=\frac{\hbar^2k^2}{2m}.$$
$$\frac{d\varepsilon}{dk}=\frac{\hbar^2}{m}kdk\text{ and } k=\sqrt{ \frac{2m\varepsilon}{\hbar^2} }\implies dk=\sqrt{ \frac{2m}{\hbar^2\varepsilon} }d\varepsilon.$$
$$g(k)dk=\frac{V}{2\pi^2}k^2dk\implies g(\varepsilon)d\varepsilon=\frac{V}{2\pi^2} \frac{2m\varepsilon}{\hbar^2}\sqrt{ \frac{2m}{\hbar^2\varepsilon} }d\varepsilon$$$$=\frac{V}{\pi^2\hbar^2}\sqrt{ 2m^3\varepsilon }d\varepsilon.$$


