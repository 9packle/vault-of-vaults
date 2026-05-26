The geometric distribution can be written as
$$
X \sim Geo(p)
$$
where $p$ is the probability of success. It is a discrete distribution, and the probability can be found by
$$
P(X = x) = (1-p)^{x-1}p
$$
$$
P(X > x) = (1-p)^{x-1}
$$
For events to be modelled by the geometric distribution they must be independent, have the same probability of success and immediately stop on the first success.

The mean and variance can be found by
$$
E(X) = \frac{1}{p}
$$
$$
Var(X) = \frac{1-p}{p^2}
$$