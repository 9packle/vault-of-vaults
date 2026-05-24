---

---
The method for taking a gradient of a curve is to select a two values each of $x$ and $y$, and then do 

$$
\frac{y_2-y_1}{x_2-x_1}
$$

Thus to get closer and closer to the gradient at a point on the curve $y = f(x)$ we can have the $x$-axis distance between the points be $h$, and so we have 

$$
\frac{f(x+h)-f(x)}{(x+h)-x}
$$

Then as the value of $h$ approaches zero, the expression gets closer to the gradient of the curve at the point. We can write this as 

$$
\lim_{h\to0}\frac{f(x+h)-f(x)}{(x+h)-x}
$$

For example, if we differentiate $y = x^2$ using this method, we would have 

$$
\lim_{h\to0} \frac{(x+h)^2-x^2}{(x+h)-x}
$$

If we simplify the expression we get 

$$
\lim_{h\to0} 2x+h^2
$$

And as $h\to0$, the expression approaches $2x$.
