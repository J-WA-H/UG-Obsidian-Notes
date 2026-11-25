The conservation of [[4-Momentum]] links the conservation of energy, $E$ and 3-momentum, $\underline{p}$.

Consider an electron with energy $E$ scattering of a proton at rest.
![[Pasted image 20250118124713.png]]
The 4-momentum of the electron before is
$$p=\begin{bmatrix}
E \\
0 \\
0 \\
E
\end{bmatrix}.$$
This assumes the rest mass of the electron is negligible, so in [[Natural Units]] $|\underline{p}|=E$.
The proton has an electron of
$$q=\begin{bmatrix}
m_{p} \\
0 \\
0 \\
0
\end{bmatrix}.$$
After the collision, 
$$p'=\begin{bmatrix}
E' \\
E'\sin \theta \\
 0 \\
E'\cos \theta
\end{bmatrix}.$$
As $p,q,p'$ are known, we can calculate $q'$ from 4-momentum conservation, $p+q=p'+q'\implies q'=p+q-q'$.

When $q\to q'$, we then include recoil. For recoil, $q=p-p'$.
This then gives
$$q=\begin{bmatrix}
E-E' \\
\underline{p}-\underline{p}'
\end{bmatrix}\implies -q^2=-[(E-E')^2-|\underline{p}-\underline{p}'|^2]=Q^2.$$
Moving to the rest frame of the proton and using the fact that the [Minkowski norm](Lorentz%20Transforms.md) is invariant we get
$$Q^2=-q^2=2(E-E')m_{p}.$$
This gives an updated [scattering formula](Cross-Sections.md), taking into account relativity, recoil, for a point charge by modifying the Mott cross-section.
$$\left( \frac{d\sigma}{d\Omega} \right)_{Rel}=\left( \frac{d\sigma}{d\Omega} \right)_{Mott}\left( 1+2\tau \tan^2 \frac{\theta}{2} \right).$$
