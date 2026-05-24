---

---
A fraction with more than one linear factor in the denominator can be split into partial fractions - writing it as a sum of two or more simpler fractions.

This is useful for things like binomial expansion and integration.

For example, this fraction 

$$
\frac{7x-7}{(2x+1)(x-3)}
$$

can be rewritten as 

$$
\frac{A}{2x+1}+\frac{B}{x-3}
$$

Something like 

$$
\frac{7x-1}{(x-3)(x-1)(x+2)}
$$

can be rewritten as 

$$
\frac{A}{x-3}+\frac{B}{x-1}+\frac{C}{x+2}
$$

The values of the numerators can be found by writing the two expressions together as an identity, like so: 

$$
\frac{7x-7}{(2x+1)(x-3)}\equiv\frac{A}{2x+1}+\frac{B}{x-3}
$$

Then adding the partial fractions together we get 

$$
7x-7 \equiv A(x-3)+B(2x+1)
$$

This allows for the coefficients to be equated, so then we have $A+2B=7$ and $-3A+B=-7$, which can then be solved as simple simultaneous equations for $A$ and $B$.
