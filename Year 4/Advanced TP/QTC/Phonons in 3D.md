The theory of [[Phonons]] can be extended to three dimensions. Consider $N$ atoms in the simplest type of crystal - the Bravais lattice.

In a Bravais lattice, the vector distance $\vec{\ell}$ between two atoms is
$$\vec{\ell}=n_{1}\vec{\ell}_{1}+n_{2}\vec{\ell}_{2}+n_{3}\vec{\ell}_{3}\tag{17.1} $$
where $\vec{\ell}_{i}$ are the lattice basis vectors and $n_{i}\in \mathbb{Z}$.

There are $N$ independent Bravais lattice vectors $\vec{\ell}$. It is convenient to define the reciprocal lattice from the set of lattice vectors $\vec{g}$ which satisfy
$$e^{ i\vec{g}\cdot \vec{\ell} }=1\;\forall\;\vec{\ell}\tag{17.2} .$$
A useful property for a vector $\vec{q}$ in reciprocal space is that $\sum_{\ell}e^{ i\vec{q}\cdot \vec{\ell}}=0$ unless $\vec{q}$ is one of the reciprocal lattice vectors $\vec{g}$ so $\sum_{\ell}e^{ i\vec{q}\cdot \vec{\ell} }=N$. We can then write
$$\sum_{\vec{\ell}}e^{ i\vec{q}\cdot \vec{\ell} }=N\Delta(\vec{q})\tag{17.3}\qquad \Delta(\vec{q})=\sum_{\vec{g}}\delta_{\vec{q}\vec{g}}. $$
The Hamiltonian of a lattice of atoms of mass $m$ at positions $\vec{\ell}$ is, with $(i,j=x,y,z)$
$$H=\frac{1}{2m}\sum_{\ell}\sum_{i=1}^{3}(p^i)^2+\frac{1}{2}\sum_{\vec{\ell},\vec{\ell}'}\sum_{i,j=1}^{3}y_{\vec{\ell}}^{i}V_{\vec{\ell}\vec{\ell}'}^{ij}y_{\vec{\ell}'}^{j}+\mathcal{O}(y^3)\tag{17.4} $$
In the harmonic approximation, we keep up to second order terms in the potential energy. The potential tensor $V_{\ell \vec{\ell}'}^{ij}$ is given by
$$V_{\vec{\ell} \vec{\ell}'}=\frac{\partial^2V}{\partial y_{\vec{\ell}}^i\partial y_{\vec{\ell}'}^j}\tag{17.5} $$
We can rewrite the Hamiltonian as
$$H=\frac{1}{2m}\sum_{\vec{\ell}}\begin{bmatrix}
p_{\vec{\ell}}^{x} & p_{\vec{\ell}}^y & p_{\vec{\ell}}^z
\end{bmatrix} \begin{bmatrix}
p_{\vec{\ell}}^x \\
p_{\vec{\ell}}^y \\
p_{\vec{\ell}}^z
\end{bmatrix}+\frac{1}{2}\sum_{\vec{\ell},\vec{\ell}'}\begin{bmatrix}
y_{\vec{\ell}}^x & y_{\vec{\ell}}^y & y_{\vec{\ell}}^z
\end{bmatrix} \begin{bmatrix}
V_{\vec{\ell}\vec{\ell}'}^{xx} & V_{\vec{\ell}\vec{\ell}'}^{xy} & V_{\vec{\ell}\vec{\ell}'}^{xz} \\
V_{\vec{\ell}\vec{\ell}'}^{yx} & V_{\vec{\ell}\vec{\ell}'}^{yy} & V_{\vec{\ell}\vec{\ell}'}^{yz} \\
V_{\vec{\ell}\vec{\ell}'}^{zx} & V_{\vec{\ell}\vec{\ell}'}^{zy} & V_{\vec{\ell}\vec{\ell}'}^{zz}
\end{bmatrix}\begin{bmatrix}
y_{\vec{\ell}'}^x \\
y_{\vec{\ell}'}^{y} \\
y_{\vec{\ell}'}^{z}
\end{bmatrix}\tag{17.6} $$
The row and column vectors have $3N$ dimensions, and the Hessian matrix is $3N\times 3N$.

The collective coordinates are defined as in the 1D case,
$$\vec{Y}_{\vec{q}}^{i}=\frac{1}{\sqrt{ N }}\sum_{\vec{\ell}}e^{ -i\vec{q}\cdot \vec{\ell} }\vec{y}_{\vec{\ell}}, \qquad \vec{P}_{\vec{q}}=\frac{1}{\sqrt{ N }}\sum_{\vec{\ell}}e^{ i\vec{q}\cdot \vec{\ell} }\vec{p}_{\vec{\ell}}\tag{17.7}. $$
These are periodic, $\vec{Y}_{\vec{q}+\vec{g}}=\vec{Y}_{\vec{q}}$, $\vec{P}_{\vec{q}+\vec{g}}=\vec{P}_{\vec{q}}$. It is convenient to consider these $N$ wavevectors with the smallest $|\vec{q}|$. We say that we take $\vec{q}$ in the first Brillouin zone. The inverse transformations are
$$\vec{y}_{\vec{\ell}}^{i}=\frac{1}{\sqrt{ N }}\sum_{\vec{q}}e^{ i\vec{q}\cdot \vec{\ell} }\vec{Y}_{\vec{q}}^{i},\qquad\vec{p}_{\vec{\ell}}=\frac{1}{\sqrt{ N }}\sum_{\vec{q}}e^{ -i\vec{q}\cdot \vec{\ell} }\vec{P}_{\vec{q}}\tag{17.8}. $$
When this is substitute into the Hamiltonian and become almost diagonal, where the double $\vec{\ell},\vec{\ell}'$ becomes a sum over just $\vec{q}$.
$$H=\sum_{\vec{q}}\left( \frac{1}{2m}\begin{bmatrix}
P_{\vec{q}}^{x\dagger} & P^{y\dagger}_{\vec{q}} & P^{z\dagger}_{\vec{q}}
\end{bmatrix}\begin{bmatrix}
P_{\vec{q}}^{x} \\
P_{\vec{q}}^{y} \\
P_{\vec{q}}^{z}
\end{bmatrix} +\frac{1}{2}\begin{bmatrix}
Y_{\vec{q}}^{x\dagger} & Y_{\vec{q}}^{y\dagger} & Y_{\vec{q}}^{z\dagger}
\end{bmatrix}\begin{bmatrix}
V_{\vec{\ell}\vec{\ell}'}^{xx} & V_{\vec{\ell}\vec{\ell}'}^{xy} & V_{\vec{\ell}\vec{\ell}'}^{xz} \\
V_{\vec{\ell}\vec{\ell}'}^{yx} & V_{\vec{\ell}\vec{\ell}'}^{yy} & V_{\vec{\ell}\vec{\ell}'}^{yz} \\
V_{\vec{\ell}\vec{\ell}'}^{zx} & V_{\vec{\ell}\vec{\ell}'}^{zy} & V_{\vec{\ell}\vec{\ell}'}^{zz}
\end{bmatrix}\begin{bmatrix}
Y_{\vec{q}}^{x} \\
Y_{\vec{q}}^{y} \\
Y_{\vec{q}}^{z}
\end{bmatrix}\right)\tag{17.9} $$
with $V_{\vec{q}}^{ij}=\sum_{\vec{\ell}'}e^{ i\vec{q}\cdot(\vec{\ell}-\vec{\ell}') }V_{\vec{\ell} \vec{\ell}'}^{ij}$.

To diagonalise the Hessian matrix, rotate the coordinate system, with unit eigenvectors $\vec{s}_{1}(\vec{q}),\vec{s}_{2}(\vec{q}),\vec{s}_{3}(\vec{q})$. These are the polarisation direction of the phonons. In this coordinate system, the Hamiltonian is fully diagonal,
$$H=\sum_{\vec{q}}\sum_{\vec{s}=\vec{s}_{1}(\vec{q})}^{\vec{s}_{3}(\vec{q})}\left( \frac{1}{2m}(P_{\vec{q}}^{s})^{\dagger}+\frac{1}{2}V_{q}^{s}(Y_{q}^{s})^{\dagger}Y_{q}^{s} \right)\tag{17.10}. $$
The frequency of these phonons are
$$\omega_{\vec{q}s}=\sqrt{ \frac{V_{q}^{s}}{m} }\tag{17.11}. $$
If one of the $\vec{s}$ vectors happens to be parallel to $\vec{q}$, we have longitudinally polarised phonons in the crystal and we also have transversely polarised phonons.

We can define creation and annihilation operators
$$A_{\vec{q}s}=\frac{1}{\sqrt{ 2m\hbar \omega_{\vec{q}s} }}(m\omega_{\vec{q}s}\vec{Y}_{\vec{q}s} +i\vec{P}_{\vec{q}s}^{\dagger})\cdot \vec{s}(\vec{q}),\qquad A_{\vec{q}s}^{\dagger}=\frac{1}{\sqrt{ 2m\hbar \omega_{\vec{q}s} }}(m\omega_{\vec{q}s} \vec{Y}_{\vec{q}s}^{\dagger}-i\vec{P}_{\vec{q}s})\cdot \vec{s}(\vec{q})\tag{17.12} $$
which gives the Hamiltonian
$$H=\sum_{\vec{q}}\sum_{\vec{s}=\vec{s}_{1}(\vec{q})}^{\vec{s}_{3}(\vec{q})}\left( A_{\vec{q}s}^{\dagger}A_{\vec{q}s}+\frac{1}{2} \right)\hbar \omega_{\vec{q}s}\tag{17.13}.$$
Not all lattices are Bravais. In a lattice with a basis where $\vec{\ell}$ does not define equilibrium positions of the atoms but positions of groups of atoms. The equilibrium position is $\vec{\ell}+\vec{b}$, where $\vec{b}$ is a vector giving the position of an atom inside the group. There are many different types of atoms in a group, each with mass $m_{\vec{b}}$. The Harmonic Hamiltonian then takes the form
$$H=\sum_{\vec{\ell},\vec{b}}\sum_{\ell=1}^{3} \frac{1}{2m_{\vec{b}}}(p_{\vec{\ell}\vec{b}}^i)^2+\frac{1}{2}\sum_{\vec{\ell},\vec{b},\vec{\ell}',\vec{b}'}\sum_{i,j=1}^{3}y_{\vec{\ell}\vec{b}}^iV_{\vec{\ell}\vec{b}\vec{\ell}'\vec{b}'}^{ij}y_{\vec{\ell}'\vec{b}'}^{i}\tag{17.14}. $$
We regard this basis as a set of $n_{b}$ interlocked Bravais lattices.

We can write that 
$$\vec{Y}_{\vec{q}\vec{b}}=\frac{1}{\sqrt{ N }}\sum_{\vec{\ell}}e^{ -i\vec{q}\cdot \vec{\ell} }\vec{y}_{\vec{\ell}\vec{b}}\tag{17.15},\qquad \vec{P}_{\vec{q}\vec{b}}=\frac{1}{\sqrt{ N }}\sum_{\vec{\ell}}e^{ i\vec{q}\cdot \vec{\ell} } \vec{p}_{\vec{\ell}\vec{b}},\qquad V_{\vec{q}\vec{b}\vec{b}'}^{ij}=\sum_{\vec{\ell}'}e^{ i\vec{q}\cdot(\vec{\ell}-\vec{\ell}') }V^{ij}_{\vec{\ell}\vec{b}\vec{\ell}'\vec{b}'}.$$
The Hamiltonian reduces to
$$H=\sum_{\vec{q},\vec{b}}\left( \frac{1}{2m}\begin{bmatrix}
P_{\vec{q}\vec{b}}^{x\dagger} & P^{y\dagger}_{\vec{q}\vec{b}} & P^{z\dagger}_{\vec{q}\vec{b}}
\end{bmatrix}\begin{bmatrix}
P_{\vec{q}\vec{b}}^{x} \\
P_{\vec{q}\vec{b}}^{y} \\
P_{\vec{q}\vec{b}}^{z}
\end{bmatrix} +\frac{1}{2}\begin{bmatrix}
Y_{\vec{q}\vec{b}}^{x\dagger} & Y_{\vec{q}\vec{b}}^{y\dagger} & Y_{\vec{q}\vec{b}}^{z\dagger}
\end{bmatrix}\begin{bmatrix}
V_{\vec{q}\vec{b}\vec{b};}^{xx} & V_{\vec{q}\vec{b}\vec{b}'}^{xy} & V_{\vec{q}\vec{b}\vec{b}'}^{xz} \\
V_{\vec{q}\vec{b}\vec{b}'}^{yx} & V_{\vec{q}\vec{b}\vec{b}'}^{yy} & V_{\vec{q}\vec{b}\vec{b}'}^{yz} \\
V_{\vec{q}\vec{b}\vec{b}'}^{zx} & V_{\vec{q}\vec{b}\vec{b}'}^{zy} & V_{\vec{q}\vec{b}\vec{b}'}^{zz}
\end{bmatrix}\begin{bmatrix}
Y_{\vec{q}\vec{b}}^{x} \\
Y_{\vec{q}\vec{b}}^{y} \\
Y_{\vec{q}\vec{b}}^{z}
\end{bmatrix}\right)\tag{17.16}$$
We can no longer just rotate the coordinate system to diagonalise this. Instead, we must form a linear combination of the $Y_{qb}^{i}$ that will make $V_{qbb'}^{ij}$ diagonal in $\vec{b}$. We find that for each $\vec{q}$ there are $3n_{b}$ distinct modes of vibrations.

The polarisation directions of these modes are in general ill defined since the $n_{b}$ atoms that form the basis group may be moving in quite different directions. Only the collective coordinates formed by the linear combination of $Y_{qb}^{i}$ has a specific direction of vibration. The $3n_{b}$ different modes we find form the various branches of the phonon spectrum of the crystal. The lowest frequencies of vibrations will be found in the three modes in which all atoms within the basis move more in less in space.

For vanishingly small values of $\vec{q}$ these can be identified as the three modes of sound, with $\omega$ proportional to $|\vec{q}|$. These three modes form the acoustic branch of the phonon spectrum. In the other modes the atoms within the basis move to some extent out of phase, and $\omega$ tends to a nonzero value as $|\vec{q}|$ tends to zero. Because the frequencies of these phonons tend to be high enough to be excited by infrared radiation, they are said to lie in the optical branch of the phonon spectrum.
![[Pasted image 20260308130625.png]]
