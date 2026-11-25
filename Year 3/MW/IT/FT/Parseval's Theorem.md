In general, Parseval's theorem states that the [[Fourier Transform]] is a [unitary](Unitary%20and%20Orthogonal%20Operators.md) operator.
As a result the Fourier transform preserves the inner product
$$\int_{-\infty}^{\infty}dxf^{*}(x)g(x)=\int_{-\infty}^{\infty}dk\tilde{f}^{*}(k)\tilde{g}(k)$$
$$\therefore \int_{-\infty}^{\infty}|f(x)|^2dx=\int_{-\infty}^{\infty}|\tilde{f}(k)|^2dk.$$
The normed [inner product](Scalar%20Products.md) in $x$ space and $k$ space are the same, the inner product is conserved.
Proof:
Substitute the definition of the Fourier transform into the RHS:
$$\int_{-\infty}^{\infty}dk\tilde{f}^{*}(k)g(k)=\int_{-\infty}^{\infty}dk \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxf^{*}(x)e^{ikx} \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dx'g(x')e^{-ikx'}$$
$$=\frac{1}{2\pi}\int_{-\infty}^{\infty} dxf^{*}(x)\int_{-\infty}^{\infty}dx'g(x')\int_{-\infty}^{\infty}dke^{ik(x-x')}$$
$$=\frac{1}{2\pi}\int_{-\infty}^{\infty}dxf^{*}(x)\int_{-\infty}^{\infty}dx'g(x')2\pi\delta(x-x')$$
$$=\int_{-\infty}^{\infty}dxf^{*}(x)\int_{-\infty}^{\infty}dx'g(x')\delta(x-x')=\int_{-\infty}^{\infty}dxf^{*}(x)g(x)\;\square.$$
Now prove the inverse:
$$f(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{f}(k)e^{ikx}dk=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty} \frac{1}{k^2+1}e^{ikx}dk.$$
Complexify the function so take $k\to z.$
$$I=\oint_{\gamma}dz \frac{e^{ixz}}{z^2+1}.$$
Consider the case where $x>0$. Consider $z=w+iy$, $e^{ix(w+iy)}=e^{ixw}e^{-xy}$. As $x>0$, this goes to zero as $y\to \infty$ so integrate in the upper half plane. In this case the only relevant pole is $z=i$. Using [[Residue Theorem]]:
$$\text{Res}[f,i]=\lim_{ z \to i } (z-i)\frac{e^{ixz}}{(z+i)(z-i)}=\lim_{ z \to i } \frac{e^{ixz}}{z+i}=\frac{e^{-x}}{2i}$$
so for $x>0$, the integral becomes
$$I^{+}=2\pi i \frac{e^{-x}}{2i}=\pi e^{-x}.$$
For $x<0$, consider $z=w+iy$ so $e^{ix(w+iy)}=e^{ixw}e^{-xy}$. As $x<0$, this goes to zero as $y\to-\infty$ so integrate in the lower half plane, so the only pole relevant is $z=-i$.
$$\text{Res}[f,-i]=\lim_{ z \to -i } (z+i) \frac{e^{ixz}}{(z+i)(z-i)}=\lim_{ z \to -i } \frac{e^{ixz}}{z-i}=\frac{e^{x}}{-2i}$$
so for $x<0$ the integral becomes
$$I^{-}=-2\pi i \frac{e^{x}}{-2i}=\pi e^{x}$$
this gives the total integral $I=\pi e^{-|x|}$.
Substituting this back into the Fourier transform gives
$$f(x)=\frac{1}{\sqrt{ 2\pi }}\pi e^{-|x|}=\sqrt{ \frac{\pi}{2} }e^{-|x|}.$$
 
Example: Lorentzian function:
$$f(x)=\sqrt{ \frac{\pi}{2} }e^{-|x|}$$
$$\tilde{f}(k)=\frac{1}{\sqrt{ 2\pi }}\sqrt{ \frac{\pi}{2} }\int_{-\infty}^{\infty}e^{-|x|}e^{-ikx}dx=\frac{1}{2}\int_{0}^{\infty}e^{-x(ik+1)}dx+\frac{1}{2}\int_{-\infty}^{0}e^{x(1-ik)}dx$$
$$=\frac{1}{2}\left[ \frac{e^{-x(1+ik)}}{-(1+ik)} \right]^{\infty}_{0}+\frac{1}{2}\left[ \frac{e^{-x(1-ik)}}{1-ik} \right]_{-\infty}^{0}=\frac{1}{2}\left[ \frac{1}{1+ik}+\frac{1}{1-ik} \right]$$
$$=\frac{1}{2}\left[ \frac{{1-ik+1+ik}}{(1+ik)(1-ik)} \right]=\frac{1}{k^2+1}.$$
Example: Solve
$$I=\int_{0}^{\infty} \frac{dk}{(\alpha^2+k^2)^2}=\frac{1}{\alpha^{4}}\int_{0}^{\infty} \frac{dk}{\left( 1+\left( \frac{k}{\alpha} \right) ^2\right)^2}=\frac{1}{2\alpha^4}\int_{-\infty}^{\infty} \frac{dk}{\left( 1+\left( \frac{k}{\alpha} \right)^2 \right)^2}$$
Sub $k'=\frac{k}{\alpha}$
$$I=\frac{1}{2\alpha^3} \int_{-\infty}^{\infty} \frac{dk'}{(1+k')^2}=\frac{1}{2\alpha^3}\int_{-\infty}^{\infty} dk' \frac{1}{1+k^2} \frac{1}{1+k^2}$$
Take
$$\tilde{f}(k)=\frac{1}{1+k^2}\implies f(x)=\sqrt{ \frac{\pi}{2} }e^{-|x|}.$$
Using Parseval's theorem,
$$I=\frac{1}{2\alpha^3}\int_{-\infty}^{\infty}dxe^{-|x|}e^{-|x|}=\frac{1}{\alpha^{3}}\int_{0}^{\infty}dxe^{-2|x|}=\frac{1}{\alpha^3}\int_{0}^{\infty}dxe^{-2x}$$
$$=\frac{1}{\alpha^3}\left[ -\frac{1}{2}e^{-2x} \right]_{0}^{\infty}=\frac{1}{2\alpha^3}.$$
