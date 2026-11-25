For a Laplace transform the convolution using the [heavy-side function](Delta%20Function.md) is defined as
$$f\times g=\int_{0}^{\infty}dt'g(t-t')\Theta(t-t')f(t')\Theta(t')$$
$$=\int_{0}^{t}dt'g(t-t')f(t').$$
Properties:
1. Linearity: $f\times(ag+bh)=a(f\times g)+b(f\times h)$.
2. Commutative: $f\times g=g\times f$
	Proof:
	$$f\times g=\int_{0}^{t}dt'g(t-t')f(t')$$
	$$g\times f=\int_{0}^{\infty}dt''f(t-t'')\Theta(t-t'')g(t'')\Theta(t'')$$
	Call $t'=t-t''$, $dt'=-dt''$,
	$$g\times f=\int_{t}^{-\infty}dt'f(t')\Theta(t')g(t-t')\Theta(t-t')$$
	$$=\int_{-\infty}^tdt'f(t')\Theta(t')g(t-t')\Theta(t-t')=\int_{0}^{t}dt'f(t')g(t-t')\;\square$$

The [[Laplace Transform]] of a convolution is given by
$$\mathcal{L}[f\times g](s)=\hat{f}(s)\hat{g}(s).$$
Proof:
$$\hat{f}(s)\hat{g}(s)=\int_{0}^{\infty}dt'e^{-st'}f(t')\Theta(t')\int_{0}^{\infty}dt''e^{-st''}g(t'')\Theta(t'')$$
$$=\int_{0}^{\infty}dt'\int_{0}^{\infty}dt''f(t'')\Theta(t'')e^{-s(t'+t'')}g(t'')\Theta(t'')$$
Call $t=t'+t''$, $dt''=dt$
$$\hat{f}(s)\hat{g}(s)=\int_{0}^{\infty}dtf(t')\Theta(t')\int_{t'}^{\infty}dte^{-st}g(t-t')\Theta(t-t').$$
From $\Theta(t-t')$ $\implies t-t'>0\implies t>t'$.
$$\hat{f}(s)\hat{g}(s)=\int_{0}^{\infty}dt'f(t')\Theta(t')\int_{0}^{\infty}dte^{-st}g(t-t')\Theta(t-t')=$$$$\int_{0}^{\infty}dte^{-st}\int_{0}^{\infty}dt'g(t-t')\Theta(t-t')f(t')\Theta(t-t')=\int_{0}^{\infty}dte^{-st}(f\times g)=\mathcal{L}[f\times g](s)\;\square$$
Example:
$$\hat{f}(s)=\frac{4}{s^2(s+2)^2}=\frac{4}{s^2} \frac{1}{(s+2)^2}=\hat{g}(s)\hat{h}(s).$$
Recall the [[Common Laplace Transforms]] $\mathcal{L}[t]=\frac{1}{s}$ and $\mathcal{L}[e^{-2t}]=\frac{1}{s+2}$.
$$g(t)=\mathcal{L}^{-1}\left[ \frac{4}{s^2} \right](t)=4t$$
$$h(t)=\mathcal{L}^{-1}\left[ \frac{1}{(s+2)^2} \right]=e^{-2t}\mathcal{L}^{-1}\left[ \frac{1}{s^2} \right](t)=te^{-2t}$$
from [[Properties of Laplace Transform]].
$$\therefore f(t)=g\times h=\int_{0}^{t}dt'g(t-t')h(t')=4\int_{0}^{t}dt'(t-t')t'e^{-2t'}=t-1+e^{-2t}(1+t)$$
$$f(t)=t-1+(1+t)e^{-2t}.$$
