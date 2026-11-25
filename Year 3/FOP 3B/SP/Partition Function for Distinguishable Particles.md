**When a question talks about distinguishable or localised particles, that means classical!**

Consider 2 distinguishable particles that can be in one of 2 single particle states, $\epsilon_{1},\epsilon_{2}$.
![[Pasted image 20241024185011.png]]
The partition function can be found from this
$$Z=\sum_{n=1}^4e^{-\beta\epsilon_{n}}=e^{-2\beta\epsilon_{1}}+e^{-\beta (\epsilon_{1}+\epsilon_{2})}+e^{-\beta(\epsilon_{2}+\epsilon_{1})}+e^{-2\beta\epsilon_{2}}.$$
$$=(e^{-\beta\epsilon_{1}}+e^{-\beta\epsilon_{2}})^2.$$
This is the square of the partition function for one particle that can be in two possible states, which we will call $Z_{(1)}$.
This can be used to generalise this system for $N$ distinguishable particles:
$$Z_{(N)}=(Z_{(1)})^N.$$
Distinguishable particles follow the usual rules of probability.

Now consider 2 indistinguishable particles in the same two state system:
![[Pasted image 20241024185752.png]]
$$Z_{(2)}=e^{-\beta\epsilon_{1}}+e^{-\beta(\epsilon_{1}+\epsilon_{2})}+e^{_\beta\epsilon_{2}}\neq(Z_{(1)})^2.$$
Due to the above partition function, care has to be taken when dealing with quantum particles.

Example: Localised spin-$\frac{1}{2}$ particles in a $B$ field.
If we have N particles in an applied B filed then they can be in one of two states - parallel or antiparallel to the B field. 
$$\epsilon_{0}=-\mu B=-\frac{\epsilon}{2}$$
$$\epsilon_{1}=+\mu B=+\frac{\epsilon}{2}$$where $\mu$ is the magnetic moment.
$$Z=e^{-\beta\epsilon_{0}}+e^{-\beta\epsilon_{1}}=e^{\beta\epsilon/2}+e^{-\beta\epsilon/2}=e^{\beta\epsilon/2}(1+e^{-\beta\epsilon}).$$
We aim to find the probability of each state being occupied as a function of temperature.
Using definition of the [probability](Partition%20Function.md),
$$P_{0}=\frac{e^{\beta\epsilon/2}}{e^{\beta\epsilon/2}(1+e^{-\beta\epsilon})}=\frac{1}{1+e^{-\beta\epsilon}}$$
$$P_{1}=\frac{e^{-\beta\epsilon/2}}{e^{\beta\epsilon/2}(1+e^{-\beta\epsilon})}=\frac{e^{-\beta\epsilon}}{1+e^{-\beta\epsilon}}.$$
![[Pasted image 20241024190954.png]]
We can calculate the magnetisation per particle by evaluating the average magnetic moment.
$$\frac{M}{N}=P_{0}\mu+P_{1}(-\mu)=N \frac{{1-e^{-\beta\epsilon}}}{1+e^{-\beta\epsilon}}=N\tanh\left( \frac{\beta\epsilon}{2} \right).$$
Now we have $Z$, we can calculate [bulk thermodynamic properties](Link%20Between%20Statistical%20and%20Thermodynamics.md).