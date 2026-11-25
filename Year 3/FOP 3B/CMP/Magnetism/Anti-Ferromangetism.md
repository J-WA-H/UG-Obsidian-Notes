Consider the [exchange energy](Exchange%20Interaction.md) $-J_{ij}\underline{s}_{i}\cdot \underline{s}_{j}$.
For $J_{ij}>0$, we get a [ferromagnet](Ferromagnetism.md)
For $J_{ij}<0$, we get an anti-ferromagnet, where there is no net magnetisation.
![[Pasted image 20250130151550.png]]
An anti-ferromagnet can be split into ferromagnetic sub lattices, $\uparrow\downarrow\uparrow\downarrow \equiv\uparrow\uparrow+\downarrow\downarrow$.
We can define the Weiss molecular field for the spin up/down lattices, where the dominant terms are the neighbouring atoms.
$$\underline{B}_{mf}^{\pm}=-|\lambda|\underline{M}^{\mp}.$$
Also $\underline{M}^{+}=-\underline{M}^{-}$ so $\underline{B}_{mf}^{\pm}=|\lambda|\underline{M}^{\pm}$.

Using results from ferromagnetism,
$$\frac{M^{\pm}}{M_{s}}=B_{J}(y^{\pm});\;y^{\pm}=\frac{g_{J}\mu_{B}J}{k_{B}T}(B+|\lambda| M^{\pm}).$$
Considering zero B field:
$$y^{+}=\frac{g_{J}\mu_{B}J}{k_{B}T}|\lambda|M^{+}\implies M^{+}=\frac{k_{B}T}{|\lambda|g_{J}\mu_{B}J}y^{+}.$$
![[Pasted image 20250130153221.png]]
This shows the spontaneous magnetisation of sub-lattices.
The linear gradient is proportional to temperature. At the Néel temperature, $T_N$, $M^{+},M^{-}\to 0$. This is the phase transition to a [paramagnet](Paramagnetism.md)
![[Pasted image 20250130153625.png]]
Unlike ferromagnets, anti-ferromagnets have no net magnetisation.

Applying a B field to a paramagnet shifts the linear $M$ graph, as the total $B$ field is $B-|\lambda|M$.
![[Pasted image 20250130154049.png]]

Here there is only one intersection.

For a $J=\frac{1}{2}$ solid, 
$$\frac{M}{M_{s}}=\frac{\mu_{B}}{k_{B}T}(B-|\lambda|).$$
For weak magnetic solids, $\chi=\frac{\mu_{0}M}{B}$
$$\implies \chi=\frac{\mu_{0}\mu_{B}M}{k_{B}\left[ T+\frac{|\lambda|\mu_{B}M_{s}}{k_{B}} \right]}\propto \frac{1}{T+T_{N}}.$$
![[Pasted image 20250130154402.png]]
Now we can generalise susceptibilities
$$\frac{1}{\chi}\propto T-\theta$$
where
$$\theta=\begin{cases}
>0 & \text{Ferromagnet} \\
<0 & \text{Anti-Ferromagnet} \\
0 & \text{Paramagnet}
\end{cases}.$$
For a parallel $B$ field to $M$, it tries to align $M^{+},M^{-}$.
![[Pasted image 20250130154827.png]]
For an orthogonal $B$ to $M$, there is a slight tilt by an angle $\phi$.
![[Pasted image 20250130154910.png]]
