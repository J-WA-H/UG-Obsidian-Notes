Stirling's approximation:
$$\ln N! \approx N\ln N-N$$
This holds true as $N\to \infty$.

#### Proof:
$$\ln N! = \sum_{k=1}^N 1\cdot\ln(k)\approx \int_{1}^N\ln (k)dk$$
as for large $N$, we can take $1\approx dk$.
$$\int_{1}^N\ln(k)dk=[k\ln k-k]_{1}^N=N\ln N-N$$
This also gives $N! \approx\left( \frac{N}{e} \right)^N$.