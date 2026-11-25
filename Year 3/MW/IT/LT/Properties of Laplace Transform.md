The key properties of the [[Laplace Transform]] are:
1. Linearity: $\mathcal{L}[af(t)+bg(t)](s)=a\mathcal{L}[f(t)](s)+b\mathcal{L}[g(t)](s)$, $f,g:\mathbb{R}\to \mathbb{C}$, $a,b\in \mathbb{C}$.
	For the inverse, $\mathcal{L}^{-1}[\mathcal{L}[f(t)](s)](t)=\mathcal{L}[\mathcal{L}[f(t)]]=f(t)$.
	Example:
	$$\hat{f}(s)=\frac{4}{s^2+2s}.$$
	$$\hat{f}(s)=4\cdot \frac{1}{2}\left( \frac{1}{s}-\frac{1}{s+2} \right)=2\left( \frac{1}{s}-\frac{1}{s+2} \right).$$
	$$f(t)=2\mathcal{L}^{-1}\left[ \frac{1}{s} \right](t)-2\mathcal{L}^{-1}\left[ \frac{1}{s+2} \right](t)=2\cdot 1-2e^{-2t}\therefore f(t)=2-2e^{-2t}.$$
2. Translation: 
	$$\mathcal{L}[f(t-t')\Theta(t-t')](s)=\int_{0}^{\infty}dte^{-st}f(t-t')\Theta(t-t').$$
	Let $t_{1}=t-t'$, $\implies t=t_{1}+t'$, $dt_{1}=dt$
	$$\mathcal{L}[f(t-t')\Theta(t-tl)](s)=\int_{-t'}^{\infty}dt_{1}e^{-s(t_{1}+t')}f(t_{1})\Theta(t_{1})=e^{-st'}\int_{0}^{\infty}dt_{1}e^{-st_{1}}f(t_{1})=e^{-st'}\hat{f}(s).$$
	$$\mathcal{L}[f(t-t')](s)=e^{-st'}\hat{f}(s).$$
	Similarly, $$\mathcal{L}[e^{s't}f(t)](s)=\int_{0}^{\infty}dte^{-st}e^{s't}f(t)=\int_{0}^{\infty}dte^{-t(s-s')}f(t)=\hat{f}(s-s').$$$$\therefore \mathcal{L}[e^{s't}f(t)](s)=\hat{f}(s-s').$$
3. Scaling: For $\lambda>0$,
	$$\mathcal{L}[f(\lambda t)](s)=\int_{0}^{\infty}dte^{-st}f(\lambda t).$$
	Let $t_{1}=\lambda t$, $dt_{1}=\lambda dt$.
	$$\mathcal{L}[f(\lambda t)](s)=\int_{0}^{\infty} \frac{dt_{1}}{\lambda}e^{-st_{1}/\lambda}f(t_{1})=\frac{1}{\lambda}\int_{9}^{\infty}dt_{1}e^{-(s/\lambda)t}f(t_{1})=\frac{1}{\lambda}\hat{f}\left( \frac{s}{\lambda} \right).$$
	$$\therefore\mathcal{L}[f(\lambda t)](s)=\frac{1}{\lambda}\hat{f}\left( \frac{s}{\lambda} \right).$$
	Example:
	$$f(t)=\begin{cases}
1 & 0\leq t\leq 1 \\
2-t & 1\leq t\leq 2 \\
0 & t\geq 2
\end{cases}.$$
	![[Pasted image 20250208125425.png]]
	Split this function into two parts,
	![[Pasted image 20250208125501.png]]
	The first graph, in terms of the heavy side function is $\Theta(t)-\Theta(t-1)$ and the second one is given by $(2-t)[\Theta(t-1)-\Theta(t-2)]$
	$$\therefore f(t)=\Theta(t)-\Theta(t-1)+(2-t)[\Theta(t-1)-\Theta(t-2)]$$
	$$=\Theta(t)-(t-1)\Theta(t-1)+(t-2)\Theta(t-2).$$
	$$\hat{f}(s)=\mathcal{L}[\Theta(t)](s)-\mathcal{L}[(t-1)\Theta(t-1)](s)+\mathcal{L}[(t-2)\Theta(t-2)](s)$$
	$$=\frac{1}{s}-\frac{e^{-s}}{s^2}-\frac{e^{-2t}}{s^2}.$$
	