The [Higgs field](Electroweak%20Symmetry%20Breaking.md) is an $SU(2)$ doublet,
$$H=\begin{bmatrix}
H^+ \\
H^0
\end{bmatrix}=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
\phi_{1}+i\phi_{2} \\
\phi_{3}+i\phi_{4}
\end{bmatrix}\tag{10.1} $$
The charge of the components is given by
$$Q=T_{3}+Y\tag{10.2} $$
The potential is
$$V(H)=-\mu^2H^{\dagger}H+\lambda(H^{\dagger}H)^2\tag{10.3} $$
The $\phi_{i}$ real scalar fields can be rotated by $SU(2)\times U(1)$ so we can use gauge freedom to align the fields, we will take the alignment along $\phi_{3}$.
The Higgs field is a fluctuation around the VEV,
$$H=\frac{1}{\sqrt{ 2 }}\begin{bmatrix}
0 \\
v+h
\end{bmatrix}\tag{10.4} $$
which gives the potential
$$V(H)=-\frac{\mu^2}{2}(v+h)^2+\frac{\lambda}{4}(v+h)^3=-\mu^2vh-\frac{\mu^2}{2}h^2+\frac{\lambda}{4}(4v^3h+6v^2h^2+4vh^3+h^4)\tag{10.5} .$$
Using $v^2=\frac{\mu^2}{\lambda}$, the linear terms cancel so
$$V(H)=-\mu^2h^2+\lambda vh^3+\frac{1}{4}h^4\tag{10.6}. $$
The Higgs coupling to matter fields is given by
$$\mathcal{L}_{M}=\left( \frac{gv}{2} \right)^2W_{\mu}^{+}W^{-\mu}+\frac{1}{2}\left( \frac{gv}{2c_{w}} \right)^2Z_{\mu}Z^{\mu}+\sum_{\psi}y_{\psi} \frac{v}{\sqrt{ 2 }}\bar{\psi}\psi \tag{10.7} $$
and as $v\to v+h$,
$$\mathcal{L}_{hXX}=g{M_{W}}hW_{\mu}^{+}W^{-\mu}+\frac{g}{2c_{w}}M_{Z}Z_{\mu}Z^{\mu}+\sum_{\psi} \frac{y_{\psi}}{\sqrt{ 2 }}h\bar{\psi}\psi \tag{10.8}. $$
These gives the tree-level Feynman diagrams
![[Pasted image 20260309112305.png]]
For Higgs production in the LHC, we have a few scenarios
![[Pasted image 20260309112334.png]]
To find the dominant production mechanism, focus on the particles which couple to the Higgs, and take the loop suppression to be of order $\frac{g^2}{16\pi^2}$.

Higgs emission from fermions, $d\bar{d}\to h$:
![[Pasted image 20260309112531.png]]
The cross section is
$$\sigma=\int_{0}^{1}dx_{1}\int_{0}^{1}dx_{2}f_{d}(x_{1})f_{\bar{d}}(x_{2})\underbrace{ \hat{\sigma}_{d\bar{d}\to h}(x_{1}x_{2}s) }_{ \sim \left( \frac{m_{d}}{v} \right)^2\delta(x_{1}x_{2}s-m_{h}^2) }\tag{10.9} $$
This gives
$$\sigma\sim \left( \frac{m_{d}}{v} \right)^2 \frac{1}{s}L_{d\bar{d}}\tag{10.10} $$
where
$$L_{d\bar{d}}=s \int_{0}^{1}dx_{1}\int_{0}^{1}dx_{2}f_{d}(x_{1})f_{\bar{d}}(x_{2})\delta(x_{1}x_{2}s-m_{h}^2)=\int_{0}^{1}f_{d}(x_{1})f_{\bar{d}}\left( \frac{m_{h}^2}{x_{1}s} \right)\tag{10.11}. $$
As $\left( \frac{m_{d}}{v} \right)^2=\left( \frac{5\text{ MeV}}{174\text{ GeV}} \right)\sim \mathcal{O}(10^{-10})$, so this production mechanism is negligible.

Another mechanism is from gluons,
![[Pasted image 20260309113903.png]]
For the first mechanism, the cross-section is
$$\sigma\sim \frac{1}{m_{h}^2}\alpha_{s}^2y_{t}^2 \frac{1}{16\pi^2}L_{gg}\tag{10.12} $$
which is not small even with the loop.

For the second mechanism, the cross-section is
$$\sigma\sim \frac{1}{(m_{h}+2m_{t})^2}\alpha_{s}y_{t}^2 \frac{1}{16\pi^2}L_{gg}\tag{10.13}. $$
This is smaller so doesn't contribute as much to Higgs production.

Alternative mechanisms are Higgsstrahlang,
![[Pasted image 20260309114404.png]]
with cross-section
$$\sigma\sim \frac{1}{(m_{h}+m_{v})^2}g^4L_{q\bar{q}}\tag{10.14} $$
and vector boson fusion
![[Pasted image 20260309114455.png]]
with cross section
$$\sigma\sim \frac{1}{(m_{h}+m_{v})^2}g^4L_{q\bar{q}}\tag{10.15}.$$
The Higgs can also decay, although given that $2m_{t}, 2m_{W}, 2m_{Z}>m_{h}$, the decay in to top quarks or W/Z bosons are kinematically forbidden.

The Higgs can decay to bottomonium,
![[Pasted image 20260309114656.png]]
with decay width
$$\Gamma\sim \frac{3y_{b}^2m_{h}}{8\pi}\tag{10.16} .$$
This produces jets which so this is difficult to detect.

Higgs can also produce weak bosons,
![[Pasted image 20260309114810.png]]
with decay width
$$\Gamma \sim \frac{1}{256\pi^2}g^2(g^2M_{W}^2) \frac{1}{M_{W}^4}M_{h}^5\tag{10.17}. $$
For gluon production,
![[Pasted image 20260309114923.png]]
with decay width
$$\Gamma \sim m_{h}\alpha_{s}y_{t}^2 \frac{1}{16\pi^2} \frac{1}{8\pi}\tag{10.18}. $$
For photon production,
![[Pasted image 20260309115011.png]]
and lepton production
![[Pasted image 20260309115024.png]]
