Example:
$$I=\int_{0}^{x} \frac{dx'}{1-x'^2}.$$
Let $x'=\tanh(u)$, $dx'=\text{sech}^2(u)du$. Boundaries: $u_{1}=\text{arctanh}(x)$, $u_{0}=\text{arctanh}(0)=0$,
$$I=\int_{0}^{u_{1}} \frac{\text{sech}^2(u)}{1-\tanh^2(u)}du=\int_{0}^{u_{1}}du=u_{1}=\text{arctanh}(x).$$
Example:
$$I_{p}=\int_{0}^{\pi/2}\log(\tan x)\log(\tan^px+\cot^px)dx.$$
Let $u=\tan x$, $du=\sec^2xdx=(1+\tan^2x)dx=(1+u^2)dx$. Boundaries: $u_{0}=\tan(0)=0$, $\tan\left( \frac{\pi}{2} \right)=\infty$.
$$I_{p}=\int_{0}^{\infty}\log(u)\log(u^{p}+u^{-p}) \frac{du}{1+u^2}$$
Let $u=e^{v}$. $du=e^{v}dv$ Boundaries: $v_{0}=\log(0)=-\infty$, $v_{1}=\log(\infty)=\infty$.
$$I_{p}=\int_{-\infty}^{\infty} \frac{e^{v}dv}{1+e^{2v}}\log(e^{v})\log(e^{pv}+e^{-pv})=\int_{-\infty}^{\infty} \frac{e^{v}dv}{1+e^{2v}}v\log(e^{ pv }+e^{ -pv })$$$$=\int_{-\infty}^{\infty} \frac{e^{v}}{1+e^{ 2v }}v\log(2\cosh(pv))dv.$$
Examine each term: 
$$\frac{e^{v}}{1+e^{ 2v }}\text{ - even}$$$$v \text{ - odd}$$$$\log(2\cosh(pv)) \text{ - even}.$$
The integral is odd so $I_{p}=0$.
Alternatively, $v=\frac{1}{u}$, $du=-\frac{dv}{v^2}$, $v_{0}=\infty$ $v_{1}=0$.
$$I_{p}=\int_{\infty}^{0} -\frac{dv}{v^2} \frac{1}{1+\frac{1}{v^2}}\left( \log \frac{1}{v} \right)\log\left( v^{p}+\frac{1}{v^{p}} \right)=\int_{0}^{\infty} \frac{dv}{v^2+1}(-\log v)\log\left( v^{p}+\frac{1}{v^{p}} \right)=-I_{p}$$
$$\therefore I_{p}=0.$$
Integrating ratios:
$$I=\int R(x)dx=\int \frac{P(x)}{Q(x)}dx$$
Assume the rank of $P$ is smaller than the rank of $Q$ and $Q$ is factorisable.
$$Q=\prod_{i=1}^{N}(x-x_i).$$
This means we can write the ratio in partial fractions.
$$R(x)=\sum_{i=1}^{N} \frac{q_{i}}{x-x_{i}}\therefore I=\sum_{i=1}^{N} q_{i}\log(x-x_{i}).$$
Example:
$$R(x)=\frac{{1+x^2}}{x^3+6x^2+11x+6}.$$
Factorise $Q$:
$$x^3+6x^2+11x+6=(x+1)(x^2+6x+6)=(x+1)(x+2)(x+3).$$
$$R(x)=\frac{q_{1}}{x+1}+\frac{q_{2}}{x+2}+\frac{q_{3}}{x+3}.$$
$$q_{1}(x+2)(x+3)=q_{2}(x+1)(x+3)+q_{3}(x+1)(x+2)=1+{x^2}.$$
This gives $q_{1}=1,q_{2}=-5,q_{3}=5$.
$$I=\int R(x)dx=\int \frac{1+x^2}{x^3+6x^2+11x+6}.$$
$$I=\log(x+1)-5\log(x+2)+5\log(x+{3})=\log\left( \frac{(x+1)(x+3)^5}{(x+2)^{5}} \right).$$
Example: Complex numbers
$$I=\int_{0}^{\infty}e^{-ax}\cos(\lambda x)dx=\mathrm{Re}\left[ \int_{0}^{\infty}e^{-ax+i\lambda x}dx \right]=\mathrm{Re}\left[ \frac{e^{-(a-i\lambda)x}}{-(a-i\lambda)} \right]_{0}^{\infty}=\mathrm{Re}\left[ \frac{1}{a-i\lambda} \right]$$$$=\mathrm{Re}\left[ \frac{{a+i\lambda}}{a^2+\lambda^2} \right]=\frac{a}{a^2+\lambda^2}.$$
Example: Differentiating under the integral sign
$$I=\int_{0}^{\infty} \frac{{\sin x}}{x}dx.$$
$$I(\alpha)=\int_{0}^{\infty} e^{-\alpha x} \frac{\sin x}{x}dx$$ where $I=I(0)$.
$$\frac{dI(\alpha)}{d\alpha}=\int_{0}^{\infty} \frac{d}{d\alpha}e^{-\alpha x} \frac{\sin x}{x}dx=\int_{0}^{\infty}-xe^{-\alpha x} \frac{\sin x}{x}dx=-\int_{0}^{\infty}e^{-\alpha x}\sin xdx$$
$$=\mathrm{Im}\left[ -\int_{0}^{\infty}e^{-\alpha x+ix}dx \right]=\mathrm{Im}\left[ \frac{e^{-(\alpha-i)x}}{\alpha-i} \right]=\mathrm{Im}\left[ -\frac{1}{\alpha-i} \right]=\mathrm{Im}\left[ -\frac{\alpha+i}{\alpha^2+1} \right]=-\frac{1}{\alpha^{2}+1}.$$
$$\frac{dI(\alpha)}{d\alpha}=-\frac{1}{\alpha^2+1}\implies I(\alpha)=-\int \frac{1}{\alpha^2+1}d\alpha=-\arctan(\alpha)+c.$$
Using the fact that $I(\infty)=0$, $-\arctan(\infty)+c=0\implies c=\frac{\pi}{2}$.
$$I=I(0)=\frac{\pi}{2}.$$
