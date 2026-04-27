<span style="color:rgb(255, 0, 0)">Perhaps I should combine this with [[Central Limit Theorem and Sampling Random Variables#Distribution of Samples from Original Distribution (Sampling Distribution)]] as they are really the same rules. The only difference is that over here, I apply the rules to binomials specifically, while over there I write the rules more generically for Random Variables.</span>
*For sampling a non-binomial Random Variable, see [[Central Limit Theorem and Sampling Random Variables#Distribution of Samples from Original Distribution (Sampling Distribution)|here]].*
# Definition
Taking the sample of a binomial-type random variable is similar to taking the [[Binomial|binomial]]. The slight difference is that with a binomial, we measure the total amount of successes and failures. When it comes to sampling, we want to measure the ratio of successes and failures.
For example, if I have a large bucket of red marbles and blue marbles, if I was discussing the amount of red of blue marbles I would pick out, I would be discussing a binomial. If I was discussing the ratio of red or blue marbles I would pick out, I would be discussing taking a sample.
# Formulas
## Expected Value (Average, Population Proportion)
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
When dealing with sampling, we are dealing with the ratio of successes to total trials, not simply the total successes. As discussed [[#Expected Value (Average, Population Proportion)|just before]], samples will be the $\frac{amount \space of \space success}{number \space of \space trials}$.
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
In other words, the larger the sample size, the samples will get closer and closer to the proportioncted value.
# Distributions
The distribution of samples taken from a population will look different depending on the true probability of the metric being sampled as well as the size of the sample.
As the probability approaches 100%, the mean (which is equal to the probability, as [[#Expected Value (Average, Population Proportion)|discussed]]) will move toward 100%, as well. However, the distribution will begin to skew left, meaning, that there will be a tail extending to the left, as discussed [[Density Curve#Skewed Distribution|here]]. Conversely, as the probability approaches 0%, the mean moves that way as well and the distribution will have a tail extending to the right (it will skew right).
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
For example, let's say that a certain event has a 90% probability and we take 10 samples. The probability distribution for the ratio of successes looks like this (there are two graphs, but the represent the same data.):
![[Pasted image 20260126221627.png]]
![[Pasted image 20260126221706.png]]
As can be seen, the data has a long tail to the left. There isn't a lot of "room" for data above the mean (which is at 90% successes, or 9 successes).
Here is the data when we run 100 trials (once again, with two graphs):
![[Pasted image 20260126221840.png]]
![[Pasted image 20260126221853.png]]
Over here, the graph looks like a normal distribution. Because there is a much larger sample size, the data is much tighter around the mean (90%, or, in this case, 90 successes). There is enough "room" above the mean.
(Side note: even though in these graphs it looks like the probability of getting a value toward the left is 0, that is certainly not actually the case. The probability is low, but it is impossible for it to be 0. The reason it looks that way is because the scale of the graph is too large. If we would make the scale of the graph smaller, the probabilities would be seen.)
# Calculating at Least/Most a Certain Percentage
Assuming that the distribution is normal (as [[#The "Normal Distribution Rule"|discussed]]), we can calculate what percentage of the data will be above or below a certain percentage.
To do this, we would need to calculate the mean, which can be calculated as [[#Expected Value (Average, Population Proportion)|discussed]] and the standard deviation, which also can be calculated as [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|discussed]].
We then need to see how many standard deviations the amount we are looking for is away from the mean, and then we would use a [[Density Curve#Z-Table|z-table]] to be able to make the calculation that we are looking for.
See [[Binomial#At Least $x$ Amount|here]] for more details.
# Calculating Population Proportion from Sample Proportion (Confidence Intervals)
We can estimate a population proportion based off the proportion of a sample, based off a few points previously discussed.
As mentioned [[Central Limit Theorem and Sampling Random Variables#Distribution of Samples from Original Distribution (Sampling Distribution)#Mean|here]], the proportion of the actual population will be the same as the proportion of the distribution of the samples.
Assuming that the sample distributions are normal (as discussed [[Central Limit Theorem and Sampling Random Variables#Shape of Sampling Distribution|here]] and [[Sampling a Binomial-Type Random Variable#The "Normal Distribution Rule"|here]]), we can calculate the probability that the sample proportion is with 1 standard deviation, or 2 standard deviation, or 2.5 standard deviation, etc. of the mean of the distribution of the samples. And since the proportion of the distribution of the samples and the actual population proportion are the same, this means that we can calculate the likelihood of how close or how far the sample proportion is from the population proportion.
For example, we know with 95% confidence that the sample proportion is within approximately 2 standard deviation of the population proportion, as discussed [[Density Curve#Empirical Rule (68-95-99.7 Rule)|here]].
This means that if we can calculate the standard deviation, we will be able to calculate a range for the population proportion (with a relatively high degree of confidence).
However, the formula for calculating the standard deviation of the distribution of the samples is based actual population proportion (as discussed [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation#formula|above]]) and we don't know that (that is what we are trying to figure out).
However, we do have a rough estimate of what the population proportion is, and that is the sample proportion. We will use that in our formula in place of the population proportion to calculate an estimate of the standard deviation. This estimate of the standard deviation is called the standard error.
Once we have calculated the standard error, we can use that as an estimate of the standard deviation. We can use this to calculate a range of possibilities for the population proportion. For example, if we wanted to create a range that we would know that the population proportion would be part of with 95% confidence, we would need to calculate around two standard errors above and below the sample proportion. This is called the margin of error (meaning, the standard error multiplied by how many standard errors we would like to be able to achieve our degree of confidence).
As can be seen from the [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation#formula|formula for calculating the standard deviation]], the larger the sample size, the smaller the standard deviation is going to be ($n$, or the sample size, is in the denominator of the fraction). This means that if we want to make the standard deviation smaller (and hence, out estimates of the population proportion to be more specific) we need to increase the sample size.
## Example
We take a random sample of 100 people and 75% say that they like vanilla ice cream and 25% say that they do not. We want to try and calculate a confidence interval with 95% confidence for what the population proportion is.
We start by calculating the standard error. The sample proportion is .75, so we just plug that into the [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation#formula|standard deviation formula]] like so:
$$\sqrt{\frac{.75 \times (1-.75)}{100}} \Rightarrow \sqrt{\frac{.75 \times .25}{100}} \approx \boxed{.043}$$
Now that we have our standard error, we need to calculate two standard errors above and below the sample proportion (our margin of error) and we will have a range of different values for the population proportion (with 95% certainty).
This becomes:
$$.75 + (.043 *2) \Rightarrow .75 + (.086) = \boxed{.836}$$
$$.75 - (.043*2) \Rightarrow .75 - (.086) = \boxed{.664}$$
We can say with 95% confidence that between 67.4% and 83.6% of people  like vanilla ice cream.
As noted, if we want to make this range smaller, we would have to get a larger sample.
For example, let's say we sampled 250 people and got 75% of people who said that they liked vanilla ice cream, the standard error would be:
$$\sqrt{\frac{.75 \times (1-.75)}{250}} \Rightarrow \sqrt{\frac{.75 \times .25}{250}} \approx \boxed{.027}$$
Two standard errors above and below would become:
$$.75 + (.027 *2) \Rightarrow .75 + (.054) = \boxed{.804}$$
$$.75 - (.027 *2) \Rightarrow .75 - (.054) = \boxed{.696}$$
In this case, we know with 95% certainty that the population proportion is between 69.6% and 80.4%.