# 7 Markov Chains

For the Markov chain, the past and **the future are conditionally independent**. For the special case of random walk on an undirected network, the network structure is the key to determining the stationary distribution.

We can picture a Markov chain intuitively by imagining a system with *states* and someone randomly wandering around from state to state.

 For many interesting Markov chains, the *stationary* distribution of the chain helps us understand how the chain will behave in the long run.

## 7.1 Markov property and transition matrix

A sequence of RVs $X_0, X_1, X_2, ...$ evolving over time. This is called a *stochastic process*.

Markov chains have a form of one-step dependence, allowing to do beyond IIDs bust still have very convenient structure.

Markov chains widely used for simulations of complex distributions, via algorithms known as *Markov chain Monte Carlo (MCMC).*

Markov chains live in both space and time: the set of possible states $X_n$ is called *state time*, and index $n$ represents evolution of the process over *time*. The state space of can be discrete or continuous, and time can also be discrete or continuous. We will focus on *discrete-state*, *discrete-time* Markov Chains with a *finite* state space.

**Markov Chain**

A sequence of RVs $X_0, X_1, X_2, ...$ taking values in *state space* $\{1, 2,...,M\}$ is called *Markov chain* $\forall\ n \geq 0$,

$$
P(X_{n+1}=j|X_n=i,X_{n-1}={i-1},...,X_0=i_0) = P(X_{n+1}=j|X_n=i)
$$

$P(X_{n+1}=j|X_n=j)$ is called the *transition probability.* from state $i$ to state $j$. This Markov chain is $time-homogeneous$, which means that $P(X_{n+1}=j|X_n=j)$ is the same $\forall\ n$.

 We can describe the probabilities of moving from state to state using a matrix called *translation matrix* whose $i,j$ entry is probability of going from $i$-th to $j$-th state in a single step.

**Translation matrix**

Let $X_0, X_1, X_2, ...$ be a Markov chain $\{1, 2,...,M\}$ and let $q_{ij}=P(X_{n+1}=j|X_n=i)$ be transition probability from state $i$ to state $j$. The matrix $Q=(q_{ij})$ is the *transition matrix* of the chain. $Q$ is nonnegative and each row sums to $1$.
