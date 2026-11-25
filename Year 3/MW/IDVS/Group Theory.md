Linear maps of a vector space into itself defines [[Linear Operators]], the corresponding matrices for these operators for a given basis.

These operations have the structure of groups.

A group $G$ is defined as a set of elements equipped with an operation $*$ which assigns for every ordered pair of elements $f,g\in G$, another element of the set, $h\in G$
$$h=f*g.$$
The operation for the group might be known as the product/combination/multiplication which has to be defined for each group.

We write the elements of a group as a set $G=\{ G_{1},G_{2},\dots \}$.

Properties of groups:
1. If $f,g\in G$ then $h=f*g\in G$
2. For any $f,g,h\in G$, $f*(g*h)=(f*g)*h$ (associativity).
3. There is a unique identity element $e\in G$ s.t. $f*e=e*f=f$.
4. $\forall\;f\in G\;\exists\;f^{-1}\in G$ s.t. $f*f^{-1}=f^{-1}*f=e$.

For groups where the order of multiplication doesn't matter, they are known as abelian groups:
$$f*g=g*f.$$
Most groups are not abelian.

The number of elements in the group is the order of the group.

Multiplication tables are useful to show how the given operation acts on an ordered pair in the group.
Consider the group $G=\{ e,f_{1},f_{2} \}$, then its multiplication table is given by
![[Pasted image 20241123123541.png]]
After multiplication each row/column has all elements and only one of each.

The representation of a group is a mapping, $D$, of the elements of $G$ onto a set of linear operators that act on some vector space. The mapping isn't unique between group elements of linear operators but it must satisfy:
1. $D(e)=1$ for the identity operator
2. Group multiplication law, $*$, must be mapped onto the multiplication of the objects in the representation
	$$D(g_{1})D(g_{2})=D(g_{1}*g_{2}).$$
The simplest example of a group is $Z_{2}$, which contains two elements, $Z_{2}=(e,-e)$.

The important examples of groups are for [[Unitary and Orthogonal Operators]], $U(n),SU(n),O(n),SO(n)$.