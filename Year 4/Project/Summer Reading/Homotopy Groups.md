The topology of the [vacuum manifold](Non-Abelian%20Gauge%20Theories.md) $\mathcal{M}$ determines the topological defects at a certain symmetry breaking. The relevant properties of the manifold can be studied using the nth homotopy group,
$$\tag{9.1} \pi_{n}(\mathcal{M}):S^{n}\to \mathcal{M}.$$
$\pi_{n}(\mathcal{M})$ classifies the number of distinct mappings from the n-dimensional sphere into the vacuum manifold. [[Cosmic Strings]] are defined by the first homotopy group $\pi_{1}(\mathcal{M})$. A non-trivial $\pi_{1}(\mathcal{M})$ suggests that $\mathcal{M}$ is not simply connected, which gives rise to cosmic strings.

![[Pasted image 20250726152044.png]]

Definitions
- Consider closed paths $f(t)$, $g(t)$ though $\mathcal{M}$ in the parameterisation $0\leq t\leq 1$ so $f(0)=f(1)=x$. These paths are homotopic at $x$ if we can continuously deform one into the other while keeping contact at $x$.
- All possible loops at $x$ can be subdivided into distinct homotopy classes $[g]$. This class defines any loop homotopic to $g$.

These homotopy groups can be used to describe strings, for example with $\mathcal{M}=S^{1}$. The presence of a string can be detected by encircling it with a closed loop $\gamma(t)$. The field values $\phi$ at points along $\gamma(t)$ take values in $\mathcal{M}$, and so they map points from physical space $\mathbb{R}^{3}$ into the vacuum manifold $\mathcal{M}$. Hence, $\phi$ completes a mapping from $S^{1}$ to the path $g(t)$ in $\mathcal{M}$, $g(t)=\phi(\gamma(t))$. If $g(t)$ possesses a non-trivial winding $n$ in $\mathcal{M}$ then a string must be present in physical space, but this is exactly the criterion for $g(t)$ to belong to the homotopy class $n$. This correspondence is one-to-one since each type of sting can be identified with a unique element of $\pi_{1}(S^{1})\cong \mathbb{Z}$. For abelian $\pi_{1}(\mathcal{M})$, the string solutions can be classified by the homotopy group elements.
For a non-abelian example, consider the figure of eight space
![[Pasted image 20250726194007.png]]

As shown, $f,g$ are not homotopic at $x$ since they cannot be deformed into each other, so they fall into different homotopy classes in the fundamental group even though they show the same topological defect - a string resulting from a winding about the second void in $\mathcal{M}$.

The two loops identify topologically equivalent, it needs to be determined whether there is any continuous deformation between them, irrespective of the base-point restriction. If this is the case, the loops are freely homotopic, which defines a subdivision of the elements of $\pi_{1}(\mathcal{M})$ known as conjugacy classes. The two loops are conjugate if
$$\tag{9.2} cfc^{-1}\sim g$$
where $\sim$ signifies homotopic at $x$. This is illustrated by the loop $c$ which 'releases' $f$ from $x$ and it takes it around the opposite side of the topological obstruction. $c$ corresponds to an automorphism on $\pi_{1}(\mathcal{M})$, because it is an isomorphism of the group onto itself.

Theorem: Let $G$ be a connected and simply-connected Lie group, having a subgroup $H$ with a component $H_{0}$ connected to the identity. The quotient group $\pi_{0}(H)\equiv H/H_{0}$, labelling the disconnected components of $H$, is then isomorphic to the fundamental group of the coset space $\pi_{1}(G/H)$, that is
$$\pi_{1}(G/H)\cong \pi_{0}(H)\tag{9.3} .$$
The existence of string solutions reduces from the complicated procedure of characterising the topology of the vacuum manifold $\mathcal{M}$ to a simply question of whether the unbroken symmetry group $H$ is connected.