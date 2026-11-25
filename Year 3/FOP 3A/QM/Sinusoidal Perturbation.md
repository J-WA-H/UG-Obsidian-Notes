To show an application of [[Perturbation Theory]], we will calculate $c_{a}^{(\lambda)}(t)$ and $c_{b}^{(\lambda)}(t)$ for the perturbation
$$\hat{H}'(\underline{r},t)=V(\underline{r})\cos(\omega t).$$
We will assume there are no transitions within the same state so $\bra{\psi_{a}}\hat{H}'(\underline{r},t)\ket{\psi_{a}}=\bra{\psi_{b}}\hat{H}'(\underline{r},t)\ket{\psi_{b}}=0$.
Take the initial condition $\Psi(t)=\psi_{a}$.
$$c_{b}^{(1)}(t)=-\frac{i}{\hbar}V_{ba}\int_{0}^tdt'\cos(\omega t')e^{i\omega_{0}t}$$
$$=-\frac{i}{2\hbar}V_{ba}\int_{0}^tdt'(e^{i\omega t'}+e^{-i\omega t'})e^{i\omega_{0}t'}=-\frac{i}{2\hbar}V_{ba}\int_{0}^tdt'[e^{i(\omega_{0}+\omega)t'}+e^{-i(\omega_{0}-\omega)t'}]$$
$$=-\frac{1}{2\hbar}V_{ba}\left[ \frac{1}{\omega_{0}+\omega}e^{i(\omega_{0}+\omega)t'}+\frac{1}{\omega_{0}-\omega}e^{-i(\omega_{0}-\omega)t'} \right]_{0}^t$$
$$=-\frac{1}{2\hbar}V_{ba}\left[ \frac{{e^{i(\omega_{0}+\omega)t}-1}}{\omega_{0}+\omega}+{\frac{e^{-i(\omega_{0}-\omega)t}-1}{\omega_{0}-\omega}} \right].$$
For large times, $t\gg \frac{1}{\omega_{0}}$,
$$c_{b}^{(1)}(t)=-\frac{V_{ba}}{\hbar}\left[ \frac{{e^{i(\omega_{0}-\omega)t}-1}}{\omega_{0}-\omega} \right]=-\frac{V_{ba}}{2\hbar}e^{i(\omega_{0}-\omega)t/2}\left[ \frac{{e^{i(\omega_{0}-\omega)t/2}-e^{-i(\omega_{0}-\omega)t/2}}}{\omega_{0}-\omega} \right]$$
$$=-\frac{V_{ba}}{2\hbar}e^{i(\omega_{0}-\omega)t/2}\left[ \frac{2i\sin\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{\omega_{0}-\omega} \right]=-\frac{V_{ba}}{\hbar}e^{i(\omega_{0}-\omega)t/2}\left[ \frac{i\sin\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{\omega_{0}-\omega} \right].$$
This shows that the probability of a transition between states $b$ to $a$ is
$$P_{b\to a}=\lvert c_{b}^{(1)}(t) \rvert^2=\frac{\lvert V_{ba}\rvert^2}{\hbar^2} \frac{\sin^2\left[ \frac{(\omega_{0}-\omega)t}{2} \right]}{(\omega_{0}-\omega)^2}.$$
![[Pasted image 20241102154913.png]]
