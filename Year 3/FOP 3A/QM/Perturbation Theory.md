We will assume the time-dependent Hamiltonian, $\hat{H}'(t)$, is small compared to $\hat{H}^{0}$. We will introduce a small parameter $\lambda$ to scale the perturbation, giving $\hat{H}=\hat{H}^{0}+\lambda\hat{H}'(t)$.
$$\therefore i\hbar \frac{\partial \ket{\Psi^{(\lambda)}(t)} }{\partial t}=[\hat{H}^{0}+\lambda \hat{H}'(t)]\ket{\Psi^{(\lambda)}(t)}.$$
where
$$\ket{\Psi^{(\lambda)}(t)}=c_{a}^{(\lambda)}(t)\ket{\psi_{a}}e^{-iE_{a}t/\hbar} +c_{b}^{{(\lambda)}}(t)\ket{\psi_{b}}e^{-iE_{b}t/\hbar}.$$
The [system of ODEs](Time%20Dependence.md) for the probability amplitudes thus becomes
$$\dot{c}_{a}^{(\lambda)}(t)=-\frac{i}{\hbar}\lambda c_{b}^{(\lambda)}(t)H'_{ab}e^{-i\omega_{0}t}$$
$$\dot{c}_{b}^{(\lambda)}(t)=-\frac{i}{\hbar}\lambda c_{a}^{(\lambda)}(t)H'_{ba}e^{i\omega_{0}t}.$$
Apply the boundary condition that $\Psi^{(\lambda)}(0)=\psi_{a}$.
$$\Psi^{\lambda}(0)=c_{a}^{(\lambda)}(0)\psi_{a}+c_{b}^{(\lambda)}(0)\psi_{b}$$
$$\implies c_{a}^{(\lambda)}(0)=1,c_{b}^{(\lambda)}(0)=0.$$
As $c_{a.b}^{(\lambda)}(t)$ are smooth functions of $\lambda$, they can be expanded around $\lambda=0$:
$$c_{a}^{(\lambda)}(t)=c_{a}^{(0)}(t)+\lambda c_{a}^{(1)}(t)+\mathcal{O}(\lambda^2)$$
$$c_{a}^{(\lambda)}(t)=c_{b}^{(0)}(t)+\lambda c_{b}^{(1)}(t)+\mathcal{O}(\lambda^2).$$
Substituting these Taylor expansions into the first ODE gives
$$\dot{c}_{a}^{(0)}(t)+\lambda \dot{c}_{a}^{(1)}(t)=-\frac{i}{\hbar}\lambda[\dot{c}_{b}^{(0)}(t)+\lambda \dot{c}_{b}^{(1)}(t)]\hat{H}'_{ab}e^{-i\omega_{0}t}$$
We can equate orders of $\lambda$
$\mathcal{O}(\lambda^0)$:
$$\dot{c}_{a}^{(0)}(t)=0\implies c_{a}^{(0)}\text{ is constant}.$$
$\mathcal{O}(\lambda^1)$:
$$\dot{c}_{a}^{(1)}(t)=-\frac{i}{\hbar}c_{b}^{(0)}(t)\hat{H}'_{ab}e^{-i\omega_{0}t}.$$
From initial conditions $c_{a}^{(\lambda)}(0)=1=c_{a}^{(0)}(0)+\lambda c_{a}^{(1)}(t)+\mathcal{O}(\lambda^2) \implies c_{a}^{(0)}(0)=1;\;c_{a}^{(1)}(0)=0$.
From the fact that $c_{a}^{(0)}(t)$ is constant in time, $c_{a}^{(0)}(t)=1$.

Doing the same for $c_{b}^{(\lambda)}(t)$:
$$\dot{c}_{b}^{(0)}+\lambda \dot{c}_{b}^{(1)}=-\frac{i}{\hbar}\lambda[c_{a}^{(0)}(t)+\lambda c_{a}^{(1)}(t)]\hat{H}'_{ba}e^{i\omega_{0}t}$$
$\mathcal{O}(\lambda^0)$:
$$\dot{c}_{b}^{(0)}(t)=0$$
$\mathcal{O}(\lambda^1)$:
$$\dot{c}_{b}^{(1)}(t)=-\frac{i}{\hbar}c_{a}^{(0)}(t)\hat{H}'_{ba}e^{i\omega_{0}t}.$$
Applying initial conditions:
$$c_{b}^{(0)}(0)=0\implies c_{b}^{(0)}(t)=0$$
Since $c_{b}^{(0)}(t)=0$, we get $\dot{c}_{a}^{(1)}(t)=0 \implies c_{a}^{(1)}(t)$ is time independent. Since $c_{a}^{(1)}(0)=0$, $c_{a}^{(1)}(t)=0$

Since $c_{a}^{(0)}(t)=1$, $\dot{c}_{b}^{(1)}=-\frac{i}{\hbar}\hat{H}'_{ba}e^{i\omega_{0}t}$.
Integrating over time gives
$$c_{b}^{(1)}(t)=-\frac{i}{\hbar}\int_{0}^tdt'\hat{H}'_{ba}e^{i\omega_{0}t'}.$$
This gives the total probability amplitudes as
$$c_{a}^{(\lambda)}(t)=1+\mathcal{O}(\lambda^2)$$
$$c_{b}^{(\lambda)}=-\frac{i\lambda}{\hbar}\int_{0}^tdt'\hat{H}'_{ba}e^{i\omega_{0}t'}.$$
Up to $\lambda=1$, we have the wavefunction to first order in $\lambda$:
$$\Psi(t)=\psi_{a}e^{-iE_{a}t/\hbar}-\frac{i}{\hbar}\psi_{b}e^{-iE_{b}t/\hbar}\int_{0}^tdt'\hat{H}'_{ba}(t')e^{i\omega_{0}t}.$$
