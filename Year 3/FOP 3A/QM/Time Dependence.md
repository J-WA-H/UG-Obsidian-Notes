A time-dependent Hamiltonian can be written as
$$\hat{H}(t)=\hat{H}^{0}+\hat{H}'(t)$$
where $\hat{H}^{0}$ is the normal [time-independent Hamiltonian](Two%20electron%20atoms.md) and $\hat{H}'(t)$ is some time dependent perturbation. 
The solution to this Hamiltonian is given by
$$\ket{\Psi(t)}=c_{a}(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+c_{b}\ket{\psi_{b}}e^{-iE_{b}t/\hbar}. $$
We can see that the amplitudes of the $\ket{\psi_{a}}$ and $\ket{\psi_{b}}$ states are now time-dependent, so the probabilities - given by $\lvert c_{i}(t) \rvert^2$ - are also time-dependent.

The time-dependent Schrodinger equation for this system is
$$i\hbar\frac{\partial \ket{\Psi(t)} }{\partial t}=(\hat{H}^{0}+\hat{H}'(t))\ket{\Psi(t)}. $$
To find expressions for $c_{a}(t)$, $c_{b}(t)$, first consider the LHS:
$$i\hbar\frac{\partial \ket{\Psi(t)} }{\partial t}=i\hbar[ \dot{c}_{a}(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+c_{a}(t)\ket{\psi_{a}}\left( -\frac{iE_{a}}{\hbar} \right)e^{-iE_{a}t/\hbar}$$$$+\dot{c}_{b}(t)\ket{\psi_{b}}e^{-iE_{b}t/\hbar}+c_{b}(t)\ket{\psi_{b}}\left( -\frac{iE_{b}}{\hbar} \right)e^{-iE_{b}t/\hbar}     ]$$
Now consider the RHS:
$$[\hat{H}^{0}+\hat{H}'(t)]\ket{\Psi(t)}=c_{a}(t)E_{a}\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+c_{b}(t)E_{b}\ket{\psi_{b}}e^{-iE_{b}t/\hbar}$$$$+c_{a}(t)\hat{H}'(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+c_{b}(t)\hat{H}'(t)\ket{\psi_{b}}e^{-iE_{b}t/\hbar} $$
Equating and cancelling both sides gives
$$i\hbar(\dot{c}_{a}(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+\dot{c}_{b}(t)\ket{\psi_{b}}e^{-iE_{b}t/\hbar} )=c_{a}(t)\hat{H}'(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar}+c_{b}(t)\hat{H}'(t)\ket{\psi_{b}}e^{-iE_{b}t/\hbar}.$$
We can multiply both sides by $\bra{\psi_{a}}e^{+iE_{a}t/\hbar}$ leaving
$$\dot{c}_{a}(t)=-\frac{i}{\hbar}[c_{a}(t)H'_{aa}+c_{b}(t)H'_{ab}e^{-i(E_{b}-E_{a})t/\hbar}]$$Multiplying by $\bra{\psi_{b}}e^{iE_{b}t/\hbar}$ gives
$$\dot{c}_{b}(t)=-\frac{i}{\hbar}[c_{b}(t)H'_{bb}+c_{a}(t)H_{ba}e^{+i(E_{b}-E_{a})t/\hbar}].$$
where $H'_{ij}=\bra{\psi_{i}}H'(t)\ket{\psi_{j}}$. In special cases the diagonal transitions are unaffected by the perturbation so $H'_{aa}=H'_{bb}=0$.

This simplifies the result to a set of two coupled first order ODEs
$$\dot{c}_{a}(t)=-\frac{i}{\hbar}c_{b}(t)H'_{ab}e^{-i\omega_{0}t}$$
$$\dot{c}_{b}(t)=-\frac{i}{\hbar}c_{a}(t)H'_{ba}e^{i\omega_{0}t}.$$
where $\omega_{0}=(E_{b}-E_{a})/\hbar$.