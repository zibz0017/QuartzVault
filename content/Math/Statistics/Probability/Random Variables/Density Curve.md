*This may also be called a [[Random Variable#Continuous|continuous random variable]].*
# Definition
A function of the distribution of the probability of an event. It basically is a line graph for the probability of an event at different values. The y-value is the probability for the event at the specific x-value.
## Examples
1. The height of different people. Some people are tall, some are short, some are somewhere in between.
2. The temperature in different parts of the world. Some places are hot, some are cold, and some are in between.
## Specific Points
1. The area under the curve will equal 1. We are dealing with probability. The probability that some event will occur is 100%. (If your flipping a coin, the odds that the coin will be heads *or* tails is 100%. If you are measuring the height of different people, the odds that everyone will be *some* height is 100%. If you are measuring the temperature of different places, the odds that every place will be *some* temperature is 100%.)
2. There are an infinite number of points in a density curve (as there are for any function). The x-value can be 1, or 2, or 1.1, or 1.01...
3. The probability for any exact value is basically 0. This makes intuitive sense. For example, think about the odds of rain tomorrow being exactly 2 inches. Not 2.1 inches. Not 1.9. Not 2.0000000000001. Not 1.999999999999999. It has to be *exactly* 2. It is basically infinitely small.
4. As such, when we talk about probabilities, we generally refer to a range of values. Like we might say, what is the probability that rain tomorrow will be between 1.9 and 2.1 inches.
5. This is calculated by finding the area under the curve for those x values. This is usually done by using calculus. <span style="color:rgb(255, 0, 0)">Add link</span>
# Different Types of Distributions
## Normal Distribution
This is the "standard", "bell-shaped" distribution of data. It is symmetrical. It rises in the middle, goes down on the sides, and then trails off on the right and left.

Example of a normal distribution:
![[Pasted image 20250610221007.png]][^1]
### Empirical Rule (68-95-99.7 Rule)
In a perfect normal distribution, a certain percentage of the data will fall within a certain amount of [[Mean Absolute Deviation (MAD), Variance, and Standard Deviation|standard deviations]] from the mean. In real life there is basically no such thing as a *perfect* normal distribution, but this still a good approximation.

Around 68% of the data is found within one standard deviation of the mean. Around 95% of the data is found within two standard deviations. And around 99.7% is found with three standard deviations.

![[Pasted_image_20250610215901_optimized.png]][^2]
### Z-Table
Similarly, a certain percentage of the data is below a point that a is certain amount of standard deviations above or below the mean. These amounts are found on a z-table (such as the one [here](https://en.wikipedia.org/wiki/Standard_normal_table#Cumulative_(less_than_Z))).

The way to read the z-table is that you go down the table to find the whole number and the first number of the decimal (the tenths spot). You then go across the list to find the second number of the decimal (the hundredths spot).

For example, to find what percentage of data is below 1.43 standard deviations, you would go down the table to the row with 1.4, and then you would go across until the column with .03.

![[Screenshot_2025-06-10_235951_optimized.png]]

As can be seen, around 92.4% of the data lies below the 1.43 standard deviations.

One can use these table to find out how much of the data is above a point that is a certain amount of standard deviations, or is between two different points at different standard deviations.
<span style="color:rgb(255, 0, 0)">There is something called the "standard correction" which is important to note when using a z-table.</span>
## Bimodal Distribution
Similar to a normal distribution except the data peaks in two different places, with a small valley between, and trails off to both sides.

This may occur in data that has normally distributed, but there is one piece of information that makes a major difference in the value of the data.

For example, if we took the weight of many different adults, this should have a normal distribution. However, if the person is male or female makes a big difference.

An example of a bimodal distribution:
![[Pasted image 20250610213834.png]][^3]
## Skewed Distribution
One side of the distribution is much steeper. The other side extends in a long tail. If the tail is to the left, it is called left-skewed. If it is toward the right, it is right skewed.

The mean is closer to the side with the tail than the median. The reason is because the median is the point where there is an equal number of points on either side. It doesn't matter how far away any of the points are.

The mean is affected by how far away points are. Since the "tail side" of the graph has points which are far away, this pulls the mean toward that side.

A way to think of the mean is like the point that balances both halves of the graph. Small amounts farther away pull their side down just as hard as many points closer to the fulcrum.

![[Pasted image 20250610233028.png]][^4]
# Footnotes

[^1]: [University of Illinois : Data Science Discovery : Normal Distribution](https://discovery.cs.illinois.edu/learn/Simulation-and-Distributions/Normal-Distribution/)
[^2]: [Dr Dawn Wright : Empirical Rule and z-score Probability](https://www.drdawnwright.com/empirical-rule-and-z-score-probability/)
[^3]: [Wikipedia : Multimodal Distribution](https://en.wikipedia.org/wiki/Multimodal_distribution)
[^4]: [Statistics How To : Skewed Distribution](https://www.statisticshowto.com/probability-and-statistics/skewed-distribution/)