# 6 Joint Distributions and Conditional Expectation

With data coming from several groups, we should consider both *within* group variation and *between* group variation.

Using *conditional expectation*, we can predict the value of one random variable, given the information we have about other random variables.

## 6.1 Joint, marginal, and conditional distributions

We introduce multivariate analogs of the CDF, PMF, and PDF.


Key concepts:

* **Distribution** of RV $X$ provides complete information about the probability of $X$ into any subset of real line.
* **Joint distribution** of two RVs $X$ and $Y$ and provides complete information about the probability of the vector $(X,Y)$.
* **Marginal distribution** of $X$ is the individual distribution of $X$ ignoring the value of $Y$.
* **Conditional distribution** of $X$ given $Y=y$ is the updated distribution of $X$ after observing $Y=y$.

### Discrete joint CDF, PMF:

The **joint CDF** of RVs $X$ and $Y$ is the function $F_{XY}$ given by:

$$
F_{XY}(x,y)=P(X\leq x,Y\leq y)
$$

analogously for joint CDF of $n$ RVs.

The **joint PMF** of discrete RVs $X$ and $Y$ is the function $p_{XY}$, given by:

$$
p_{XY}(x,y)=P(X = x,Y = y)
$$

analogously for joint PMF of $n$ RVs.

We require valid joint PMF to be nonnegative and sum to $1$:

$$
\sum_x \sum_y P(X=x, Y=y)=1.
$$

**Marginal PMF:**
For discrete RVs $X$ and $Y$, the *marginal PMF* of $X$ is:

$$
P(X=x)=\sum_y P(X=x, Y=y)
$$

The operation of summering over the possible values of $Y$ in order to convert the joint PMF to marginal PMF is *marginalizing* out of $Y$.
