Symmetries arise when the laws of physics stay the same under a symmetry transformation - magnitudes are conserved. 
There are two main types of symmetries
1. Continuous (like rotation of circle) - e.g. angular momentum
2. Discrete (like rotation of square) - e.g. [[Selection Rules]], parity.

Parity describes space inversion, $\underline{x}\to -\underline{x}$.
We can show space inversion by defining a parity operator:
$$\hat{P}\underline{x}=-\underline{x}.$$
We can easily see that $\hat{P}\hat{P}=\mathbb{I}$. We can use this to find the eigenvalues of $\hat{P}$. Let $\ket{u}$ be an eigenstate of $\hat{P}$ with eigenvalue $C$:
$$\hat{P}\hat{P}\ket{u}=\hat{P}(C\ket{u} )=C^2\ket{u}=\ket{u}  $$
$$\implies C^2=1\implies C=\pm 1.$$
The parity operator acts on a wavefunction as
$$\hat{P}\psi(\underline{x})=(-1)^{p_{int}}\psi(-\underline{x})$$where $p_{int}$ is the intrinsic parity, for all particles this can be set to $(-1)^{p_{int}}=1$.
We can write $\psi(\underline{x})$ as a combination of even and odd functions
$$\psi(\underline{x})=\frac{{\psi(\underline{x})+\psi(-\underline{x})}}{2}+\frac{{\psi(\underline{x})-\psi(-\underline{x})}}{2}$$
The first term will be called $\psi_{+}$ and the second term $\psi_{-}$. Applying the parity operator gives
$$\hat{P}\psi_{+}=\psi_{+}$$
$$\hat{P}\psi_{-}=-\psi_{-}.$$
If parity is conserved then $[\hat{P},\hat{H}]=0$ so a parity eigenstate will remain an eigenstate of the Hamiltonian.