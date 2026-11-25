To consider the transformations of EM fields under a [Lorentz transformation](Lorentz%20Transforms.md), we need to have some assumptions
- Transformation is independent of source
- Transformation is linear

To consider the transformation of fields, consider a capacitor in the frame $S_{0}$
![[Pasted image 20241129160540.png]]
Take this to be the rest frame of the charges. In this frame the charge density is $\sigma_{0}$. The E-field in this frame is
$$E_{0}=\frac{\sigma_{0}}{\varepsilon_{0}}\underline{\hat{y}}.$$
Consider a frame $S$ that is moving at a speed $v_{0}$ with respect to $S_{0}$. The distance between the charges undergo [[Length Contraction]] which gives $\sigma=\gamma(v_{0})\sigma_{0}$ which gives an E field of
$$\underline{E}=\gamma(v_{0})\underline{E}_{0}.$$
In $S$, the charges are moving so there is also a magnetic field, given by $\underline{B}=-\mu_{0}\sigma v_{0}\underline{\hat{z}}$.
![[Pasted image 20241129162342.png]]
Considering a frame $S'$ moving at speed $v$ with respect to $S$, the E and B fields are given by
$$E'_{y}=\frac{\sigma'}{\varepsilon_{0}}$$
$$B_{z}'-\mu_{0}\sigma'v'$$
$$\sigma'=\gamma(v')\sigma_{0}.$$
We are looking to compare the fields in $S$ and $S'$. The speed of $S'$ with respect to $S_{0}$, $v'$, is given by the relativistic [velocity transform](Relativistic%20Magnetism.md),
$$v'=\frac{{v+v_{0}}}{1+vv_{0}/c^2}.$$
The fields in the $S'$ frame will be of the form
$$E_{y}'=\frac{\gamma(v')}{\gamma(v_{0})} \frac{\sigma}{\varepsilon_{0}}$$
$$B_{z}'=-\left( \frac{\gamma(v')}{\gamma(v_{0})} \right)\mu_{0}\sigma v'.$$
$$\frac{\gamma(v')}{\gamma(v_{0})}=\frac{\sqrt{ 1-v_{0}^2/c^2 }}{\sqrt{ 1-v'^2/c^2 }}=\frac{\cancel{\sqrt{ 1-v_{0}^2/c^2 }}(1+vv_{0}/c^2)}{\cancel{\sqrt{ 1-v_{0}^2/c^2 }}\sqrt{ 1-v^2/c^2 }}=\gamma(v)\left( 1+\frac{vv_{0}}{c^2} \right).$$
This gives
$$E_{y}'=\gamma(v)\left( 1+\frac{vv_{0}}{c}^2 \right) \frac{\sigma}{\varepsilon_{0}}=\gamma(v)\left( \frac{\sigma}{\varepsilon_{0}}+\frac{vv_{0}}{c^2} \frac{\sigma}{\varepsilon_{0}} \right)=\gamma(v)(E_{y}-vB_{z}).$$
$$B_{z}'=-\gamma(v)\left( 1+\frac{vv_{0}}{c^2} \right)\mu_{0}\sigma\left( \frac{{v+v_{0}}}{1+vv_{0}/c^2} \right)=-\gamma(v)\mu_{0}\sigma(v+v_{0})=\gamma(v)\left( B_{z}-\frac{vE_{y}}{c^2} \right).$$
Now rotate the capacitor about the $x$ axis to find the other components
![[Pasted image 20241129182232.png]]
Doing the same derivation as above, we get
$$E_{z}'=\gamma(v)\left( E_{z}+vB_{y} \right)$$
$$B_{y}'=\gamma(v)\left( B_{y}+\frac{v}{c^2}E_{z} \right).$$
![[Pasted image 20241129182624.png]]
For this rotation, the charges lie orthogonal to the $x$ axis and the boost, so only the distance between the plates undergoes length contraction - so the charge density doesn't change
$$E_{x}=E'_{x}.$$
![[Pasted image 20241129182819.png]]
For the B field, consider a Solenoid aligned on the $x$ axis. The number density of turns undergoes length contraction. $n'=\gamma(v)n$. The current, defined as the rate of change of charge, undergoes [[Time Dilation]] so $I'=\frac{I}{\gamma(v)}$.
$$B_{x}'=\mu_{0}n'I'=\mu_{0}\cancel{\gamma(v)}n \frac{I}{\cancel{\gamma(v)}}=\mu_{0}nI=B_{x}.$$
This shows EM fields do not transform at [[4-Vectors]]