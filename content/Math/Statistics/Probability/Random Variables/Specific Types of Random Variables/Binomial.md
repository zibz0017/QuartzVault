# Definition
Binomials are a specific type of [[Random Variable|random variable]] that has the following rules:
1. There are only two possible outcomes.
2. There must be a defined number of events.
3. The probability for each outcome in each event is the same.
## Example
The amount of heads after flipping a coin 10 times (ignoring the fact that the coin can technically land on its side).
This checks all of the boxes: there are two possible outcomes, there are a defined number of events, and the probability of each event is the same.
# Calculation
## Getting $x$ Amount in 50/50 Events
Let's say we want to figure out the odds of getting exactly 3 heads in 5 coin flips. The way we would calculate is simply:
$$\frac{All \space possible \space ways \space of \space getting \space 3 \space heads \space in \space 5 \space flips}{All \space possible \space ways \space of \space flipping \space a \space coin \space 5 \space times}$$
We can figure out all of the possible ways of flipping a coin 5 times. For every coin flip I take, the amount of possibilities doubles. As such, for 5 coin flips, I have $2^5=32$ coin flips.
To calculate the amount of ways of getting 3 heads in 5 flips, we can think about this is the following way: We have numbers 1-5 lined up and each number represents a flip (1 represents the 1<sup>st</sup> flip, 2 represents the 2<sup>nd</sup> flip, etc.) and we are "selecting" flips to a group that will be heads. Any flip that we select will be heads and any we don't will be tails.
Coming back to our example, we are trying to figure out how many different combinations we can make of 3 flips that we select in the "heads" group. To calculate this, we can use the [[Combinations|combinations formula]]. This is exactly what a combination is. A combination is the amount of ways we can select a specific number of things to a group from a different group. That is what we are doing: we are figuring out the amount of ways we can select a certain number of flips to be part of out "heads" group from the total number of flips.
The formula is:
$$\frac{(Total \space amount \space of \space things)!}{(Amount \space of \space things \space we \space are \space choosing)! \times (Amount \space of \space things \space we \space are \space not \space choosing)!}$$
Plugging in the values, we get:
$$\frac{5!}{3!(5-3)!} \Rightarrow \frac{5!}{3! \times 2!} \Rightarrow \frac{120}{6 \times 2} \Rightarrow \frac{120}{12} = \boxed{10}$$
In other words, there are 10 different ways we can flip a coin 5 times and end up with 3 heads.
Going back to the original question, there are 10 ways to flip a coin 5 times and end up with exactly 3 heads, and there 32 different possible ways of flipping a coin 5 times. As such, the odds of flipping a coin and getting exactly 3 heads is $\frac{10}{32}=\frac{5}{16}$.
## Getting $x$ Amount in non-50/50 Events
Let's say we want to get the odds of spinning a 1 or a 2 in exactly 3 die rolls out of the next 5. (We are not trying to get the odds of getting *at least* 3 die rolls with a 1 or 2. We are trying to get the odds of getting *exactly* 3 die rolls. Getting *at least* something is [[#At Least $x$ Amount|discussed later]].)
We start with figuring out the odds of a single permutation with this result, for example $S, \space S, \space S, \space F, \space F$. ($S$ means "success", by which we mean spinning the 1 or 2, and by $F$ we mean "failure", by which we mean spinning a 3 or greater. This labeling is arbitrary.)
The way to figure out the odds of this happening is by multiplying the odds of each individual spin together as discussed [[Independent Events#Probability of Event A AND B|here]]. The odds of spinning a 1 or 2 is $\frac{1}{3}$, and the odds of spinning a 3 or greater is $\frac{2}{3}$. As such, we get:
$$\frac{1}{3} \times \frac{1}{3} \times \frac{1}{3} \times \frac{2}{3} \times \frac{2}{3}$$
If we wanted to write this a little simpler, we can write it as:
$$\left(\frac{1}{3}\right)^3 \times \left(\frac{2}{3}\right)^2$$
Either way, we get:
$$\boxed{\frac{4}{243}}$$
However, this is the odds of getting a *single* permutation. We don't just want the odds of this permutation. We want the odds of every permutation that has 3 "successes" and 2 "failures". How many different permutations are there?
We can figure this out using the [[Combinations#Calculation|combinations formula]]. In a sense, this is a combination. As discussed by combinations, we can view it that there are the numbers 1-5 here, each representing a die roll. We pick 3 of them for the "success" team and any we don't is a "failure". For example, if we pick 1, 3, and 4, then that means that rolls 1, 3 and 4 were "successes" and rolls 2 and 5 were failures.
We are trying to figure out how many different combinations of numbers we can pick without repeating a combination. And remember that the order does not matter: 1, 3, and 4, is the same as 4, 3, and 1.
This is exactly what a combination is, and so we can use the combination formula to calculate this.
The combination formula is:
$$\frac{(Total \space amount \space of \space things)!}{(Amount \space of \space things \space we \space are \space choosing)! \times (Amount \space of \space things \space we \space are \space not \space choosing)!}$$
Plugging in the numbers from out example, that is:
$$\frac{5!}{3!(5-3)!} \Rightarrow \frac{5!}{3! \times 2!} \Rightarrow \frac{120}{6 \times 2} \Rightarrow \frac{120}{12} = \boxed{10}$$
As such, we see that there are 10 different permutations for which we can spin a die 5 times and have it land on 1 or 2, 3 times and land on 3 or greater, 2 times.
We want to know the odds of any one of these permutations occurring. In other words, we want to know the odds of permutation A occurring, or permutation B, or permutation C, etc. To calculate this, we add them up, as discussed [[Independent Events#Probability of Event A OR B|here]].
As such, we get:
$$\frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243} + \frac{4}{243}$$
If we wanted to write this a little simpler, we can write it as:
$$\frac{4}{243} \times 10$$
Either way, we get:
$$\boxed{\frac{40}{243}}$$
And that is our final answer.
Putting it into a formula, it is:
$$probability \space of \space a \space single \space permutation \times amount \space of \space different \space permutations$$
## At Least $x$ Amount
The way to calculate the odds of getting *at least* a certain amount, we need to calculate the odds of getting each amount individually.
For example, if we wanted to calculate the odds of spinning *at least* 3, 1s or 2s, in the next 5 rolls, we have to calculate the odds of spinning, ⅗, and then calculate the odds of spinning ⅘, and then calculate the odds of spinning 5/5, and then add them all up.
This applies whether the event is 50/50 or not.
# Binomial Distributions
The distribution of a binomial is the percentage of each possible result in the binomial.
For example, let's say I want to see how many heads I get in 5 coin flips. We can calculate the likelihood of getting 0, 1, 2, 3, 4, or 5 heads. The calculations would be done as discussed [[#Getting $x$ Amount in 50/50 Events|above]]:
Since we are flipping the coin 5 times, there are $2^5$ different possiblilties. This is equal to 32.
The odds of getting 0 heads is therefore $\frac{1}{32}$. This can be calculated intuitively (there is only one way to get 0 heads, and that is by flipping 5 tails). But we can also figure this out using the formula above, which is $\frac{Amount \space of \space ways \space to \space get \space 0 \space heads}{total \space amount \space of \space different \space permutations}$.
The way to figure out how many ways one can get 0 heads is by doing $_5 C_0$. This is:
$$\frac{5!}{0! \times (5-0)!} \Rightarrow \frac{5!}{1\times 5!} = \boxed{1}$$
Now for 1 head:
$$\frac{5!}{1! \times (5-1)!} \Rightarrow \frac{5!}{1\times 4!} = \boxed{5}$$
Now for 2 heads:
$$\frac{5!}{2! \times (5-2)!} \Rightarrow \frac{5!}{2 \times 3!} \Rightarrow \frac{5 \times 4}{2} = \boxed{10}$$
Now for 3 heads:
$$\frac{5!}{3! \times (5-3)!} \Rightarrow \frac{5!}{6 \times 2!} \Rightarrow \frac{5 \times 4 \times 3}{6} = \boxed{10}$$
Now for 4 heads:
$$\frac{5!}{4! \times (5-4)!} \Rightarrow \frac{5!}{4! \times 1!} = \boxed{5}$$
Now for 5 heads:
$$\frac{5!}{5! \times (5-5)!} \Rightarrow \frac{5!}{5! \times 0!} = \boxed{1}$$
We now have our distribution.
The odds of getting 0 heads is $\frac{1}{32}$
The odds of getting 1 heads is $\frac{5}{32}$
The odds of getting 2 heads is $\frac{10}{32}$
The odds of getting 3 heads is $\frac{10}{32}$
The odds of getting 4 heads is $\frac{5}{32}$
The odds of getting 5 heads is $\frac{1}{32}$

As can be seen, once you pass the halfway point, the percentages repeat. This is true for all $50/50$ events.

If we graph this, it will look like this:
![[Coin Flip Distribution.png]]

## Binomial Distributions Approximate [[Density Curve#Normal Distribution|Normal Distributions]]
As can be seen in the example above, the binomial distribution somewhat approximates a bell curve, or a normal distribution. The more trials you have, the more the binomial will approximate the normal distribution. It is useful to work with normal distributions because there are certain rules about estimating the probabilities of normal distributions (see the linked article for further discussion).
# [[Random Variable#Expected Value (Average)|Expected Value (Average)]]
## Formula
The expected value (or average) of a binomial is:
$$(Amount \space of \space events) \times (Probability \space of \space each \space event)$$
Which is generally written as:
$$np$$
## Proof
A binomial is a certain amount of [[Bernoulli Trial|Bernoulli Trials]], where there is a set amount of events and the probability is independent.
A Bernoulli Trial is a random variable that has a value of 1 if there is a success and a value of 0 if there is a failure.
The probability of success is $p$ (by definition. $p$ is literally the probability of success) and the probability of failure is $1-p$.
A binomial is the value of these Bernoulli Trials added together.
As discussed [[Adjusting and Combining Random Variables#Random Variable Expected Value (Average) Expected Value (Average)|here]] when adding random variables together, the expected value of these random variables added together is equal to the expected value of each random variable added together.
As such, the expected value of a binomial is equal to the expected value of each Bernoulli Trial added together, or something like this:
$$E(Binomial) = E(Bernoulli \space Trial) + E(Bernoulli \space Trial) + ... E(Bernoulli \space Trial)$$
($E$ means expected value of...)
We add the expected value for the Bernoulli Trials as many times as there are trials in the binomial. If there are 5 trials, then we add the expected value 5 times to get the expected value of the binomial.
To make it simpler, instead of adding the expected value together a bunch of times, we can use multiplication, which looks like:
$$E(Binomial) = n \times E(Bernoulli \space Trial)$$
($n$ is the amount of Bernoulli Trials in the binomial.)
As discussed [[Bernoulli Trial#Random Variable Expected Value (Average) Expected Value (Average)|here]], the expected value of a Bernoulli Trial is equal to $p$. As such, replacing that in out equation, we get:
$$E(Binomial) = n \times p$$
or just:
$$E(Binomial) = \boxed{np}$$
# [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Variance|Variance]] and [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation#Standard Deviation (σ or $s$)|Standard Deviation]]
## Variance
### Formula
The formula is:
$$np(1-p)$$
### Proof
Similar to what we said by [[#Random Variable Expected Value (Average) Expected Value (Average)|expected value]], a binomial is made up of a bunch of Bernoulli Trials.
Bernoulli Trials are random variables where there are two possible values, 1 or 0, dependent on whether there is a success or a failure.
The probability of success is $p$ and the probability of failure is $1-p$.
As mentioned [[Adjusting and Combining Random Variables#Variance|here]], when we add the variances of numerous random variables, the variance of this "combined random variable" is equal to the variances of each random variable added together, which looks something like this:
$$V(Binomial) = V(Bernoulli \space Trial) + V(Bernoulli \space Trial) + ... V(Bernoulli \space Trial)$$
($V$ means variance of...)
We simplify this by using multiplication instead of addition, which becomes:
$$V(Binomial) = n \times V(Bernoulli \space Trial)$$
($n$ is the amount of Bernoulli Trials in the binomial.)
As discussed [[Bernoulli Trial#Mean Absolute Deviation (MAD), Variance, and Standard Deviation Variance Variance and Mean Absolute Deviation (MAD), Variance, and Standard Deviation Standard Deviation (σ or $s$) Standard Deviation|here]], the variance of a Bernoulli Trial is $p(1-p)$. As such, replacing that in out equation, we get:
$$V(Binomial) = n \times p(1-p)$$
or just:
$$V(Binomial) = \boxed{np(1-p)}$$
## Standard Deviation
### Formula
The standard deviation is just the square root of the variance. As such, the formula is:
$$\sqrt{np(1-p)}$$
# "10% Rule"
Because each test must be independent, technically, if we run a series of tests without replacement, the tests will not be independent. The odds of the later tests will depend on the results of the earlier tests.
For example, if I plan on selecting a card from a standard deck of cards 3 times and I want to see if any of them are kings, the odds of the first test is $\frac{4}{52}$, but the odds of the next test depend on the result of my first test. If I picked a king on the first test, the odds of picking another king on the second test is $\frac{3}{51}$, and if I didn't pick a king on the first test, the odds of picking a king on the second test is $\frac{4}{51}$.
Now, it is useful to work with binomials because they have relatively normal distributions, as mentioned above. As such, if the sample is 10% or less than the population size, we treat the random variable as a binomial, even though we are not replacing and so it is technically not a binomial. This is because even though all of the trials aren't fully independent, the fact that we pulled one piece of data out doesn't make much of a difference.
Obviously, the smaller of a percentage of the data is, the less of a difference each piece of data that is not being replaced makes.
At the same time, that does not mean that we prefer to work with small samples. Obviously large samples are better. It just means that in terms of achieving independence (or close to it), having a smaller sample is better.
# Bernoulli Trial
When we have a binomial but we only focus on a single instance of the experiment, that is called a Bernoulli Trial. For more details, see [[Bernoulli Trial|here]].
# Poisson Process
A Poisson process is a binomial with a near infinite number of trials. For more details, see [[Poisson Process|here]].