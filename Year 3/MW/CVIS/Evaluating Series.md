Example: The Basel problem
$$S=1+\frac{1}{4}+\frac{1}{16}+\frac{1}{36}+\dots+\frac{1}{(2n)^2}.$$
This is the sum of the square of even numbers,
$$S=1+\sum_{n=1}^{\infty} \frac{1}{(2n)^2}.$$
The 1 is brought out as it doesn't match the pattern,
$$S=1+\frac{1}{4}\sum_{n=1}^{\infty} \frac{1}{n^2}=1+\frac{1}{4}\zeta(2)=1+\frac{1}{4} \frac{\pi^2}{6}=1+\frac{\pi^2}{24}.$$
Example: [Telescopic Series](Infinite%20Series.md)
$$S=\sum_{n=1}^{\infty} \frac{1}{n(n+1)}.$$
Split using partial fractions,
$$\frac{1}{n(n+1)}=\frac{A}{n}+\frac{B}{n+1}$$
$$1=A(n+1)+Bn$$
For $n=0$:
$$1=A$$
For $n=-1$
$$1=-B\implies B=-1.$$
$$\therefore S=\sum_{n=1}^{\infty}\left(  \frac{1}{n}-\frac{1}{n+1} \right).$$
Evaluate terms:
$$1-\cancel{\frac{1}{2}}+\cancel{\frac{1}{2}}-\cancel{\frac{1}{3}}+\cancel{\frac{1}{3}}-\cancel{\frac{1}{4}}+\dots+\lim_{ n \to \infty }\left( \cancel{\frac{1}{n}}-\frac{1}{n+1} \right) $$
$$=1-\lim_{ n \to \infty } \left( \frac{1}{n+1} \right)=1.$$
We can also use the connection between series and integrals to evaluate sums.
Example:
$$\log(1+x)=\int_{0}^{x} \frac{dx}{1+x}.$$
Taylor expand the integral:
$$\int_{0}^{x} \frac{dx}{1+x}=\int_{0}^{x}(1-x+x^2-x^3+\dots)dx=\left[ x-\frac{1}{2}x^2+\frac{1}{3}x^3+\dots \right]_{0}^{x}=\sum_{n=1}^{\infty}(-1)^{n+1} \frac{x^{n}}{n}.$$
For the inverse,
$$\sum_{n=1}^{\infty}(-1)^{n+1} \frac{x^{n}}{n}=\int_{0}^{x}dx \sum_{n=1}^{\infty}(-1)^{n-1}x^{n-1}=\int_{0}^{x}dx\sum_{n=0}^{\infty}(-1)^{n}x^{n}=\int_{0}^{x} \frac{1}{1+x}dx=\log(1+x).$$
Example:
$$S=\sum_{n=0}^{\infty} \frac{1}{(2n+1)2^{2n+1}}.$$
Substitute $x=\frac{1}{2}$,
$$S(x)=\sum_{n=0}^{\infty} \frac{x^{2n+1}}{2n+1}=\sum_{n=0}^{\infty}\int_{0}^{x}dx x^{2n}=\int_{0}^{x}dx\sum_{n=0}^{\infty}x^{2n}=\int_{0}^{x} \frac{1}{1-x^{2}}dx=\text{arctanh}(x)$$
$$\implies S=S\left( \frac{1}{2} \right)=\text{arctanh}\left( \frac{1}{2} \right).$$
Example: 
$$S=\frac{1}{2}+\frac{1}{4}+\frac{1}{16}+\frac{1}{96}+\dots$$
Check for pattern:
$$\frac{1}{2}\times \frac{1}{2}=\frac{1}{4};\; \frac{1}{4}\times \frac{1}{4}=\frac{1}{16};\; \frac{1}{16}\times \frac{1}{6}=\frac{1}{96}.$$
$$\therefore S=\sum_{n=0}^{\infty} \frac{1}{2^{n+1}n!}.$$
Substitute $x=\frac{1}{2}$,
$$S(1)=\sum_{n=1}^{\infty} \frac{x^{n+1}}{n!}=x\sum_{n=0}^{\infty} \frac{x^{n}}{n!}=xe^{x}.$$
$$\therefore S=S\left( \frac{1}{2} \right)=\frac{1}{2}e^{1/2}.$$
Aside: Reindexing
$$\sum_{n=1}^{\infty}f(n)=\sum_{n=0}^{\infty}f(n+1)$$
$$\sum _{n=0}^{\infty}f(n)=f(0)+\sum_{n=1}^{\infty}f(n)$$
Aside: Alternating terms,
- For odd terms that are negative, $(-1)^{n}$
- For even terms negative, $(-1)^{n+1},(-1)^{n-1}$.
- Other alternations:
	- Use $\lfloor a \rfloor$ to give the integer part of $a$, e.g. $\lfloor 2.1 \rfloor=2$.
$(-1)^{\lfloor n/2 \rfloor}$ gives two positive, and two negative values.

