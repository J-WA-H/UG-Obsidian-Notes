The [[Vector Spaces]] considered so far have been of a finite dimension, so lets consider vector spaces with an infinite dimension [[Basis of Vectors]].

Consider the basis $\{ \underline{e}_{i} \}$ where $i=1,\dots,n$ and $n\to \infty$.
For a vector space $H$ with vector $\underline{p}\in H$,
$$\underline{p}=\underline{e}_{i}p^{i}=\lim_{ n \to \infty } \sum_{i=1}^{n}\underline{e}_{i}p^{i}.$$
We need to know if this infinite sum converges, and if it does, whether it converges on an element of $H$.

A pre-Hilbert space is a vector space with a Euclidean [inner product](Scalar%20Products.md). The inner product allows us to define the norm of the elements.
The definition of a complex inner product is:
$$\forall\;f,g\in X\to(f,g)\in \mathbb{C}.$$
- $$(f,g)=(g,f)^{*}$$
- $$(f,\alpha g)=\alpha(f,g)$$
$$(\alpha f,g)=\alpha^{*}(f,g)$$
- $$(f,g+{h})=(f,g)+(f,h)$$
- $$(f,f)>0\;\forall\;f\neq 0.$$
The inner product can be used to define the norm
$$\lVert f \rVert =\sqrt{ (f,f) }.$$
Theorem: A scalar product satisfies the Cauchy-Schwarz inequality
$$\lvert (f,g) \rvert \leq \lVert f \rVert \lVert g \rVert. $$
Proof:
For $g=0$, this is trivial, $(f,0)=0=\lVert f \rVert\cdot 0$.
For $g\neq 0$, consider $h=f+\alpha g$.
$$(f+\alpha g,f+\alpha g)=\lVert f \rVert^2+\alpha^{*}(g,f)+\alpha(f,g)+\lvert \alpha \rvert^2\lVert g \rVert^2 \geq 0.$$
take $\alpha=-(g,f)/\lVert g \rVert^2$.
$$(f+\alpha g,f+\alpha g)=\lVert f \rVert^2-\frac{(f,g)(g,f)}{\lVert g \rVert^2 }-\frac{(g,f)(f,g)}{\lVert g \rVert^2 }+\frac{{\lvert (f,g) \rvert }}{\lVert g \rVert ^2}  $$
$$=\lVert f \rVert ^2 -\frac{{\lvert (f,g) \rvert^2 }}{\lVert g \rVert^2 }\geq 0$$$$\implies \lvert (f,g) \rvert^2\leq \lVert f \rVert ^2 \lVert g \rVert ^2\;\;\square$$
This reduces to an equality when $f,g$ are linearly dependent.

Consider
$$\lVert f+g \rVert^2=\lVert f \rVert ^2+\lVert g \rVert^2+2\mathrm{Re}[(f,g)]. $$
Using Cauchy-Schwarz:
$$2\mathrm{Re}[(f,g)]\leq{2}\lvert (f,g) \rvert \leq{2}\lVert f \rVert\lVert g \rVert  $$
$$\lVert f+g \rVert^2\leq \lVert f \rVert^2+\lVert g \rVert^2+2\lVert f \rVert \lVert g \rVert    $$
$$\lVert f+g \rVert \leq \lVert f \rVert+\lVert g \rVert  $$
This is the triangle inequality.
