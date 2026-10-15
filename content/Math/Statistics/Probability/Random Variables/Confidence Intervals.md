# Calculation
## Standard Formula and Intuition
We can estimate a population mean and standard deviation based off the mean of a sample, based off a few points discussed [[Central Limit Theorem and Sampling Random Variables|here]].
As [[Central Limit Theorem and Sampling Random Variables#Mean|mentioned]] the mean of the actual population will be the same as the mean of the distribution of the means of the samples.
Assuming that the sample distributions are normal (see [[Central Limit Theorem and Sampling Random Variables#Getting a Normal Distribution for the Distribution of Sample Means|here]] for the parameters for when we assume that), we can calculate the probability that the sample mean is within 1 standard deviation, or 2 standard deviation, or 2.5 standard deviation, etc. of the mean of the distribution of the means of the samples. And since the mean of the distribution of the means of the samples and the actual population mean are the same, this means that we can calculate the likelihood of how close or how far the sample mean is from the population mean.
For example, approximately 95% of sample means will be within 2 standard deviations of the mean of the distribution of the means of the samples, the same way we know that for any normal distribution, a randomly selected value will be within 2 standard deviations of the mean, as discussed [[Density Curve#Empirical Rule (68-95-99.7 Rule)|here]]. In other words, the sample mean of a random sample will be within 2 standard deviations of the mean of the distribution of the sample means 95% of the time. And since the mean of the distribution of the sample means is the same as the population mean, the sample mean of a random sample will be within 2 standard deviations of the population mean. This means that if we can calculate the standard deviation, we will be able to calculate a range for the population proportion (with a certain degree of confidence).
However, the [[Central Limit Theorem and Sampling Random Variables#Standard Deviation|formula for calculating the standard deviation of the distribution of the samples]] is based on the actual population standard deviation and we don't know that.
However, we can estimate the population standard deviation using the sample, as discussed [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Steps to Find Sample Variance (s 2)|here]]. We will use that in our formula in place of the population standard deviation to calculate an estimate of the standard deviation of the distribution of the sample means. This estimate of the standard deviation of the distribution of the sample means is called the standard error.
We can use this to calculate a range of possibilities for the population proportion. For example, if we knew that our estimate was an accurate measure of the actual standard deviation of the distribution of the sample means and we wanted to create a range that we would know that the population proportion would be part of with 95% confidence, we would need to calculate around two standard errors above and below the sample mean (as seen from a [[Density Curve#Z-Table|z-table]]).
However, we don't know that our estimate for the standard deviation of the distribution of the sample means is accurate. While we did use Bessel's Correction (see [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Steps to Find Sample Variance (s 2)|here]]) that just makes the estimate *unbiased*. In other words, if we kept taking sets of samples and measuring the standard deviation of the means, the *average* of the standard deviations would be the same as the true standard deviation of the population standard deviation. However, for any individual set of samples, the standard deviation of that set may not accurately measure the standard deviation of the population, eve with Bessel's correction. It can be too high or too low. To account for this, we use a [[T-Score|t-score]] and t-table. This is similar to a z-table and z-score, except this accounts for the fact that we don't actually know the true standard deviation. The way it accounts for this is by assuming that the data is more spread out from the mean than by a z-table. How many standard deviations we need is called the z critical-value. The standard error multiplied by the z critical-value is called the margin of error.
The larger the sample size, the smaller the standard deviation is going to be ($n$, or the sample size, is in the denominator of the fraction). This means that if we want to make the standard deviation smaller (and hence, the estimate of the population proportion to be more specific) we need to increase the sample size. ^59e303
### Formula
The formula is going to come out to be:
$$\text{Standard Error}=\sqrt{\frac{\sum^n_{i=1}(x_i-\bar{x})^2}{n-1}}$$
(Where $n$ is the amount of samples taken and $\bar{x}$ is the average of the sample.)

$$\text{Margin of Error}= \text{SE} \times z^*$$
($z^*$ is the z critical-value.)

$$\text{Confidence Interval} = \bar{x} \pm \text{MoE}$$
## "Shortcut" for Bernoulli Random Variables
The standard deviation for a Bernoulli random variable is $\sqrt{p(1-p)}$. As discussed [[Bernoulli Trial#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance and Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|here]], this is simplified from the regular standard deviation formula (getting the distances from the mean, squaring them, adding them together, dividing by $n$, and getting the square root). However, this assumes that we are dividing by $n$. In our situation, we are estimating the standard deviation of the population from the sample and so we have to use $n-1$ (Bessel's Correction) as [[#^59e303|just discussed]]. Technically, this simplification to $\sqrt{p(1-p)}$ does not work in this situation. However, if the sample is large, the difference between $n$ and $n-1$ becomes very small and so, in most situations, the difference will not matter. As such, one can use $\sqrt{p(1-p)}$ as the standard deviation of the Bernoulli random variable (and use that as an estimate of the population standard deviation).
## Minimum Sample Size to Achieve a Desired Confidence Interval and Margin of Error for Bernoulli Trials
Let's say you want to have a certain confidence interval, and you also want the margin of error to be under a certain size. To guarantee that this will happen, there is a minimum sample size that you will need.
(Keep in mind that the larger the confidence interval and the smaller the margin of error, the larger the sample size will need to be.)

This can be calculated based on the margin of error formula. As stated above, the formula for the margin of error is $\text{SE} \times z^*$. And for a Bernoulli Trial, we can say that the standard error is $\sqrt{\frac{\hat{p}(1-\hat{p})}{n}}$ ($\hat{p}$ is the sample proportion, which is basically the same thing as the sample mean but specifically for Bernoulli Trials). The margin of error is $\sqrt{\frac{\hat{p}(1-\hat{p})}{n}} \times z^*$. So a way of thinking about this is:
$$\text{Desired MoE} \le \sqrt{\frac{\hat{p}(1-\hat{p})}{n}} \times \text{Desired } Z^*$$
We have to be concerned about the "worst case scenario", which would be the value for the sample proportion (or $\hat{p}$) that would make the MoE the maximum possible value it could be. This is going to be $\hat{p}=.5$.
From this point, we just need to do algebra to find the value of $n$.
It may come out that once we take out sample, we find that the sample proportion is less than or greater than .5 and so the MoE is actually less than the desired MoE. That is fine; the desired MoE was the maximum amount. It is fine if it is less.
For example, let's say I wanted my MoE to be no more than 3% and I wanted to be 95% confident, this is what the formula would look like:
$$.03 \ge \sqrt{\frac{.5*(1-.5)}{n}} * 1.96$$
(As discussed above, we assume the "worst case scenario that $\hat{p}$ is .5. The z critical-value for a 95% confidence is 1.96)

Dividing both sides by 1.96 and simplifying a bit we get:
$$\frac{.03}{1.96} \ge \sqrt{\frac{.5*.5}{n}} \Rightarrow \frac{.03}{1.96} \ge \frac{.5}{\sqrt{n}}$$

Multiplying both sides by 2 we get:
$$2 \times \frac{.03}{1.96} \ge 2 \times \frac{.5}{\sqrt{n}} \Rightarrow \frac{.06}{1.96} \ge \frac{1}{\sqrt{n}}$$

We then flip to the reciprocals. When we do this, the greater than/less than sign changes direction:
$$\frac{.06}{1.96} \ge \frac{1}{\sqrt{n}} \Rightarrow \frac{1.96}{.06} \le \sqrt{n}$$

Squaring both sides, we get:
$$ n \ge \boxed{1067.111}$$

So to guarantee that we will get no greater than $\pm3\%$ and we wanted to be 95% confident, we would need a minimum sample size of 1068 people.
(As discussed above, this is assuming the worst-case scenario that the population proportion is .5. When you actually take the sample, if you discover that the population proportion is not .5, your margin or error will actually be lower.)
### Some Practical Points about Required Minimum Sample Size
This formula only works for Bernoulli random variables because we know that the highest variance occurs at .5. For non-Bernoulli random variables, there is technically no maximum variance. However, in most real-life situations, either you can estimate a maximum variance, or you may have some sort of previous pilot study that you can use to give you a feel for what the max is.
And even when it comes to Bernoulli random variables, you may know from your own estimates or from previous pilot studies that the population proportion is not .5. In that case, you can take a smaller sample.
## Sampling from a Finite Population (Finite Population Correction)
When sampling something, we will usually be sampling from a population with finite size (for example, we may be sampling voting patterns in a certain population. There are a finite amount of people in that population) and we are not going to be replacing the people that we sample (in the above example, once we ask someone how they are voting, we are not going to ask them again). This allows us to get get even tighter confidence intervals.
Intuitively, this makes sense. If there are 100 people in our population and we sample all 100 of them, we know with 100% certainty the exact distribution. There is no "range of values" or "degree of confidence".
Similarly, even if we don't sample everyone, the greater percentage of the population we sample, the less the means of samples can move around.
For example, let's say I have a population of 100 people and I sample 94 of the them and I get 47 successes and 47 failures, I know that the population can range from 53 successes against 47 failures, to 47 successes against 53 failures. And I also know that the extremes are unlikely as it is very unlikely that all of the people I didn't sample happened to all be the same thing (in this example where the population proportion is basically 50/50. It's basically as likely as flipping 6 heads or 6 tails in a row). In other words, because we basically sampled the whole population, the standard error is going to be very small.
### Formula
One takes this into account by multiplying the standard error by the Finite Population Correction formula. This is:
$$\text{FPC} = \sqrt{\frac{N-n}{N-1}}$$
*($N$ is the population size and *n* is the sample size.)*
### Some Intuition with Examples
As $N$ increases compared to $n$, the less of a difference $n$ makes. For example, let's say $N=10000$ and $n=10$, this is going to equal:
$$\sqrt{\frac{10000-10}{10000-1}} = \sqrt{\frac{99990}{99999}} \approx \sqrt{.99991} \approx \boxed .99995$$
As can be seen, this basically equals $1$. When me multiply the standard error by this number, it basically won't change. The fact that this population is finite doesn't really help us get a more precise estimate.
Conversely, as $n$ approaches the size of $N$, this will approach $0$. For example, let's say that $N=10000$ and $n=9500$, this becomes:
$$\sqrt{\frac{10000-9500}{10000-1}} = \sqrt{\frac{500}{9999}} \approx \sqrt{.05} \approx \boxed{.223}$$
In other words, we can shrink the standard error by nearly 80%. And if $n$ is even closer to $N$, the effects get stronger. For example, if $N=10000$ and $n=9990$, this becomes:
$$\sqrt{\frac{10000-9990}{10000-1}} = \sqrt{\frac{10}{9999}} \approx \sqrt{.001} \approx \boxed{.032}$$
And if $N$ and $n$ are equal, the fraction will equal $0$. The numerator is $N-n$. If $N$ and $n$ are equal, this will equal $0$. In other words, there will be no error at all. We will have the exact population proportion.
### 10% Rule of Independence
There is a "rule of thumb" that if the sample size is 10% or less than the population size, we ignore the finite population correction. At such a small percentage, correcting for the fact that we are dealing with a finite population will barely make a difference which is barely worth it in most real-life situations.
# Example
We take a random sample of 100 people from a certain population and 75% say that they like vanilla ice cream and 25% say that they do not. We want to try and calculate a confidence interval with 95% confidence for what the population proportion is.
## Using the "Shortcut"
*Note: We are only able to use the shortcut because this is a Bernoulli random variable. This does not work for non-Bernoulli random variables.*

The sample proportion is .75, so the variance of the sample is:

$$.75 \times (1-.75)$$

To calculate the standard error, we use this in place of the population variance to calculate the standard deviation of the distribution of the means of samples. As [[#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance And Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation#formula|discussed above]], we just need to divide by $n$ (which is 100) and then take the square root, like so:
$$\sqrt{\frac{.75 \times (1-.75)}{100}} \Rightarrow \sqrt{\frac{.75 \times .25}{100}} \approx \boxed{.043}$$
Now that we have our standard error, we need to calculate two standard errors above and below the sample proportion (our margin of error) and we will have a range of different values for the population proportion (with 95% certainty).
This becomes:
$$.75 + (.043 *2) \Rightarrow .75 + (.086) = \boxed{.836}$$
$$.75 - (.043*2) \Rightarrow .75 - (.086) = \boxed{.664}$$
We can say with 95% confidence that between 67.4% and 83.6% of people in this population like vanilla ice cream.
As noted, if we want to make this range smaller, we would have to get a larger sample.
For example, let's say we sampled 250 people and got 75% of people who said that they liked vanilla ice cream, the standard error would be:
$$\sqrt{\frac{.75 \times (1-.75)}{250}} \Rightarrow \sqrt{\frac{.75 \times .25}{250}} \approx \boxed{.027}$$
Two standard errors above and below would become:
$$.75 + (.027 *2) \Rightarrow .75 + (.054) = \boxed{.804}$$
$$.75 - (.027 *2) \Rightarrow .75 - (.054) = \boxed{.696}$$
In this case, we know with 95% certainty that the population proportion is between 69.6% and 80.4%.
## Using the "Regular" Method
We are trying to estimate the standard deviation of the population from a sample. As such, we have to get the square root of the squared distance of every sample from the mean, but then, instead of dividing by the sample size (to get the real average and the standard deviation for the sample we took), we divide by $n-1$, as discussed.
"Successes" are considered a $1$ and failures are a $0$. The mean is simply $p$, which in this case is $.75$.
There are $75$ successes and $25$ failures. We need to calculate the squared distance from the mean for each of these and add them together. For the successes, that becomes:
$$75 \times \left((1-.75)^2\right)$$
And for the failures:
$$25 \times \left((0-.75)^2\right)$$
We then add these together:
$$75 \times \left((1-.75)^2\right) + 25 \times \left((0-.75)^2\right) = 18.75$$
If we wanted to get the standard deviation of the sample, we would then divide this by the sample size. However, because we are using this as an estimate of the population standrad deviation, we divide this by $n-1$, as discussed. This becomes:
$$\frac{18.75}{100-1} \approx .189$$
Now we need to get the square root of this:
$$\sqrt{.189}= \boxed{.435}$$
This number is our approximation of the standard deviation of the population.
We can take this number and plug it into the formula for getting the standard deviation of the distribution of the means of samples. As discussed above, the formula is $\frac{\sigma}{\sqrt{n}}$. Plugging in the numbers, we get:
$$\frac{.435}{\sqrt{100}} \Rightarrow \frac{.435}{10} \approx \boxed{.044}$$
Since we are looking for 95% confidence, we need calculate 2 standard deviations above and 2 standard deviations below to create the range. For the upper bound, this is:
$$.75+(.044 \times 2) = \boxed{.838}$$
And for the lower bound:
$$.75-(.044 \times 2) = \boxed{.662}$$

As can be seen, using the "shortcut" resulted in nearly the exact same value as the "regular" method. They are approximately $.001$ apart.