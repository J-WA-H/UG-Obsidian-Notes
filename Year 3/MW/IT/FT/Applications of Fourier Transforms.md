One applications of [[Fourier Transform]] is to solve differential equations.
Consider an infinity long string along the $x$ axis with a propagating wave with vertical displacement $y(x,t)$ that satisfies the wave equation
$$\frac{\partial^{2}y}{\partial t^2}=v^2 \frac{\partial^2y}{\partial x^2}.$$
Solve using Fourier transforms:
$$\tilde{y}(k,t)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxe^{-ikx}y(x,t)$$
$$y(x,t)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dke^{ikx}\tilde{y}(k,t).$$
$$\frac{\partial^2}{\partial t^2} \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dk\tilde{y}(k,t)e^{ikx}=v^2 \frac{\partial^2}{\partial x^2} \frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dk \tilde{y}(k,t)e^{ikx}$$
$$\int_{-\infty}^{\infty}dk \frac{\partial^2\tilde{y}}{\partial t^2}e^{ikx}=-v^2k^2\int_{-\infty}^{\infty}dk\tilde{y}(k,t)e^{ikx}$$
$$\implies \frac{\partial^2\tilde{y}}{\partial t^2}=-v^2k^2\tilde{y}(k,t).$$
This is the wave equation in Fourier space, which is much easier to solve.
Ansatz:
$$\tilde{y}(k,t)=A(k)e^{-ikvt}+B(k)e^{ikvt}$$
This gives
$$y(x,y)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dke^{ikx}[A(k)e^{-ikvt}+B(k)e^{ikvt}]$$
$$=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dk[A(k)e^{ik(x-vt)}+B(k)e^{ik(x+vt)}].$$
This solution consists of a plane wave moving right, and a plane wave moving left.
Example:
Solve
$$\frac{d^2f}{dx^2}-f=\delta(x).$$
The solution has a homogeneous and particular solution, $f(x)=f_{h}(x)+f_{p}(x)$ where
$$\frac{d^2f_{h}}{dx^2}-f_{h}=0$$
$$\frac{d^2f_{p}}{dx^2}-f_{p}=\delta(x).$$
First find homogeneous solution,
$$f_{h}(x)=Ae^{x}+Be^{-x}.$$
Now for the particular solution, using the [completeness relation](Delta%20Function.md) and definition of the Fourier transform:
$$\delta(x)=\frac{1}{2\pi}\int_{-\infty}^{\infty}e^{ikx}dk$$
$$f_{p}(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{f}_{p}(k)e^{ikx}dk.$$
Substituting into the equation gives
$$\frac{1}{\sqrt{ 2\pi }} \frac{d^2}{dx^2}\int_{-\infty}^{\infty}\tilde{f}_{p}(k)e^{ikx}dk-\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}\tilde{f}_{p}(k)e^{ikx}dk=\frac{1}{2\pi}\int_{-\infty}^{\infty}e^{ikx}$$
$$\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}(-k^2-1)\tilde{f}_{p}(k)e^{ikx}dk=\frac{1}{2\pi}\int_{-\infty}^{\infty}e^{ikx}.$$
For this equality to hold, the integrands must be equal so
$$(-k^2-1)\tilde{f}_{p}(k)=\frac{1}{\sqrt{ 2\pi }}$$
$$\implies \tilde{f}_{p}(k)=-\frac{1}{\sqrt{ 2\pi }} \frac{1}{k^2+1}.$$
Knowing the Fourier transform of the [Lorentzian](Parseval's%20Theorem.md), $\mathcal{F}\left[ \sqrt{ \frac{\pi}{2} } e^{-|x|}\right]=\frac{1}{k^2+1}$,
$$f_{p}(x)=-\frac{1}{2}e^{-|x|}.$$
This gives the full solution
$$f(x)=Ae^{x}+Be^{-x}-\frac{1}{2}e^{-|x|}.$$
Fourier transforms can also be applied to integral equations
Example:
Find $h(x)$ that satisfies
$$h(x)=e^{-i{3}x}+\int_{-\infty}^{\infty}dyh(x-y)e^{-|y|}.$$
The integral is a convolution of $h(x)*e^{-|x|}$
$$\implies h(x)=e^{-i 3x}+h(x)*e^{-|x|}.$$
Taking the Fourier transform of this expression, first we need $\mathcal{F}[e^{-i 3x}](k)$
$$\mathcal{F}[e^{-i 3x}](k)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxe^{i{3}x}e^{-ikx}=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dxe^{i(3-k)x}=\sqrt{ 2\pi }\delta(3-k)=\sqrt{ 2\pi }\delta(k-3).$$
Using the Lorentzian
$$\tilde{h}(k)=\sqrt{ 2\pi }\delta(k-3)+\sqrt{ 2\pi }\tilde{h}(k)\sqrt{ \frac{2}{\pi} } \frac{1}{k^2+1}$$
$$\implies \tilde{h}(k)\left( 1-\frac{2}{k^2+1} \right)=\sqrt{ 2\pi }\delta(k-3)$$
$$\tilde{h}(k)\left( \frac{{k^2+1-2}}{k^2+1} \right)=\tilde{h}(k)\left( \frac{{k^2-1}}{k^2+1} \right)=\sqrt{ 2\pi }\delta(k-3)$$
$$\implies \tilde{h}(k)=\sqrt{ 2\pi } \frac{{k^2+1}}{k^2-1}\delta(k-3).$$
Take inverse Fourier transform to get $h(x)$.
$$h(x)=\frac{1}{\sqrt{ 2\pi }}\int_{-\infty}^{\infty}dk\sqrt{ 2\pi } \frac{{k^2+1}}{k^2-1}\delta(k-3)e^{ikx}$$
$$=\frac{{3^2+1}}{3^2-1}e^{i 3x}=\frac{5}{4}3^{i 3x}.$$
