# Definition
A Bernoulli Trial is a [[Binomials|binomial]], but we focus on only one instance of the trial.
For example, getting a heads in a single coin flip, spinning a six with a standard six-sided die, or whether it will rain tomorrow are all Bernoulli Trials.
# [[Expected Value]] (Average)
The expected value (or average) of a Bernoulli Trial is the probability. It is the likelihood of getting the specific result over time.
For example, the expected value of getting heads (or tails) for a regular coin flip is $\frac{1}{2}$.
The expected value of spinning a six (or any other number) for a regular die roll is $\frac{1}{6}$.
The expected value of whether it will rain tomorrow or not depends on where you live, what time of the year it is, and things like that.
## Proof
As with binomials, we generally refer to getting the "successful result" as $1$ and not getting it as $0$.
The way to calculate the mean is to add up all of the values and divide them by the total. Over here, we don't actually have any specific values; we just have the probability of whether it will occur. As such, the way to calculate the mean is by multiplying the probability of getting a "failure" by $0$ (the number we ascribe to "failure") and the probability of getting a "success" by $1$ (the number we ascribe to "success").
As such, we get:
$$(1-p) \times 0 + p \times 1 \Rightarrow p \times 1 = \boxed{p}$$
Where $p$ is the probability of getting "success". Because there are only two possibilities, if $p$ is the probability of getting a success, then $1-p$ is the probability of getting a failure, because the probability of getting success or failure must equal $100\%$, or $1$ (everything, or $100\%$ of things, must be either success or failure, because those are the only possibilities).
As such, if the probability of success is $p$, the probability of failure must be $1-p$ so together they equal $1$ ($1=p+1-p$. The $p$ and $-p$ cancel out and you are left with $1=1$).
# [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]] and [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]]
## Variance
### Formula
The formula for getting the variance is $\boxed{p(1-p)}$
### Proof
The variance is the average of the squared distances from the mean.
As said above, the mean is $p$.
We want to get how far the "failure" is from the mean, and the success is from $p$, and we want to weight them by how common they are (similar to what we just did when calculating the mean, we used the probability of getting a success or a failure), and then need to square these values and add them together.
Starting with the "failure", a "failure" is $0$, so its distance from the mean is $0-p$ (because $p$ is the mean). Then we need to square it (because we are getting the squared distance from the mean) and then we need to get how common it is. As discussed earlier, the probability of getting a failure is $1-p$. Putting that all together we get $(1-p)(0-p)^2$.
Now for the "success", a "success" is $1$, so its distance from the mean is $1-p$ (because $p$ is the mean). Then we need to square it (because we are getting the squared distance from the mean) and then we need to get how common it is. As discussed earlier, the probability of getting a success is $p$. Putting that all together we get $p(1-p)^2$.
Now putting them both together we get:
$$(1-p)(0-p)^2 + p(1-p)^2$$
Writing out the terms that are squared we get:
$$(1-p)p^2 + p(p^2-2p+1)$$
Now using the distributive property on the parentheses we get:
$$p^2-p^3+p^3-2p^2+p$$
Simplifying, the $p^3$ and $-p^3$ cancel out. In addition, we can add the $p^2$ to the $-2p^2$. Then we can simplify. That comes out to:
$$-p^2+p = \boxed{p(1-p)}$$
## Standard Deviation
### Formula
The standard deviation is the square root of the variance. As such, the standard deviation is $\boxed{\sqrt{p(1-p)}}$.