Current density is the charge flowing per unit area per unit time.
$$J=nqv$$
where $n$ us the number density of charges, $q$ is the charge and $v$ is the velocity.

For a real system, $\underline{J}\neq 0$, $\sum \underline{v}=\underline{0}\implies \sum \underline{k}=\underline{0}$.

Consider the [bands](Band%20Gaps%20in%20Semiconductors.md) in a semiconductor,
![[Pasted image 20250213113425.png]]
The group velocity is given by
$$v_{g}=\frac{1}{\hbar} \frac{dE}{dk}.$$
Looking at $T=0\text{ K}$, considering the gradient of a $k$ point, the gradient at $-k$ is equal and opposite
$$\therefore \sum \underline{k}=\underline{0},\;\sum \underline{v}=\underline{0}.$$
The same reasoning can be given for $T>0\text{ K}$, so $\sum \underline{k}=\sum \underline{v}=\underline{0}$.
This implies there is no current at any given temperature for zero E-field.

For a non-zero E-field, consider a completely filled band,
![[Pasted image 20250213114235.png]]
Applying an E-field in the positive $k$ direction gives a force in the negative $k$ direction, due to electrons having a negative charge.
$$\underline{F}=\hbar \frac{d\underline{k}}{dt}\parallel -\underline{k}$$
$\implies \underline{k}$ is decreasing in time.
Consider a time $\Delta t$ later,
![[Pasted image 20250213114729.png]]
The far left electron moves outside the Brillouin zone, which in the reduced zone scheme moves to the far right position due to the periodic nature of crystals. This leaves the same configuration,
$$\sum \underline{k}=\sum \underline{v}=\underline{0}$$
so under an E-field a full band does not carry a current so the semiconductor is insulating at $T=0\text{ K}$.

Consider a nearly empty band under an E-field, like the conduction band at $T>0\text{ K}$.
![[Pasted image 20250213115355.png]]
Here $\sum \underline{k}=\sum \underline{v}=\underline{0}$.
At some later time $\Delta t$.
![[Pasted image 20250213115524.png]]
Each electron has shifted one place. All still within the Brillouin zone so no need to reduce. Here $\sum \underline{k}\neq 0\implies \sum \underline{v}\neq 0$ so there is an instantaneous current.

Considering the group velocity,
![[Pasted image 20250213122718.png]]
Over time, each electron samples each $k$ point, and as $v_{g}$ is anti-symmetric, integrated over time gives $\langle v_{g} \rangle=0\therefore \langle J \rangle=0\implies$ there is no net current over an extended period of time.
This is not the full picture.
