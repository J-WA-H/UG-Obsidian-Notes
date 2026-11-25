Everything so for has been for elastic scatter, where the particle types are conserved.

Now consider inelastic scattering, where we create new particles and excite bound ones:
![[Pasted image 20250123185637.png]]
For elastic scattering, $w^2=m_{p}^2$ but for inelastic scattering $w^2\neq m_{p}^2$.
$$p_{e}=\begin{bmatrix}
E \\
\underline{p}_{e}
\end{bmatrix};\;p_{e}'=\begin{bmatrix}
E' \\
\underline{p}'_{e}
\end{bmatrix}\;p_{p}=\begin{bmatrix}
E \\
\underline{0}
\end{bmatrix}.$$
[We know](4-Momentum%20Conservation.md) $q=p_{e}-p_{e}'$:
$$q=\begin{bmatrix}
E-E' \\
\underline{p}_{e}-\underline{p}_{e}'
\end{bmatrix}.$$
Define a new quantity $\nu$:
$$\nu=\frac{{p_{p}\cdot q}}{m_{p}}=E-E'.$$
$\nu$ gives the change in energy.
Looking at $w$:
$$w=p_{e}+p_{p}-p_{e}'.$$
For 4-momentum calculations it is usually good to 4-momentum squared.
$$\implies w^2=(p_{e}+p_{p}-p_{e}')^2=(p_{p}+q)^2=p_{p}^2+2p_{p}q+q^2$$
$$=p_{p}^2+2p_{p}q-Q^2$$
$$\implies w^2=p_{p}^2+2m_{p}\nu-Q^2.$$
In elastic scattering we had $w^2=p_{p}'^2=m_{p}^2$ so we can read off $2m_{p}\nu-Q^2=0$ or $Q^2=2m_{p}(E-E')$ but for inelastic scattering, $w^2>m_{p}^2$ i.e. $2m_{p}\nu-Q^2>0$. It appears that $\nu$ is some sort of measure as to how inelastic a collision is.

We call excitation of particles in inelastic scattering as new particles, e.g. the first excitation state of a proton is $\Delta^{+}$. There are several ways to excite a compound object, particularly given the degrees of freedom in quantum mechanics. The lowest energy excitation is most likely a spin flip.
$$p \text{ spin } \frac{1}{2}\to \Delta^{+} \text{ spin } \frac{3}{2}.$$
Naming conventions:
- Elastic scattering: No change other than velocity (particle unchanged)
- Inelastic scattering: particle is excited into a higher energy state, e.g. $\Delta^{+}$
- Deep inelastic scattering: particle no longer exists, it has changed into a number of other products.

