Einstein's summation convention allows us to get rid of the summation sign.
1. Summation is implied when we have a sub or superscript index
2. Index used in implicit summation is a dummy index and can be replaced by another one not in use
3. Infer summation range from context
4. Free indices are not summed over
5. Convention to put summation index as subscript on the left of the symbol containing the superscript

Using this convention we can rewrite the expansion of a vector in a [basis](Basis%20of%20Vectors.md) as
$$\underline{x}=x^{i}\underline{\hat{e}}_{i}.$$
For a [change of basis](Coordinate%20Transforms.md):
$$\underline{\hat{e}}_{j}'=\underline{\hat{e}}_{i}S^{\;i}_{j}.$$
$$x^{j}=S^{j}_{\;i}x'^{i}.$$
$$x'^{j}=R^{j}_{\;i}x^{i}=(S^{-1})^{j}_{\;i}x^{i}.$$
