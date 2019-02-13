Compiled: https://samybencherif.github.io/RotationProof/

We start with the expression below, and wonder how it could possibly be equivalent to the far more simple expression $xcos(\theta) - ysin(\theta)$.

1) $x^{'} = \sqrt{x^2+y^2} \cdot cos(\theta + acos(x/\sqrt{x^2+y^2}))$

Then we substitute $\sqrt{x^2+y^2}$ with $r$ for convenience.

2) $x^{'} = rcos\Big(\theta + acos\big(\frac{x}{r}\big)\Big)$

Next we will using the following identity.

$cos(\alpha+\beta) = cos(\alpha)cos(\beta) - sin(\alpha)sin(\beta)$

[more info](https://en.wikipedia.org/wiki/List_of_trigonometric_identities#Angle_sum_and_difference_identities)

3) $x^{'} = r\Big(cos(\theta)cos\big(acos\frac{x}{r}\big) - sin(\theta)sin\big(acos\frac{x}{r}\big)\Big)$

Notice that $cos\Big(acos\big(\frac{x}{r}\big)\Big) = \frac{x}{r}$

4) $x^{'} = r\Big(cos(\theta)\frac{x}{r} - sin(\theta)sin\big(acos\frac{x}{r}\big)\Big)$

Now we will use the identity $sin(acos(\gamma)) = \sqrt{1-\gamma^2}$.

[more info](https://math.stackexchange.com/a/1252289/86997)

5) $x^{'} = r\Big(cos(\theta)\frac{x}{r} - sin(\theta)\sqrt{1-\big(\frac{x}{r}\big)^2}\Big)$

Distribute $r$.

6) $x^{'} = cos(\theta)x - rsin(\theta)\sqrt{1-\big(\frac{x}{r}\big)^2}$

Recall that $r$ was just a placeholder for $\sqrt{x^2+y^2}$. We will now substitute this value back into the second $r$.

7) $x^{'} = cos(\theta)x - rsin(\theta)\sqrt{1-\big(\frac{x}{\sqrt{x^2+y^2}}\big)^2}$

Now it is time to exponentiate both parts of the fraction.

8) $x^{'} = cos(\theta)x - rsin(\theta)\sqrt{1-\frac{x^2}{x^2+y^2}}$

Find a common denominator.

9) $x^{'} = cos(\theta)x - rsin(\theta)\sqrt{\frac{x^2+y^2}{x^2+y^2}-\frac{x^2}{x^2+y^2}}$

Subtract.

10) $x^{'} = cos(\theta)x - rsin(\theta)\sqrt{\frac{y^2}{x^2+y^2}}$

Now we will split the radical over the fraction. (Hang in there, we're almost done.)

11) $x^{'} = cos(\theta)x - rsin(\theta)\frac{y}{\sqrt{x^2+y^2}}$

Now lets substitute $\sqrt{x^2+y^2}$ for the last remaining $r$.

12) $x^{'} = cos(\theta)x - \sqrt{x^2+y^2}sin(\theta)\frac{y}{\sqrt{x^2+y^2}}$

It cancels!

13) $x^{'} = cos(\theta)x - sin(\theta)y$

Rearrange variables.

14) $x^{'} = xcos(\theta) - ysin(\theta)$

Congratulations on making it this far! Now you know how to find this reduced equation without using the geometric proof.
