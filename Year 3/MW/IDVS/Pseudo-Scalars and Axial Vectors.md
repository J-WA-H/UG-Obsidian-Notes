To consider different types of scalars and vectors, we need to consider two [[Rotations]], proper rotations, $R\in SO(n)$, and improper rotations, $P\in O(n)$, where $\det P=-1$.

- Scalars are invariant under rotation and reflection ($P$ acts as a reflection on scalars):
	- $$R:\phi\to \phi'=\phi$$
	- $$P:\phi\to \phi'=\phi$$
- Pseudoscalars are invariant under rotations but flip signs under reflection:
	- $$R:\rho\to \rho'=\rho$$
	- $$P:\rho\to \rho'=-\rho$$
- True vectors are tensors of rank 1 that under a reflection go to the negative of itself $\underline{v}\to-\underline{v}$:
	- $$R:v^{i}\to v'^{i}=R^{i}_{\;j}v^{j}$$
	- $$P: v^{i}\to v'^{i}=P^{i}_{\;j}v^{j}$$
- Axial vectors are invariant under reflection (e.g. angular momentum $\underline{L}$):
	- $$R:a^{i}\to a'^{i}=R^{i}_{\;j}a^{j}$$
	- $$P: a^{i}\to a'^{i}=P^{i}_{\;j}a^{j}.$$

