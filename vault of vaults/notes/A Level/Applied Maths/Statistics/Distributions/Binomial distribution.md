The binomial distribution can be written as 
$$
X \sim Bi(n,\, p)
$$
where $n$ is the number of trials and $p$ is the probability of success for each trial. It is a discrete distribution, meaning that $P(X\geq 10) = 1 - P(X\leq 9)$, and the probability can be found by
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
This can be proven by combining $n$ identical binomial distribution in the form of $X \sim Bi(1,\,p)$ - each distribution obviously has $E(X) = p$ and $Var(X) = p(1-p)$, so when we combine these identically distributed distributions, since each singular trial is a Bernoulli trial, they are independent and so 
$$
E(X_1 + X_2 + \ldots) = E(X_1) + E(X_2) + \ldots
$$ and 
$$
Var(X_1 + X_2 + \ldots) = Var(X_1) + Var(X_2) + \ldots
$$
$$
\implies E(X) = np,\, Var(X) = np(1-p)
$$
where $X \sim Bi(n,p)$.