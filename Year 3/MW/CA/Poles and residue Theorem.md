If $f$ has a [simple pole](Poles%20and%20Zeros.md) at $z=z_{0}$ which lies in the region bounded by $C$ then
$$\oint_{C}f(z)dz=2\pi i\lim_{ z \to z_{0}}(z-z_{0})f(z_{0}) .$$
This theorem is particularly useful as it converts an integral, which can be difficult to solve, to a limit, which is easier to evaluate.

Example:
$$\oint_{C} \frac{dz}{z(z-1)}\;C:z=2e^{i\theta}$$
Poles at $z=0,1$
Using partial fractions
$$\frac{1}{z(z-1)}=\frac{1}{z-1}-\frac{1}{z}$$
so
$$\oint_{C} \frac{1}{z-1}-\frac{1}{z}dz=2\pi i\left[ -\lim_{ z \to 0 }(z-0)\left(-\frac{1}{z} \right) +\lim_{ z \to 1 } (z-1)\left( \frac{1}{z-1} \right) \right]=0$$
Example:
$$\oint_{C} \frac{e^{2z}}{z^2-4}dz=\oint \frac{e^{2z}}{(z+2)(z-2)}dz\;C:z={3e^{i\theta}}.$$
Poles at $z=\pm{2}$
$$\oint_{C} \frac{e^{2z}}{z^2-4}dz=2\pi i\left[ \lim_{ z \to -2 }(z+2) \frac{e^{2z}}{(z+2)(z-2)}+\lim_{ z \to 2 } (z-2) \frac{e^{2z}}{(z+2)(z-2)}  \right]$$
$$=2\pi i\left[ \frac{{e^4-e^{-4}}}{4} \right]=\pi i\sinh(4).$$
