# 2. Conditional Probability and Bayes' Rule

$$
P(A|B) \neq P(B|A)
$$

How should we update our beliefs in light of the evidence we observe? *Bayes' rule* is an extremely useful theorem that helps us perform such updates.

Together, Bayes' rule and the law of total probability can be used to solve a very wide variety of problems.

## 2.1 The importance of thinking conditionally

A useful perspective is that all probabilities are *conditional*

$A$ and $B$ events, $P(B) > 0$, then *conditional probability* of A given B:

$$
P(A|B)=\frac{P(A \cap B)}{P(B)}
$$

 $A$ is the event whose uncertainty we want to update, and B is the evidence we observe.

$P(A)$ is called *prior probability* of $A$.

$P(A|B)$ is called *posterior probability* of $A$.

$P(A|B)$ is the probability of $A$ given the evidence $B$, **not** the probability of some weird entity called $A|B$.
