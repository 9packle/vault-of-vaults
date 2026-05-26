The normal distribution can be written as 
$$
X \sim \mathcal{N}(\mu,\, \sigma ^2)
$$
where $\mu$ is the mean of the sample and $\sigma$ is the standard distribution. The distribution is a perfect bell-shaped curve, and the mean, median and mode all lie in the centre of the curve. The area under the curve also represents the total probability.

In some cases one of $x$, $\mu$, or $\sigma$ is not given, which means the standard normal distribution is needed: 
$$
Z \sim \mathcal{N}(0,\, 1)
$$
We can then convert the distribution to the standard distribution: 
$$
Z = \frac{X - \mu}{\sigma}
$$
Then we can find out the missing value of either the mean or standard distribution.

The normal distribution can also be used to do hypothesis testing:

[[Normal distribution testing]]

The normal distribution can also be used to approximate a binomial distribution once there are a lot of trials:

[[Binomial distribution]]

The conditions for a distribution $X \sim Bi(n,\, p)$ to be approximated by a normal distribution is that $n$ is large and $p \approx 0.5$. Then for the approximate normal distribution, $\mu = np$ and $\sigma^2 = np(1-p)$. The continuity correction also needs to be applied, where $P(X \geq 10)$ in the binomial distribution is equal to $P(X \geq 9.5)$ in the approximate normal distribution, since the binomial distribution is discrete and the normal distribution is continuous.