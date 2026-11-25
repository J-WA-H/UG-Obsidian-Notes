Atmospheric sources (gaining atmosphere):
1. Accretion of gas from solar nebula before the sun's radiation disperses the gas from the protoplanetary disk.
2. Delivery of volatile molecules during collisions with other bodies.
3. Outgassing of volatile molecules from magma within the planets itself.

Source 1. leads to primary atmospheres while 2. and 3. lead to secondary atmospheres.

Atmospheric sinks (losing atmosphere):
1. Thermal (Jeans) escape with fastest molecules exceeding the escape speed.
2. Non-thermal escape, which typically involves interacting that leave molecules charged and susceptible to acceleration in the solar B-field.
3. Blowoff, where escaping light elements such as hydrogen entrain heavier molecules.
4. Erosion during impacts with incoming bodies.

Thermal escape:
For planets with sufficient B-fields to protect atmosphere from non-thermal loss processes, atmospheric retention depends on the rms velocity at the top of the atmosphere.
$$v=\sqrt{ \frac{3k_{B}T}{\mu m_{H}} }$$
relative to the escape velocity
$$v_{e}=\sqrt{ \frac{2Gm_{p}}{R_{p}} }.$$
Define the top of the atmosphere as the level above which 50% of upward moving molecules do not hit another molecule. Temperature here depends on the solar flux and will vary with semi-major axis
$$T\propto a^{-1/2};\;v\propto a^{-1/4}.$$
Empirically, to retain an atmosphere for the age of the solar system requires $v_{e}>10v$.

The pressure dependence on height can be found from [[Hydrostatic Equilibrium]].
$$\frac{dP}{dz}=-\rho g.$$
For an ideal gas, $PV=Nk_{B}T$:
$$\rho=\frac{N\mu m_{H}}{V}=\frac{N\mu m_{H}P}{k_{B}T}$$
$$\implies \frac{dP}{dz}=-\frac{\mu m_{H}gP}{k_{B}T}=-\frac{P}{H}$$
where $H$ is the scale height, given by
$$H=\frac{k_{B}T}{\mu m_{H}g}.$$
Integrating the ODE above gives
$$\int_{P_{0}}^P \frac{dP}{P}=-\frac{1}{H}\int_{0}^{h}dz$$
$$\ln\left( \frac{P}{P_{0}} \right)=-\frac{h}{H}$$
$$\implies P(h)=P_{0}e^{-h/H}.$$
This shows atmospheric pressure undergoes an exponential decay with height.