# Definition
Sampling is very similar to a [[Binomial|binomial]]. We have a specific amount of trials, the trials have the same probability, and there are two possible outcomes.
The slight difference is that with a binomial, we measure the total amount of successes and failures. When it comes to sampling, we want to measure the ratio of successes and failures.
For example, if I have a large bucket of red marbles and blue marbles, if I was discussing the amount of red of blue marbles I would pick out, I would be discussing a binomial. If I was discussing the ratio of red or blue marbles I would pick out, I would be discussing taking a sample.
# Formulas
## Expected Value (Average)
### Formula
The formula for the expected value is simply the probability, or $p$.
### Proof
The expected value for a binomial is $np$, as discussed [[Binomial#Random Variable Expected Value (Average) Expected Value (Average)|here]].
Since we are discussing sampling, we are trying to calculate the ratio of successes to the total. This would be:
$$\frac{Amount \space of \space successes}{Total \space trials}$$
As just mentioned, the average amount of the total successes is $np$.
The total amount of trials is $n$.
As such, we get:
$$\frac{np}{n} = p$$
This intuitively makes sense. Let's say I have 10,000 marbles in a bucket and 8000 of them are red, we would expect to pull a red marble out 80% (or .8) of the time.
## [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]] And [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]]
### Formula
The formula for the variance is $\frac{p(1-p)}{n}$ and the formula for the standard deviation is $\sqrt{\frac{p(1-p)}{n}}$ or $\frac{\sqrt{np(1-p)}}{n}$.
### Proof
As discussed [[Binomial#Variance|here]], the formula for getting the variance is a binomial distribution is $np(1-p)$.
When dealing with sampling, we are dealing with the ratio of successes to total trials, not simply the total successes. As discussed [[#Expected Value (Average)|just before]], samples will be the $\frac{amount \space of \space success}{number \space of \space trials}$.
When getting the variance of binomials, we are getting the variance of the amount of successes that we have for each set of trials. When getting the variable of samples, we are getting the variance of the amount of successes *divided by the amount of trials*. In other words, the difference between the values of the binomials and the samples is that every one of the sample values is the binomial value divided by $n$.
For example, if I have 8,000 red marbles and 2,000 non-red marbles in a bucket and I pick 10 out, and I do this 5 times, I may get the 6, 8, 6, 9, and 7 "successes".
If I viewed these as samples, I get $\frac{6}{10}$, $\frac{8}{10}$, $\frac{6}{10}$, $\frac{9}{10}$, and $\frac{7}{10}$ ratio of successes to total trials. In other words, in this example, the values of the samples are the same as the values of total successes divided by 10.
When all of the values are divided by $x$, the value of the variance will be $\frac{1}{x^2}$ of the original variance and the standard deviation will be $\frac{1}{x}$ of the original standard deviation, as discussed [[Adjusting and Combining Random Variables#Multiplying Constant to Random Variables|here]].
As such, the variance becomes:
$$np(1-p) \times \frac{1}{n^2} \Rightarrow \frac{np(1-p)}{n^2} \Rightarrow \boxed{\frac{p(1-p)}{n}}$$
The standard deviation becomes:
$$\sqrt{np(1-p)} \times \frac{1}{n} \Rightarrow \boxed{\frac{\sqrt{np(1-p)}}{n}}$$
Or we can simplify it further by dividing the $\sqrt{n}$ in the numerator by the $n$ in the denominator to get:
$$\frac{\sqrt{np(1-p)}}{n} \Rightarrow \frac{\sqrt{p(1-p)}}{\sqrt{n}} \Rightarrow \boxed{\sqrt{\frac{p(1-p)}{n}}}$$
# Larger Samples
Based on the formulas, a larger sample will not change the expected value for a sample. This makes intuitive sense. If I take a bunch of samples of 10 marbles and a bunch of samples of 100 marbles, the average amount of "successes" should be the same.
However, a larger sample will make the variance and standard deviation shrink. The formulas for the variance and the standard deviation are basically $\frac{Lots \space of \space stuff}{n}$, so as $n$ increases, the variance and standard deviation decreases.
In other words, the larger the sample size, the samples will get closer and closer to the mean.
# Distributions
The distribution of samples taken from a population will look different depending on the true probability of the metric being sampled as well as the size of the sample.
As the probability approaches 100%, the mean (which is equal to the probability, as [[#Expected Value (Average)|discussed]]) will move toward 100%, as well. However, the distribution will begin to skew left, meaning, that there will be a tail extending to the left, as discussed [[Density Curve#Skewed Distribution|here]]. Conversely, as the probability approaches 0%, the mean moves that way as well and the distribution will have a tail extending to the right (it will skew right).
However, if we use a large enough sample size, the distribution will still look more or less like a [[Density Curve#Normal Distribution|normal distribution]].
The idea is as follows: when we have a small sample size, there is a large variance and standard deviation (as [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|discussed]]) or, in other words, the samples will not be close to the mean. As the probability goes higher or lower, the highest part of the distribution moves along with it. The closer it gets to one side or the other, the "less room" there is for the samples which are far from the mean. And since there are a relatively large amount of samples which are far from the mean, most of the samples which are far from the mean are going to be on the "roomier" side.
For example, if I have a population that has a 80% probability of something and I take samples that have a sample size of 5, the most common amount of "successes" I would get in a sample is $\frac{4}{5}$. However, there would be far more samples that have 0, 1, 2, or 3 successes than 5 successes, and so the distribution curse would peak at .8, but then have a large tail to the left.
As the sample size increases, the results become closer to the mean, and so there is still enough "space". For example, if I have take samples that have a sample size of 1000 instead, the vast majority of my samples will be right around $\frac{800}{1000}$. There is enough "room" around the mean to fit most of the results. There will still be a tail to the left as there will be some extreme results, but the tail will be relatively small, and the resulting distribution will look similar to a norms distribution.
## The "Normal Distribution Rule"
The "rule" (it's not a hard-and-fast rule, but it is generally considered this way amongst statisticians) for deciding if we view the distribution as normal or not is if the following two things are true:
$$(sample \space size) \times (probability) \ge 10$$
and:
$$(sample \space size) \times (1-probability) \ge 10$$
This is generally just written as:
$$np \ge 10$$
and:
$$n(1-p) \ge 10$$
The basic intuition is as we said before: the more likely or less likely something is, the more the mean moves in one direction or the other, and the "less room" there is for the data to on the "small size". This will make the distribution "have a tail".
However, if we have a larger sample size, the data "tightens up" around the mean and so there is enough room to fit the data. This makes the graph look normal.
For example, let's say that a certain event has a 90% probability and we take 10 samples. The probability distribution for the ratio of successes looks like this (there are two graphs, but the represent the same data. I just put them both because either one may be easier to visualize):
![[Pasted image 20260126221627.png]]
![[Pasted image 20260126221706.png]]
As can be seen, the data has a long tail to the left. There isn't a lot of "room" for data above the mean (which is at 90% successes, or 9 successes).
Here is the data when we run 100 trials (once again, with two graphs):
![[Pasted image 20260126221840.png]]
![[Pasted image 20260126221853.png]]
Over here, the graph looks like a normal distribution. Because there is a much larger sample size, the data is much tighter around the mean (90%, or, in this case, 90 successes). There is enough "room" above the mean.
# Calculating at Least/Most a Certain Percentage
Assuming that the distribution is normal (as [[#The "Normal Distribution Rule"|discussed]]), we can calculate what percentage of the data will be above or below a certain amount.
To do this, we would need to calculate the mean, which can be calculated as [[#Expected Value (Average)|discussed]] and the standard deviation, which also can be calculated as [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|discussed]].
We then need to see how many standard deviations the amount we are looking for is away from the mean, and then we would use a [[Density Curve#Z-Table|z-table]] to be able to make the calculation that we are looking for.
See [[Binomial#At Least $x$ Amount|here]] for more details.
