For random variable basics, see [[Random Variable|here]].
# Adding Constant to Random Variables
If you add a constant to every value in a random variable, the mean will change by that constant.
The amount of each standard deviation will not change at all.
## Example 1
If I measure the height of a bunch of people, I will get a certain mean, and a certain standard deviation.
If I randomly decide to add 5 inches to everyone's height, the mean will move up by 5 inches.
The standard deviation will not change at all. Everyone is still the same distance from the mean as they were before.
# Multiplying Constant to Random Variables
If you multiply every value in a random variable, the mean and standard deviation will both change by a factor of that constant.
## Working out the Math
The standard deviation of a random variable is: $$\sqrt{\frac{\sum_{i=1}^n{\left(x_i-\mu\right)}^2}{n}}$$
If we multiply every value by $k$, then $x_i-\mu$ will be $k$ times higher, for every value of $x$. For example, if I am measuring the height of a bunch of people and the mean is 6 feet (72 inches) and someone is 5" 11' (71 inches) and then I multiply all of the heights by 5, the mean will be 30 feet (360 inches) and the height of this person will be 29" 7' (355 inches), now 5 inches away from the mean.
As such, before $x_i-\mu$ would have been 1. Now it is 5.
For the next step in calculating the standard deviation, I am going to end up squaring all of these values. Now all of these value are $k^2$ what they were before.
The next step is to add them all up. The total is now $k^2$ what they were before.
The next step is to divide by $n$. $n$ does not change because I multiplied the values. As such, this is going to remain $k^2$ more than what it was before.
However, now when I take the square root, it only becomes $k$ times what it would have been.
Let's say that until the last square root step, the value of everything would have been $x$. Now that I multiplied all of the individual values by $k$ it is now (meaning, right before this last step that we get the square root) $k^2$ more, as discussed.
To get the square root, it would look something like this: $\sqrt{xk^2}$. This is the same as this: $\sqrt{x} \times \sqrt{k^2}$, which becomes $\sqrt{x} \times k$.
Before multiplying all of the values by $k$ the standard deviation would have been $\sqrt{x}$ (because $x$ was the value that we got right before this last square root step). Now that we multiplied everything by $k$, the standard deviation is $\sqrt{x} \times k$. $\sqrt{x} \times k$ is $k$ times bigger than $\sqrt{x}$.
## Example 2
If I measure the height of a bunch of people, I will get a certain mean, and a certain standard deviation.
If I randomly decide to multiply every height by 5, the mean will be 5 times higher.
The standard deviation will also increase by 5 times, because now, everyone is 5 times farther from the mean.
# Adding and Subtracting Random Variables Together
Let's say we want to combine random variables to together, like, let's say we took the heights of a bunch of people on Sunday and we calculated the mean and variance and then we took the height of a bunch of other people on Monday and also calculated the mean and variance.
Now, let's say we want to randomly select one person from each group. What is the expected value and mean of these 2 people together (meaning, if we added their heights together)?
## Expected Value (Mean)
The expected value of this group is simply the means of each group added together/subtracted from each other (depending on whether you are adding them together or subtracting them from each other). Written in formula, this is:
$$\mu_{X+Y}=\mu_X+\mu_Y$$
and:
$$\mu_{X-Y}=\mu_X-\mu_Y$$
($X$ and $Y$ are random variables)
## Variance
The variance of the combined group depends on how independent the selections are. If the selections are totally independent (meaning, we randomly select someone from the first group and randomly select someone from the second group. We don't make a decision about who to select from the second group based on who we selected in the first group) then the variance is simply the variance of both groups added together. This is true for both adding the random variables together or subtracting them from each other.
For a simple example of why the selections must be independent, see [[#Example 4|below]].
The formula is:
$$\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y) + 2 \cdot \text{Cov}(X, Y)$$
($X$ and $Y$ are random variables and $\text{Cov}$ is the the covariance) <span style="color:rgb(255, 0, 0)">Need to learn about covariance and then add link</span>
As such, if the $\text{Cov(X,Y)=0}$, we get:
$$\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y) + 2 \cdot 0 \Rightarrow \boxed{\text{Var}(X + Y) = \text{Var}(X) + \text{Var}(Y)}$$

In other words, if the covariance is 0 (everything is independent), the variance of the combined group is the variance of each group added together.
## Standard Deviation
The standard deviation is the square root of the variance.
We discussed how to calculate the variance of the combined group. The way to get the standard deviation for combined group is by calculating the variance of the combined group and then taking the square root.
Adding/subtracting the standard deviation of each group together/from each other will not work.
## Example 3
Group 1 has four people with heights (in inches) of 60, 61, 65, and 70. Group 2 has four people with heights of 65, 70, 72, and 73.
### Calculating the Mean
The mean of the first group is:
$$\frac{60+61+65+70}{4} \Rightarrow \frac{256}{4} = \boxed{64}$$
The mean of the second group is:
$$\frac{65+70+72+73}{4} \Rightarrow \frac{280}{4} = \boxed{70}$$
Together this becomes:
$$64+70=\boxed{134}$$
The way to calculate the mean of adding the heights of each member of group one with each member of group two is as by getting the heights for each combination and getting the average:
$$60+65=125$$
$$60+70=130$$
$$60+72=132$$
$$60+73=133$$
$$61+65=126$$
$$61+70=131$$
$$61+72=133$$
$$61+73=134$$
$$65+65=130$$
$$65+70=135$$
$$65+72=137$$
$$65+73=138$$
$$70+65=135$$
$$70+70=140$$
$$70+72=142$$
$$70+73=143$$
The average of all of these is:
$$\frac{125+130+132+133+126+131+133+134+130+135+137+138+135+140+142+143}{16} \Rightarrow$$
$$\frac{2144}{16}=\boxed{134}$$
### Calculating the Variance
The variance of the first group is:
$$\frac{(60-64)^2 + (61-64)^2 + (65-64)^2 + (70-64)^2}{4} \Rightarrow$$
$$\frac{16+9+1+36}{4} = \boxed{15.5}$$
The variance of the second group is:
$$\frac{(65-70)^2 + (70-70)^2 + (72-70)^2 + (73-70)^2}{4} \Rightarrow$$
$$\frac{25+0+4+9}{4}= \boxed{9.5}$$
Together this becomes:
$$15.5+9.5=\boxed{25}$$
We need to calculate the variance of all of the heights for the heights of every member from both groups added together. We already calculated these heights earlier, so now we just need to calculate the variance for them. That is:
$$\frac{(125-134)^2 + (130-134)^2 + (132-134)^2 + (133-134)^2 + (126-134)^2 + (131-134)^2 + (133-134)^2 + (134-134)^2 + (130-134)^2 + (135-134)^2 + (137-134)^2 + (138-134)^2 + (135-134)^2 + (140-134)^2 + (142-134)^2 + (143-134)^2}{16} \Rightarrow$$
$$\frac{81+16+4+1+64+9+1+0+16+1+9+16+1+36+64+81}{16} \Rightarrow$$
$$\frac{400}{16} = \boxed{25}$$
### Calculating the Standard Deviation
The standard deviation is the square root of the variance. As such, it is:
$$\sqrt{25}=\boxed{5}$$
#### What not to Do
As said before, adding the standard deviations of each group together will not get the correct standard deviation for the combined group. We will demonstrate that.
The standard deviation for the first group is the square root of its variance. We calculated that before, so we just need to take the square root, which is:
$$\sqrt{15.5} \approx 3.937$$
We also calculated the variance of the second group. Taking the square root of that we get:
$$\sqrt{9.5} \approx 3.082$$
If we add them together we get:
$$3.937+3.082=7.019$$
This is not correct. As shown before, the standard deviation for the combined group is 5.
## Example 4
Let's say we have two "groups". We take the average amount that people sleep and the average amount that they are awake.
Let's say that the data come out to have an average of 8 hours of asleep and 16 hours of awake.
Let's also say that the variance for each group is 2 hours.
Let's say we want to calculate the variance in the amount of asleep plus awake time for each person (meaning, we add together the amount of time that each person sleeps plus the amount of time that they are awake. But we only do this for each person, meaning, we add the asleep plus awake time of person A, and the same for person B, etc. We don't add person A's awake time to person B, for example).
The variance is very easy to calculate; it is going to be 0. This is because everyone is asleep plus awake for 24 hours a day. As such, there is going to be 0 variance.
If we added the variance of each group together, we would get 4 hours. We can clearly see that this would not work here.
# Distribution Curve of Combined Random Variable
If the two random variables are normally distributed, if we made a new random variable of the difference between the two random variables, it would also be normally distributed.
## Example 5
Let's say the average height of men is 70 inches with a standard deviation of 5 inches and the average height of women is 65 inches with a standard deviation of 4 inches, what are the odds that a randomly selected man will be taller than a randomly selected woman?
We can calculate this by subtracting the random variable of the height of women from the random variable of the height of men and create a new random variable.
We will call the random variable for he height of men $M$, the random variable for the height of women $W$ and the random variable for the height of a random man minus the height for a random women $C$ (for combination).
As said before, the mean of the combined random variable is just the means of the individual random variables subtracted from each other. As such, it becomes:
$$\mu_C=\mu_M-\mu_W \Rightarrow 70-65=\boxed{5}$$
The standard deviation is the square root of the variance of the height of men minus the variance of the height of women. Since we only have the standard deviations of each group, we have to square them to get the variance of each group. This is as follows (first for the men and then for the women):
$$\sigma^2_M=5^2=\boxed{25}$$
$$\sigma^2_W=4^2=\boxed{16}$$
We now need to add the women's variance to the men's and then get the square root. This becomes:
$$\sigma_C=\sqrt{25+16} \Rightarrow \sqrt{41} \approx \boxed{6.4}$$
The average of the combined random variable is 5 and the standard deviation is 6.4. We want to know the percentage that a randomly selected man will be shorter than a randomly selected woman. That means that we want to find out what percentage of the density curve of the random variable is below 0. (When the height of a random man minus the height of a random woman is less than 0, that means that the woman is taller than the man).
Because the random variable for the height of men and women are both normally distributed, the random variable for the height of men minus the height of women is also normally distributed.
Because the combined random variable is normally distributed, we can use a [[Density Curve#Z-Table|z-table]] to figure out what percentage of the random variable is below 0.
We need to figure out how many standard deviations below the mean the value of 0 is. the mean is 5, and the standard deviation is 6.4. That gives us:
$$\frac{5}{6.4} \approx .78$$
We now can use [a z-table](https://en.wikipedia.org/wiki/Standard_normal_table#Cumulative_(less_than_Z)) to figure out how much of the density curve is below this value. We see that .22363 of the data is below 0. As such, the odds that a randomly selected man is taller than a randomly selected woman is: $1-.22363=\boxed{.77637}$.
