We have observational data for the rotation of planetary surfaces - but the top of the atmosphere rotates raster than the interior, as shown by the magnetic field.

The ellipticity of a planet - defined as how much the planet has flattened due to rotation, and is given by
$$f=\frac{R_{eq}-R_{pole}}{R_{eq}}.$$
Outside a rotating planet, the gravitational potential can be approximated well using a Legendre polynomial expansion:
$$U(r,\theta)=-\frac{GM_{p}}{r}\left[ 1-\sum_{n=2}^{\infty}\left( \frac{R_{p}}{r} \right)^nJ_{n}P_{n}(\cos \theta) \right].$$
Most planets are nearly spherical so the $J_{2}$ coefficients dwarfs higher order components so
$$U(r, \theta)=-\frac{GM}{r}\left[ 1-\left( \frac{R_{p}}{r} \right)^2J_{2}P_{2}(\cos \theta) \right]$$
where $P_{2}(\cos \theta)=(3\cos^2\theta-1)/2$.

These $J$ coefficients can be calculated using natural satellites in motion and by doppler tracking of spacecraft flying by.

Odd $n$ coefficients are small, but non-zero, and have been used to measure differential rotation caused by winds in the top few $1000\text{ km}$ of the atmospheres. Values of lower order moments suggest that the deeper planetary interiors are not entirely differentiated.

A self-gravitating spinning planet will be flattened to a degree that depends on the rotation rate and the interior mass distribution, which can be described using the moment of inertia factor for rotation about the polar axis
$$\alpha_{p}=\frac{I}{M_{p}R_{p}^2}.$$
This can be related to density by
$$\alpha_{p}=\frac{\int(r\sin \theta)^2dm}{M_{p}R_{p}^2}=\frac{\int(r\sin \theta)^2\rho d^3r}{M_{p}R_{p}^2}.$$
For a uniform density sphere $\alpha_{p}=0.4$, which may differ for more concentrated planets that have somewhat lower values.

In [[Hydrostatic Equilibrium]], a good approximation for $J_{2}$ and $\alpha_{p}$ are
$$J_{2}=\frac{2}{3}\left[ f-\frac{\Omega}{2} \right]$$
$$\alpha_{p}=\frac{2}{3}\left[ 1-\frac{2}{5}\left( \frac{4\Omega-3J_{2}}{\Omega+3J_{2}} \right)^{1/2} \right]$$
where $\Omega$ is the ratio of the centrifugal and gravitational forces
$$\Omega=\frac{\omega^2R_{eq}^3}{GM_{p}}$$