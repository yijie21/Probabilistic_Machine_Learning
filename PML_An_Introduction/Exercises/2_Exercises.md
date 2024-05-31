**Exercise 2.1**

a. The set $ii$ is sufficient for the calculation, because:
$$
P(H|e_1,e_2)=\frac{P(H)P(e_1,e_2|H)}{P(e1,e2)}
$$
according to the Bayes rule.

b. Both $i$ and $ii$ are sufficient now, because:
$$
E_1,E_2|H\rightarrow P(e_1,e_2|H)=P(e_1|H)P(e_2|H)
$$

**Exercise 2.2**

Suppose a tetrahedron dice where three faces are painted as red, green and blue,respectively, and the 4th face is painted with all three colors.

Any pair of variables are independent, for example:
$$
\begin{align*}
P(red\cap blue) &= P(red) * P(blue)\\
&=\frac{1}{2} * \frac{1}{2}\\
&=\frac{1}{4}
\end{align*}
$$
But:
$$
\begin{align*}
P(red\cap green\cap blue)\neq \frac{1}{8}
\end{align*}
$$
**Exercise 2.3**

(Reference from [StackExchange](https://stats.stackexchange.com/questions/125479/conditional-independence-iff-joint-factorizes))

If we integrate both sides in $x$:
$$
\int_Xp(x,y|z)dx=\int_Xg(x,z)h(y,z)dx
$$
This implies:
$$
p(y|z)=h(y,z)\int_Xg(x,z)dx
$$
And this tells us that:
$$
h(y,z)=p(y|z)\mu(z)
$$
And for $g$, we can also get:
$$
g(x,z)=p(x|z)\omega(z)
$$
Therefore,
$$
g(x,z)h(y,z)=p(y|z)\mu(z)p(x|z)\omega(z)
$$
Since both sides integrate to 1, we conclude with:
$$
\mu(z)\omega(z)=1
$$
So:
$$
p(x,y|z)=p(x|z)p(y|z)
$$
Therefore,
$$
X\perp Y|Z
$$
**Exercise 2.4**

(Lengthy proving process. Just remember the convolution of two Gaussian is still a Gaussian.)

**Exercise 2.5**

Set $Z=min(X,Y)$, and construct the cdf function of $Z$ as $F_Z(z)$

(The detailed process can be referred to in [link](https://www.quora.com/Say-we-have-X-Uniform-0-1-and-Y-Uniform-0-1-What-is-the-expected-value-of-the-minimum-of-X-and-Y))

**Exercise 2.6**

Refer to [link](https://www.google.com/search?q=Show+that+the+variance+of+a+sum+is&oq=Show+that+the+variance+of+a+sum+is&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRigAdIBBzIyOGowajSoAgCwAgE&sourceid=chrome&ie=UTF-8)

**Exercise 2.7**

Refer to [link](https://www.johndcook.com/inverse_gamma.pdf)

**Exercise 2.8**

Refer to [link](https://probml.github.io/pml-book/solns-public.pdf#page=4.12)

**Exercise 2.9**

Let $p(H=1)$ represents the prevalence of the disease. Let $Y=1$ if the test is positive, and $Y=0$ otherwise. And now I want to compute $p(H=1|Y=1)+p(H=1|Y=0)$.
$$
\begin{align*}
p(H=1|Y=1)&=\frac{p(H=1)p(Y=1|H=1)}{p(Y=1|H=1)p(H=1)+p(Y=1|H=0)p(H=0)}\\
&=\frac{0.0001*0.99}{0.99*0.0001+0.01*0.9999}\\
&=0.009804
\end{align*}
$$

$$
\begin{align*}
p(H=1|Y=0)&=\frac{p(H=1)p(Y=0|H=1)}{p(Y=0|H=1)p(H=1)+p(Y=0|H=0)p(H=0)}\\
&=\frac{0.0001*0.01}{0.01*0.0001+0.99*0.9999}\\
&=0.00001
\end{align*}
$$

So
$$
p(H=1|Y=1)+p(H=1|Y=0)=0.009814
$$
**Exercise 2.10**

(refer to [link](https://probml.github.io/pml-book/solns-public.pdf#page=4.12))

a. Mistaken $p(E|I)$ for $p(I|E)$ 

b. The evidence has shrink the range of guilty people from 80000 to 8000, thus relevant.

**Exercise 2.11**

a. $\frac{2}{3}$

b. $\frac{1}{2}$

**Exercise 2.12**

Refer to [link](https://probml.github.io/pml-book/solns-public.pdf#page=4.12)

Key: reformulate a standard gaussian distribution.
