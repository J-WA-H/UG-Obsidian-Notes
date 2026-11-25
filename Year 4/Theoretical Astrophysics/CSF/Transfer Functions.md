Plane wave density perturbations in the [growing mode](Density%20Perturbations%20Without%20Pressure.md) evolves as
$$\delta(\vec{x},a)\propto D_{+}(\vec{x},a)e^{ i\vec{k}\cdot \vec{x} }\tag{20.1} .$$
Dark matter perturbations grow due to gravity only for:
- $a<a_{enter}(t)$ [outside the horizon](Perturbations%20Outside%20Horizon.md) 
- $a>a_{eq}$ in the matter dominated era.

In the long wavelength limit,
$$D_{+}(k,a)\to D_{+}(a)\propto \begin{cases}
a^2 & a<a_{eq} \\
a & a_{eq}<a<a_{DE} \\
\text{const} & a>a_{DE}
\end{cases}.\tag{20.2} $$
For initial and final epochs, $a_{i}\ll a_{enter}(k)$ and $a_{f}\gg a_{eq}$, the total factor by which $\delta_{DM}$ grows is
$$\frac{\delta_{DM}(\vec{x},a_{f})}{\delta_{DM}(\vec{x},a_{I})}=\frac{D_{+}(k,a_{f})}{D_{+}(k,a_{i})}\equiv \frac{D_{+}(a_{f})}{D_{+}(a_{i})}T(k)\tag{20.3} .$$
$T(k)$ is the dark matter transfer function/

The $\frac{D_{+}(a_{f})}{D_{+}(a_{i})}$ gives the factor by which perturbations would grow due to gravity alone. $T(k)$ gives modification to this from other effects. The physical meaning of the transfer function is that it gives the net effect of pressure, Meszaros effect, free streaming on an amplitude of $\delta_{DM}$ for plane-wave density perturbations at late times relative to what it would have been with growth due to gravity only.

For $a_{enter}<a_{eq}$ ($\lambda_{com}<\ell_{H_{eq}}$):
- $\delta_{DM}$ frozen between $a_{enter}$ and $a_{eq}$ due to the Meszaros effect
- Perturbations outside the horizon grow as $\delta_{DM}\propto D_{+}(a)\propto a^2$.
![[Pasted image 20251120153443.png]]

Recall
$$a_{enter}(\lambda_{com})\approx \begin{cases}
\left( \frac{\lambda_{com}}{\ell_{H_{eq}}} \right)a_{eq} & \lambda_{com}<\ell_{H_{eq}} \\
\left( \frac{\lambda_{com}}{\ell_{H_{eq}}} \right)^2a_{eq} & \lambda_{com}>\ell_{H_{eq}}
\end{cases}.\tag{20.4} $$With $k=\frac{2\pi}{\lambda_{com}}$, we can rewrite this as
$$a_{enter}(k)\approx \begin{cases}
\left( \frac{k_{eq}}{k} \right)a_{eq} & k>k_{eq} & a_{enter}<a_{eq} \\
\left( \frac{k_{eq}}{k} \right)^2a_{eq} & k<k_{eq} & a_{enter}>a_{eq}
\end{cases}\tag{20.5} $$
where $k_{eq}$ is the wavenumber entering the horizon at matter-radiation equality, $k_{eq}=\frac{2\pi}{\ell_{H_{eq}}}$.

For cold dark matter, there is no free streaming so there are 2 cases:
- $a_{enter}(k)<a_{eq}(k>k_{eq})$
The Meszaros effect implies the growth factor is supressed by a factor
$$T(k)=\left( \frac{a_{enter}(k)}{a_{eq}} \right)^2=\left( \frac{k_{eq}}{k} \right)^2\tag{20.6}$$where the RHS comes from $a_{enter}(k)=\left( \frac{k_{eq}}{k} \right)a_{eq}$.
- $a_{enter}(k)>a_{eq}(k<k_{eq})$:
$\delta_{DM}\propto D_{+}(a)$ before and after horizon entry so $T(k)=1$.
This gives for cold dark matter,
$$T(k)\approx\begin{cases}
1 & k\lesssim k_{eq} \\
\left( \frac{k_{eq}}{k} \right)^2 & k\gtrsim k_{eq}
\end{cases}.\tag{20.7} $$
For warm dark matter and hot dark matter, we need to include the effect of free-streaming. Free streaming erases all dark matter perturbations with
$$\lambda_{com}=\frac{2\pi}{k}\lesssim \ell_{FS}\tag{20.8} .$$
Perturbations with $\lambda_{com}\gtrsim \ell_{FS}$ which enter the horizon at $a<a_{eq}$ still subject to the Meszaros effect, as for cold dark matter. Thus the transfer function is modified to become
$$T(k)\approx \begin{cases}
1 & k\lesssim k_{eq} \\
\left( \frac{k_{eq}}{k} \right)^2 & k_{eq}\lesssim k \lesssim \frac{2\pi}{\ell_{FS}} \\
0 & k\gtrsim \frac{2\pi}{\ell_{FS}}
\end{cases}.\tag{20.9} $$
For warm dark matter, $\ell_{FS}\ll \ell_{H_{eq}}$. For hot dark matter, $\ell_{FS}\sim \ell_{H_{eq}}$, so the intermediate range of $k$ in which the Meszaros effect operates disappears.
