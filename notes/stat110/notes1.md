<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>

# 1. Probability and counting
## 1.2.Sample Spaces and Pebble World

The **sample space**  $S$  of an experiment = set of all possible outcomes of the experiment.
Can be finite or infinite.

An **event** $A$  is a subset of the $S$, and we say that  $A$ **occurred** if the actual outcome is in  $A$.

not A = $A^c$

Example:

$A, B \subseteq S$

$A \cup B$ if and only if at least one of $A, B$ occurs.

$A \cap B$ if and only if both of $A, B$.

De Morgan's laws:

$(A \cup B)^c = A^c \cap B^c$ | $A$ OR $B$ not occur = $A$ not occur AND $B$ not occur
$(A \cap B)^c = A^c \cup B^c$ | $A$ AND $B$ not occur = $A$ not occur OR $B$ not occur

##1.3 Naive definition of probability


$$P_{naive}(A) = \frac{|A|}{|S|}$$

Requires $S$ to be finite, with equal mass for each outcome.

## 1.4 How to count

Multiplication rule:

Consider experiment $C$ = 2 sub-experiments $A, B$.
$A$ has $a$ outcomes, $B$ has $b$ outcomes.
Then $C$ has $ab$ outcomes.

Sampling without replacement:

$n$ objects and making $k$ choices from them, one at a time without replacement.
Number of outcomes: $n(n-1)...(n-k+1)$ for $n \le k$ .

A **permutation** of $1,2,...,n$ is an arrangement of them in some order, e.g., 3,5,1,2,4 is a permutation of 1,2,3,4,5.

There are $n!$ permutations of $1,2,...,n$

**Binomial coefficient**: $\binom{n}{k}$ = "$n$ choose $k$" number of subsets of size $k$ for a set of size $n$.
For example, $\binom{4}{2}=6$

For $n \le k$:

$$\binom{n}{k}=\frac{n(n-1)...(n-k+1)}{k!}=\frac{n!}{(n-k)!k!}$$

For $n > k$:

$$\binom{n}{k}=0$$

## 1.5 Story Proofs

Example: **Vandermonde's identity**

$$\binom{n + m}{k}=\sum^k_{j=0}\binom{m}{j}\binom{n}{k-j}$$

Story proof:

Consider a group of  $m$  peacocks and  $n$  toucans, from which a set of size  $k$  birds will be chosen.
There are  $\binom{n + m}{k}$  possibilities for this set of birds. If there are  $j$  peacocks in the set, then there must be  $k−j$  toucans in the set. The right-hand side of Vandermonde's identity sums up the cases for  $j$.
