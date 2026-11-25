Definition: An [analytic](Complex%20Differentiation.md) function $f(z)$ has a zero at point $z_0$ if we can write $f(z)=(z-z_{0})g(z)$, where $g$ is analytic on the same domain as $f$.

Definition: If $f(z)=(z-z_{0})^ng(z)$ and $f,g$ are analytic on domain $D$ and $g(z_0)\neq 0$ then $f(z_0)$ has a multiplicity of $n$.

Example:
$$f(z)=\frac{{z+1}}{z^2(z^2+1)}$$
has a zero at the point $z_{0}=-1$.
$$f(z)=(z-i)^2$$
has zero at $z_{0}=i$ with multiplicity of $2$.

Definition: Let $f$ be analytic on domain $D/\{z_{0}\}$. Then $f$ has a pole at $z=z_{0}$ if $$f(z)=\frac{g(z)}{(z-z_{0})^m}$$where $g$ is analytic in all of $D$. 
The pole at $z=z_{0}$ has order $m$.
A pole of order 1 is known as a simple pole.

Example:
$$f(z)=\frac{{z+1}}{z^3(z^2+1)}=\frac{{z+1}}{z^3(z+i)(z-i)}.$$
$f$ has two simple poles at $z=\pm i$ and a pole of order $3$ at $z=0$.