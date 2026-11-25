Consider the [transition probability](Electrons%20In%20Atoms%20in%20an%20EM%20field.md)
$$P_{a\to b}(\omega,t)=\frac{{\lvert V_{ba} \rvert^2}}{\hbar^2} \frac{\sin^2\left[ (\omega_{0}-\omega) \frac{t}{2} \right]}{(\omega_{0}-\omega)^2}.$$
![[Pasted image 20241108200357.png]]
Consider a transition between state a and an area of densely packed states. 
Looking at
$$dN(E_{n})=\left( \frac{dN}{dE} \right)_{E_{n}};dE_{n}=\rho(E_{n})dE_{n}.$$
$\rho(E_n)$ is known as the density of states.
$$P_{i\to n}dN(E_{n})=p_{i\to n}\rho(E_{n})dE_{n}$$
$$=\frac{{\lvert V_{in} \rvert^2 }}{\hbar^2} \frac{{\sin^2\left[ (\omega_{0}-\omega) \frac{t}{2} \right]}}{(\omega_{0}-\omega)^2}\rho(E_{n})dE_{n}.$$
The total probability of excitation from $E_{i}\to E_{f}\pm \frac{\Delta}{2}$ where $\Delta$ is some small energy change.
$$P_{i\to f}=\frac{{\lvert V_{in} \rvert^2 }}{\hbar^2}\int_{E_{f}-\Delta/2}^{E_{f}+\Delta/2} \frac{{\sin^2\left[ (\omega_{0}-\omega) \frac{t}{2} \right]}}{(\omega_{0}-\omega)^2}\rho(E_{n})dE_{n}.$$
Using the long time limit where the sinc function goes to a delta function,
$$P_{i\to f}=\frac{{\lvert V_{in} \rvert^2 }}{\hbar^2}\rho(E_{f}) \frac{\pi t}{2}$$
and the rate of transition is given by
$$R_{i\to f}=\frac{{\lvert V_{if} \rvert^2 }}{\hbar^2} \frac{\pi}{2}\rho(E_{f}).$$
This is known as Fermi's Golden rule.