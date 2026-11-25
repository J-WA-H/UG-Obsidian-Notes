Consider a periodic function with period $T$: $f(t+nT)=f(t)$ $n\in \mathbb{N}$. Its [[Laplace Transform]] is given by
$$\hat{f}(s)=\frac{1}{1-e^{-st}}\int_{0}^{T}dtf(t)e^{-st}.$$
Proof:
$$\hat{f}(s)=\int_{0}^{\infty}dte^{-st}f(t)=\left[ \int_{0}^{T}+\int_{T}^{2T}+\int_{2T}^{3T}+\dots \right]dte^{-st}f(t)$$
$$=\sum_{n=0}^{\infty}\int_{nT}^{(n+1)T}e^{-st}f(t)dt.$$
Let $t'=t-nT$, $dt'=dt$. When $t=nT,t'=0$, when $t=(n+1)T,t'=T$
$$\hat{f}(s)=\sum_{n=0}^{\infty}\int_{0}^{T}e^{-s(t'+nT)}f(t'+nT)dt'$$
$$=\sum_{n=0}^{\infty}e^{-snT}\int_{0}^{T}dt'e^{-st'}f(t')=\frac{1}{1-e^{-st}}\int_{0}^{T}dt'e^{-st}f(t)\;\square$$
