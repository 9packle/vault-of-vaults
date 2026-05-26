The binomial distribution can be written as 
$$
X \sim Bi(n,\, p)
$$
where $n$ is the number of trials and $p$ is the probability of success for each trial. It is a discrete distribution, and the probability can be found by
$$
P(X = x) = \binom{n}{x}p^x(1-p)^{n-x}
$$
For events to be modelled by the binomial distribution they must be independent, have a constant rate of success, have a fixed number of trials and only have two outcomes. 

The mean and variance can be found by
$$
E(X) = np
$$
$$
Var(X) = np(1-p)
$$