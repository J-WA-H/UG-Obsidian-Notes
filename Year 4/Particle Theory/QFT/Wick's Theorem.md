Wick's theorem relates time ordered products to [[Normal Ordering]]. Consider the product of operators in the interaction picture $\hat{\phi}_{I}(x_{1})\hat{\phi}(x_{2})$. The interaction picture is used so we can use free fields which are defined by the creation and annihilation operators, which allows normal ordering to happen. 

First, split $\hat{\phi}_{I}$ into $\hat{\phi}_{I}^{-}+\hat{\phi}_{I}^{+}$ where
$$\hat{\phi}^{-}(x)=\int \frac{d^3k}{(2\pi)^32E_{k}}\hat{a}_{k}e^{ -ik_{\mu}x^{\mu} };\;\hat{\phi}^{+}(x)=\int \frac{d^3k}{(2\pi)^32E_{k}}\hat{a}^{\dagger}_{k}e^{ ik_{\mu}x^{\mu} }.\tag{9.1} $$
This gives the product as
$$\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2})=(\hat{\phi}^{-}(x_{1})+\hat{\phi}^{+}(x_{1}))(\hat{\phi}^{-}(x_{2})+\hat{\phi}^{+}(x_{2}))=\hat{\phi}^{-}(x_{1})\hat{\phi}^{-}(x_{2})+\hat{\phi}^{-}(x_{1})\hat{\phi}^{+}(x_{2})+\hat{\phi}^{+}(x_{1})\hat{\phi}^{-}(x_{2})+\hat{\phi}^{+}(x_{1})\hat{\phi}^{+}(x_{2}).\tag{9.2} $$
As normal ordering moves the creation operators left and the annihilation operators right, only the second term isn't normal ordered, so rewriting it as a normal ordered product gives
$$\hat{\phi}^{-}(x_{1})\hat{\phi}^{+}(x_{2})=\hat{\phi}^{+}(x_{2})\hat{\phi}^{-}(x_{1})+[\hat{\phi}^{-}(x_{1}),\hat{\phi}^{+}(x_{2})]\tag{9.3} .$$
The commutator evaluates to
$$\int \frac{d^3k}{(2\pi)^32E_{k}}e^{ -ik_{\mu}(x_{1}-x_{2})^{\mu} }\equiv D(x_{1}-x_{2}).\tag{9.4} $$
This gives the total product
$$\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2})=:\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2}):+\bra{0} \hat{\phi}(x_{1})\hat{\phi}(x_{2})\ket{0} .\tag{9.5} $$
Applying time ordering gives
$$T(\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2}))=:\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2}):+\bra{0} T(\hat{\phi}_{I}(x_{1})\hat{\phi}_{I}(x_{2}))\ket{0} \tag{9.6} $$
using the fact that time ordering doesn't effect normal ordered products.

This shows that time and normal ordering are related by a Feynman propagator,
$$T(\hat{\phi}(x_{1})\hat{\phi}(x_{2}))=:\hat{\phi}(x_{1})\hat{\phi}(x_{2}):+G_{F}(x_{1}-x_{2}).\tag{9.7} $$
This is the simple version of Wick's theorem - a product of 2 fields.

Normal ordering only works in free fields as we need $\hat{a},\hat{a}^{\dagger}$ operators so we use the interaction picture.

The product of 3 fields is given by
$$T(\hat{\phi}(x_{1})\hat{\phi}(x_{2})\hat{\phi}(x_{3}))=:\hat{\phi}(x_{1})\hat{\phi}(x_{2})\hat{\phi}(x_{3}):+:\hat{\phi}(x_{1}):G_{F}(x_{2}-x_{3})+:\hat{\phi}(x_{2}):G_{F}(x_{1}-x_{3})+:\hat{\phi}(x_{3}):G_{F}(x_{1}-x_{3}).\tag{9.8} $$
The general patter is that any time-ordered product of fields is equal to its normal ordered version plus terms in which pairs of fields are removed from the normal ordered product, and sandwiched between the vacuum to form 2-point functions. Then one sums over all permutations,
$$\begin{matrix}
T(\hat{\phi}(x_{1})\dots \hat{\phi}(x_{n}))=:\hat{\phi}(x_{1})\dots \hat{\phi}(x_{n}):+:\hat{\phi}(x_{1})\dots \overbrace{\hat{\phi}(x_{i})\dots \hat{\phi}(x_{j})}\dots \phi(x_{n}):\bra{0}T(\hat{\phi}(x_{i})\hat{\phi}(x_{j}))\ket{0}  +\text{perms} \\
+:\hat{\phi}(x_{1})\dots \overbrace{\hat{\phi}(x_{i})\dots \hat{\phi}(x_{j})}\dots\overbrace{\hat{\phi}(x_{k})\dots \hat{\phi}(x_{l})}\dots \hat{\phi}(x_{n}):\bra{0}T(\hat{\phi}(x_{i})\hat{\phi}(x_{j})) \ket{0} \bra{0} T(\hat{\phi}(x_{k})\hat{\phi}(x_{l}))\ket{0}+\text{perms}  \\
+\dots+\bra{0}T(\hat{\phi}(x_{1})\hat{\phi}(x_{2}))\ket{0} \bra{0} T(\hat{\phi}(x_{3})\hat{\phi}(x_{4}))\ket{0} \dots \bra{0} T(\hat{\phi}(x_{n-1})\hat{\phi}(x_{n})) +\text{perms}.
\end{matrix}\tag{9.9} $$
The overbrace $\overbrace{\hat{\phi}(x_{i})\dots\hat{\phi}(x_{j})}$ shows that $\hat{\phi}(x_{i}),\hat{\phi}(x_{j})$ have been removed from the normal ordered product and paired in the Feynman propagator.

Consider the Greens function
$$G_{n}(x_{1},\dots,x_{n})=\bra{0} T(\hat{\phi}(x_{1})\dots\hat{\phi}(x_{n}))\ket{0}.\tag{9.10}  $$
From the definition of normal ordering, creation operators are moved left and annihilation operators are moved right, applying the vacuum states to the time-order product from Wick's theorem eliminates any terms with normal ordering, since $\bra{0}\hat{a}^{\dagger}=0$ and $\hat{a}\ket{0}=0$. From $(9.8)$, it is obvious that $G_{3}$ vanishes since every term has a normal ordered operator. This extends to any odd numbered Green's function. For example,
$$G_{4}(x_{1},x_{2},x_{3},x_{4})=\bra{0} T(\phi(x_{1})\phi(x_{2})\phi (x_{3})\phi(x_{4}))\ket{0} =G_{F}(x_{1}-x_{2})G_{F}(x_{3}-x_{4})+G_{F}(x_{1}-x_{3}) G_{F}(x_{2}-x_{4})+G_{F}(x_{1}-x_{4})G_{F}(x_{2}-x_{3}).$$
$(9.11)$
In functional form, Wick's theorem is
$$T(\hat{\phi}(x_{1})\dots \hat{\phi}(x_{n}))=: \exp\left[ \frac{1}{2} \frac{\delta}{\delta \phi}G_{F} \frac{\delta}{\delta \phi} \right]\hat{\phi}(x_{1})\dots \hat{\phi}(x_{n}): \tag{9.12} $$where the exponent is defined by
$$\frac{1}{2} \frac{\delta}{\delta \phi}G_{F} \frac{\delta}{\delta \phi}=\frac{1}{2}\int d^4x \int d^3y \frac{\delta}{\delta \phi(x)}G_{F}(x-y) \frac{\delta}{\delta \phi(y)} \tag{9.13} $$which uses variational derivatives, which when applied to the field operators is
$$\frac{\delta \phi(x_{i})}{\delta \phi(x)}=\delta^{(4)}(x-x_{i}).\tag{9.14} $$
