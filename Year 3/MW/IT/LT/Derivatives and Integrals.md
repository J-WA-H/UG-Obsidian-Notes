Consider the [[Laplace Transform]] of a derivative,
$$\mathcal{L}[f'(t)](s)=\int_{0}^{\infty} dte^{-st} \frac{df}{dt}=[e^{-st}f(t)]_{0}^{\infty}+s \int_{0}^{\infty}dtf(t)e^{-st}=s\hat{f}(s)-f(0).$$
This gives the Laplace transform of a derivative as
$$\mathcal{L}[f'(t)](s)=s\hat{f}(s)-f(0).$$
For the second derivative,
$$\mathcal{L}[f''(t)](s)=\mathcal{L}\left[ \frac{d}{dt}(f'(t)) \right](s)=s\mathcal{L}[f'(s)](s)-f'(0)=s[s\hat{f}(s)-f(0)]-f'(0)$$
$$\mathcal{L}[f''(t)](s)=s^2\hat{f}(s)-sf(0)-f'(0).$$
In general:
$$\mathcal{L}[f^{(n)}(t)](s)=s^n-\sum_{j=1}^{n}s^{n-j}f^{(n-j)}(0).$$
A derivative in $t$ corresponds to a multiplication in $s$.

For the integral of a function,
$$\mathcal{L}\left[ \int_{a}^{t}dt'f(t) \right](s)=\frac{1}{s}\hat{f}(s)-\frac{1}{s}\int_{0}^{a}dt'f(t')$$
Proof:
$$\mathcal{L}\left[ \int_{a}^{t}dt'f(t) \right](s)=\int_{0}^{\infty}dte^{-st}\int_{a}^{t}dt'f(t')=\left[ \frac{e^{-st}}{-s}\int_{a}^tdt'f(t') \right]_{0}^{\infty}-\int_{0}^{\infty}dtf(t) \frac{e^{-st}}{-s}$$
$$=\frac{1}{s}\int_{a}^{0}f(t')dt'+\frac{1}{s}\int_{0}^{\infty}dtf(t)e^{-st}=\frac{1}{s}\hat{f}(s)-\frac{1}{s}\int_{0}^{a}dt'f(t')\;\square.$$
