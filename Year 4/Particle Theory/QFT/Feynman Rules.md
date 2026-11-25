Consider the [interaction Lagrangian](Interacting%20Fields.md) $(7.4)$,
$$\mathcal{L}=\frac{1}{2}(\partial_{\mu}\phi)(\partial^{\mu}\phi)-\frac{1}{2}m^2\phi^2-\frac{\lambda}{4!}\phi^4\tag{10.1} .$$
From the interaction term, the interaction Hamiltonian is then
$$\mathcal{H}_{int}=-i \frac{\lambda}{4!}\phi^4\tag{10.2} .$$
The 4th [Greens function](Time%20Evolution.md) is given by the $S$ matrix,
$$G_{4}(x_{1},x_{2},x_{3},x_{4})=\bra{0} T\left( \hat{\phi}(x_{1})\hat{\phi}(x_{2})\hat{\phi}(x_{3})\hat{\phi}(x_{4})\exp \left[ -i \frac{\lambda}{4!}\int d^4y\;\hat{\phi}^4(y) \right] \right)\ket{0}.\tag{10.3}  $$
To evaluate the Greens function, expand the $S$-matrix as a Taylor series,
$$\exp\left[ -i \frac{\lambda}{4!}\int d^4y\;\hat{\phi}^4(y) \right]\approx 1-\frac{i\lambda}{4!}\int d^4y\;\hat{\phi}^4(y)+\frac{1}{2}\left( \frac{i\lambda}{4!} \right)^2\int d^4y\;\hat{\phi}^4(y)\int d^4z\;\hat{\phi}^4(z)+\mathcal{O}(\lambda^3).\tag{10.4} $$
Consider the $\mathcal{O}(\lambda^{0})$ term,
$$G_{4}(x_{1},x_{2},x_{3},x_{4})=\bra{0} T(\hat{\phi}(x_{1})\hat{\phi}(x_{2})\hat{\phi}(x_{3})\hat{\phi}(x_{4}))\ket{0}.\tag{10.5} $$
This can be drawn as Feynman diagrams which each $x_{i}$ point being a node, and each vertex being a propagator.
![[Pasted image 20251109150916.png]]
Given that each vertex is a propagator, these diagrams are equivalent to [(9.11)](Wick's%20Theorem.md), with the propagators linking to points in the same diagram multiplied by each other - for example in the first diagram, $x_{1},x_{2}$ are linked and $x_{3},x_{4}$ are linked so its contribution to the propagator is $G_F(x_{1}-x_{2})G_{F}(x_{3}-x_{4})$.

These are disconnected Feynman diagrams, as the two parts of the diagram are not connected. Particles linked by a propagator have the same momentum.
Only connected diagrams contribute to $G_{n}$ so $\mathcal{O}(\lambda^{0})$ makes no contribution since all possible Feynman diagrams are disconnected.

For $\mathcal{O}(\lambda^{1})$,
$$G_{4\,connected}^{(\lambda^{1})}=-\frac{i\lambda}{4!}\int d^4y\bra{0}T( \overbrace{\hat{\phi}(x_{1})\overbrace{\hat{\phi}(x_{2})\overbrace{\hat{\phi}(x_{3})\overbrace{\hat{\phi}(x_{4})\hat{\phi}^4(y)}}}})\ket{0} .\tag{10.6} $$
Each $x_{i}$ field couples to one of the four $\hat{\phi}(y)$ fields. There is only one connected diagram,
![[Pasted image 20251109152338.png]]
In terms of propagators this is
$$-i\lambda \int d^4y\;G_{F}(x_{1}-y)G_{F}(x_{2}-y)G_{F}(x_{3}-y)G_{F}(x_{4}-y)\tag{10.7}.$$
The extra factor of $4!$ to account for the number of ways to arrange the fields.

$y$ is an interaction vertex, since $y$ comes from the interaction. There are many other possible Feynman diagrams but they are all disconnected so they don't contribute to $G_{4}$,
![[Pasted image 20251109152758.png]]
For $\mathcal{O}(\lambda^2)$, there are two unique topologies that contribute to $G_{4}$,
![[Pasted image 20251109153116.png]]
![[Pasted image 20251109153126.png|206]]

They full Feynman rules are for the $\mathcal{O}(\lambda^{m})$ contribution to an $n$-point Greens function $G_{n}(x_{1},\dots,x_{n})$:
1. Draw all distinct diagrams with $n$ external lines and $m$ 4-point vertices:
	- Draw $n$ dots and label them $x_{1},\dots,x_{n}$ (external points)
	- Draw $m$ dots and label them $y_{1},\dots,y_{m}$ (vertices)
	- Join the dots according to the following rules:
		- Only one line emanates from each $x_{i}$
		- Exactly four lines run into each $y_{i}$
	- The resulting diagram must be connected, i.e. there must be a continuous path between any two points.
2. Assign a factor $-\frac{i\lambda}{4!}\int d^4y_{i}$ to the vertex at $y_{i}$
3. Assign a factor $G_{F}(x_{i}-y_{j})$ to the line joining $x_{i}$ and $y_{j}$
4. Multiply by the number of contractions $C$ from the Wick expansion which led to the same diagram.

These are Feynman rules in position space.