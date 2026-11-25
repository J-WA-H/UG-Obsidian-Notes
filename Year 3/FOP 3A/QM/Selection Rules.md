As shown before in an [EM-field](Electrons%20In%20Atoms%20in%20an%20EM%20field.md) defined by $\underline{E}=\underline{E}_{0}\cos(\omega t)$ gives the Hamiltonian
$$\hat{H}(\underline{r},t)=-q(\underline{r}\cdot \underline{E}_{0})\cos(\omega t).$$
In the dipole approximation, $E_{0x}$, $E_{0y}$, $E_{0z}$ are independent of space.
$$(p)_{ab}=\bra{\psi_{a}}q\underline{r}\ket{\psi_{b}} =\bra{\psi_{a}}qx\ket{\psi_{b}}\underline{\hat{x}}+\bra{\psi_{a}}qy\ket{\psi_{b}}\underline{\hat{y}}+\bra{\psi_{a}}qz\ket{\psi_{b}}\underline{\hat{z}}.$$
Say $\ket{\psi_{a}}=\ket{\psi_{nlm}}=\ket{nlm}$, $\ket{\psi_{b}}=\ket{\psi_{n'l'm'}}=\ket{n'l'm'}$.
We aim to investigate what transitions between these states are allowed, i.e. find the restrictions on the quantum numbers where $\bra{n'l'm'}\underline{r}\ket{nlm}\neq 0$.
Recall $[\hat{L}_{z},\hat{z}]=0$, $\hat{L}_{z}\ket{nlm}=m\hbar \ket{nlm}$.
Proof for matrix element z: $\bra{n'l'm'}[\hat{L}_{z},\hat{z}]\ket{nlm}=0$.
$$\bra{n'l'm'}\hat{L}_{z}z\ket{nlm}-\bra{n'l'm'}z\hat{L}_{z}\ket{nlm}=0$$
$$m'\hbar \bra{n'l'm'}z\ket{nlm}-m\hbar \bra{n'l'm'}z\ket{nlm}=0$$
$$(m'-m)\hbar \bra{n'l'm'}z\ket{nlm}=0$$
so for $m'\neq m$, $\bra{n'l'm'}z\ket{nlm}=0$ so no transition allowed.
In x,y:
$$[\hat{L}_{z},\hat{x}]=i\hbar \hat{y}$$
$$[\hat{L}_{z},\hat{y}]=-i\hbar \hat{x}$$
$$[\hat{L}_{z},\hat{x}+i\hat{y}]=\hbar(\hat{x}+i\hat{y}).$$
$$\bra{n'l'm'}[\hat{L}_{z},\hat{x}+i\hat{y}]\ket{nlm}=\hbar \bra{n'l'm'}x+iy\ket{nlm}$$
$$\bra{n'l'm'}\hat{L}_{z}(x+iy)\ket{nlm}-\bra{n'l'm'}(x+iy)\hat{L}_{z}\ket{nlm}$$
$$=m'\hbar \bra{n'l'm'}x+iy\ket{nlm}-m\hbar \bra{n'l'm'}x+iy\ket{nlm}=\hbar \bra{n'l'm'}x+iy\ket{nlm}$$
$$\implies(m'-m-1)\hbar \bra{n'l'm'}x+iy\ket{nlm}=0$$
so for $m'\neq m+1$, $\bra{n'l'm'}x+iy\ket{nlm}=0$ so no transition occurs. 

Using the same method for $x-iy$, we get that no transitions occur when $m'\neq m-1$.

This gives the selection rules for $m$, which state that transitions between states only occur when
$$\Delta m=0,\pm 1$$
The selection rules for $l$ are
$$\Delta l=\pm 1.$$
![[Pasted image 20241108195511.png]]
The figure shows the allowed transitions between states in the atom. Here we can see why the transition between the $2P\to 1S$ states has a smaller energy than the $2S\to 1S$ transition as for the latter, it involves the transition from $2S\to 3P$ then from $3P\to1S$, when $2P$ can move directly to $1S$. 