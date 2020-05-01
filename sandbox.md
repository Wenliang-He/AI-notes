
### Random Variable vs. Case

Test it $f(k) = {n \choose k} p^{k} (1-p)^{n-k}$ and see how it renders

$$f(k) = {n \choose k} p^{k} (1-p)^{n-k}$$



|| Random Variable(s) | Case(s) |
|---|---|---|
| is a | concept | instance |
| is a | probabiilty distribution | number |
| comprise a | population | sample |
| with sample size | $n = \infty$ or all data | $n$ is finite or some data |
| comprise a | probability distribution | empirical spread/distribution |
| comprise a | random sample | sample |
| give rise to a | sampling statistic | sample statistic |

### Properties of a Random Variable

Previously, we have $Y_1, Y_2, Y_3, ..., Y_n \overset{iid}{\sim} N(0,1)$ and $\bar{Y} = \frac{1}{n} \sum_{i=1}^{n} Y_i$, where both $Y_i$s and $\bar{Y}$ are random variables. In practice, we would encounter a variety of random variables. As a result, we would constantly ask the questions:

- What does a RV look like?
- What is the distribution of a RV?
- What are the properties of a RV?
    - center of a RV or $E(RV)$
    - spread of a RV or $Var(RV)$
    - shape of a RV or $shape(RV)$

The first two questions are identical. The first one is using informal language and the second using formal academic language. The two questions are reduced to the third question, which is basically asking for a quick summary of a distribution in terms of the _center_, _spread_, and _shape_. 

The properties of a RV can be succintly summarized as 

$$Y \sim \forall(\mu, \sigma^2) $$
where $\forall$ stands for **_any_**. Notice $\forall$ is just an inverted **A**. 


## Central Limit Theorem 

**Central Limit Theorem** or **CLT** is the singularly most important theorem in statistics. CLT forms the foundation of **statistical inference**, a subject of perpetual interest in statistics. 

### Presenting Central Limit Theorem

1. Given a random variable Y of **any shape** with mean $\mu$ and variance $\sigma^2$,

$$Y \sim \forall(\mu,\sigma^2)$$

2. We choose a random sample from Y
$$Y_1, Y_2, Y_3, ..., Y_n ~ \overset{iid}{\sim} ~ \forall(\mu,\sigma^2)$$
where each $Y_i$ is a random variable with $E(Y_i) = \mu$ and $Var(Y_i) = \sigma^2$. 

3. We can compute the sampling statistic of the sample mean
$$\bar{Y} = \frac{1}{n} \sum_{i=1}^{n} Y_i$$
where $\bar{Y}$ becomes another random variable. 

4. Hence, we would immediately ask the question: What are the properties of $\bar{Y}$?

The answer to this question gives birth to the singularly most important theorem in statistics, known as the **_Central Limit Theorem_** or **CLT**. See the proof of part of the theorem below.

**Answers**:
$$\bar{Y} \sim N \left( \mu, \frac{\sigma^2}{n} \right)$$
or equivalently

- $E(\bar{Y}) = \mu$
- $Var(\bar{Y}) = \sigma^2 / n$
- $shape(\bar{Y}) = N$

The most surprising part of the CLT is the discovery that given a random variable $Y$ of **any** distribution, $\bar{Y}$ is **always** normally distributed as long as two conditions are satisfied:

1. $Y_1, Y_2, Y_3, ..., Y_n ~ \overset{iid}{\sim} ~ \forall(\mu,\sigma^2)$
2. sample size n is large enough


`Proof - Prerequisites`:

- $E(cX) = c E(X)$
- $E(X+Y) = E(X) + E(Y)$
- $E(cX) = c^2E(X)$
- $Var(X+Y) = Var(X) + Var(Y)$ if $X \perp Y$, i.e., X is independent of Y




