If a [[Laplace Transform]] is more complicated than the [[Common Laplace Transforms]], then the Bromwich inversion integral needs to be used, which is given by the line integral
$$f(t)=\frac{1}{2\pi i} \int_{C-i\infty}^{C+i\infty}\hat{f}(s)e^{st}dt$$
where $C\in \mathbb{R}$.

Proof:
Recall that the Laplace transform was introduced for functions that don't decay to 0 as $t\to\infty$. We can find some positive constant $C\in \mathbb{R}^{+}$ such that
$$\lim_{ t \to \infty } g(t)=\lim_{ t \to \infty } f(t)e^{-Ct}=0.$$
For this to be true, $f$ must diverge slower than $e^{-st}$ converges.

As $g$ decays to zero $\exists\; \mathcal{F}[g(t)](\omega)$ which can be used to find $f(t)$. Using [[Fourier Transform]],
$$\tilde{g}(\omega)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dte^{-i\omega t}e^{-Ct}f(t)$$
$$=\frac{1}{\sqrt{ 2\pi }}\int_{0}^{\infty}dte^{-(C+i\omega)}f(t).$$
Introduce variable $s=C+i\omega$.
$$\frac{1}{\sqrt{ 2\pi }}\int_{0}^{\infty}dte^{-st}f(t).$$
This includes the Laplace transform.
Now consider the inverse Fourier transform,
$$g(t)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}d\omega \tilde{g}(\omega)e^{i\omega t}=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}d\omega  \frac{1}{\sqrt{ 2\pi }}\hat{f}(C+i\omega)e^{i\omega t}$$
set $s=C+i\omega \implies i\omega=s-C, d\omega=\frac{ds}{i}$.
$$f(t)\cancel{e^{-Ct}}=\frac{1}{2\pi i}\int_{C-i\infty}^{C+i\infty}ds\hat{f}(s)e^{(s-\cancel{C})t}$$
$$\implies f(t)=\frac{1}{2\pi i}\int_{C-i\infty}^{C+i\infty}ds\hat{f}(s)e^{st}.$$
$C$ is chosen to lie to the right of any poles.
![[Pasted image 20250219103931.png]]
The integration is along the vertical line $\{ C-i\infty, C+i\infty \}$ so that $C\in \mathbb{R}^{+}$.

Consider $t<0$: no singularities are enclosed in the contour,
![[Pasted image 20250219104243.png]]
$$\oint ds\hat{f}(s)e^{st}=0=\int_{C+i\infty}^{C-i\infty}ds\hat{f}(s)e^{st}+\int_{\gamma_{r}}ds\hat{f}(s)e^{st}$$
The integral over the line is $-I$ and the integral over the arc goes to 0 as $\hat{f}(s)e^{st}$ is vanishing.
$$\therefore f(t)=0$$
For $t>0$:
![[Pasted image 20250219104608.png]]
$$\oint ds\hat{f}(s)e^{st}=2\pi i\sum_{n} \mathrm{Res}[\hat{f}(s)e^{st},s_{n}]=\int_{C-i\infty}^{C+i\infty}ds\hat{f}(s)e^{st}+\int_{\gamma_{l}}ds\hat{f}(s)e^{st}=I+0$$
$$\therefore f(t)=\frac{1}{2\pi i}2\pi i\sum_{n}\mathrm{Res}[\hat{f}(s)e^{st},s_{n}]=\sum_{n}\mathrm{Res}[\hat{f}e^{st},s_{n}].$$
$$\therefore f(t)=\begin{cases}
\sum_{n}\mathrm{Res}[\hat{f}(s)e^{st},s_{n}] & t>0 \\
0 & t<0
\end{cases}.$$
Example: Find the inverse Laplace transform of 
$$\hat{f}(s)=\frac{1}{1+s^2}.$$
Rewrite as
$$\hat{f}(s)=\frac{1}{(s+i)(s-i)}.$$
We know for $t<0$, $f(t)=0$ so only consider for $t>0$ so we just need to calculate residues
$$\mathrm{Res} \left[ \frac{e^{st}}{(s+i)(s-i)},-i \right]=\lim_{ s \to -i } \cancel{(s+i)} \frac{e^{st}}{\cancel{(s+i)}(s-i)}=\lim_{ s \to -i } \frac{e^{st}}{s-i}=-\frac{e^{-it}}{2i}.$$
$$\mathrm{Res}\left[ \frac{e^{st}}{(s+i)(s-i)},i \right]=\lim_{ s \to i } \cancel{(s-i)} \frac{e^{st}}{(s+i)\cancel{(s-i)}}=\lim_{ s \to i } \frac{e^{st}}{s+i}=\frac{e^{it}}{2i}.$$
$$f(t)=\frac{e^{it}}{2i}-\frac{e^{-it}}{2i}=\sin(t)$$
$$\therefore f(t)=\sin(t)\Theta(t).$$
