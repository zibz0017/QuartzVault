# Definition
Sampling is very similar to a [[Binomial|binomial]]. We have a specific amount of trials, the trials, have the same probability, and there are two possible outcomes.
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