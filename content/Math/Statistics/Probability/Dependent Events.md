# Definition
<span style="display: block; text-align: justify;">We have multiple events happening. The odds of one of the events occurring changes depending on the result of the other event. (In other words, these events are correlated. The odds that a person will contract a disease if they took a vaccine goes down. This also goes the other way, too. If someone contracts a disease, it is less likely that they took a vaccine.) Dependence in this context has nothing to do with causation.</span>
<span style="display: block; text-align: justify;">Dependence goes both ways. If event A is dependent on event B, then event B is dependent on event A, and vice-versa. See the example in the previous paragraph.</span>
# Calculation
<span style="display: block; text-align: justify;">As we said by [[Independent Events#Probability of Event A AND B|independent events]], we need to multiply the probability of the events happening together.</span>
<span style="display: block; text-align: justify;">This is more difficult to do than by independent events because there are now many more options. Even though there are just two events, we need to calculate the odds of each leg, meaning, we need to calculate:</span>
1. <span style="display: block; text-align: justify;">The probabilities of all of the different possibilities of the first result.</span>
2. <span style="display: block; text-align: justify;">The probability that the second event will have a certain result, given each one of these possible results in the first event.</span>
## Syntax
<span style="display: block; text-align: justify;">We represent "given that a certain event occurred" with the $|$ symbol.</span>
<span style="display: block; text-align: justify;">For example, $P(A|B)$ means the probability of $A$ given that $B$ has happened.</span>
## Example 1
<span style="display: block; text-align: justify;">There are 2 weighted coins in a bag with 40% to land on heads, and 5 normal coins (50/50). The probability of selecting one coin at random from the bag and flipping 2 heads in a row is as follows:</span>
1. <span style="display: block; text-align: justify;">The probability of selecting an unfair coin is $\frac{2}{7}$. The probability of flipping two heads in a row with this unfair coin is $\frac{2}{5} \cdot \frac{2}{5} = \frac{4}{25}$.</span>
2. <span style="display: block; text-align: justify;">We now need to calculate the odds of both selecting an unfair coin AND flipping two heads in a row. We do this by multiplying the odds together (as [[#Independent Events|discussed]]). As such, that is $\frac{2}{7} \cdot \frac{2}{5} = \frac{4}{35}$.</span>
3. <span style="display: block; text-align: justify;">The probability of selecting a fair coin is $\frac{5}{7}$. The probability of flipping two heads in a row with this fair coin is $\frac{1}{2} \cdot \frac{1}{2} = \frac{1}{4}$.</span>
4. <span style="display: block; text-align: justify;">We now need to calculate the odds of both selecting a fair coin AND flipping two heads in a row. We do this by multiplying the odds together. As such, that is $\frac{5}{7} \cdot \frac{1}{2} = \frac{5}{14}$.</span>
5. <span style="display: block; text-align: justify;">We now need to find the odds of flipping two heads with an unfair coin OR flipping two heads with a fair coin. We do this by adding the odds together (as [[#Probability of Event A OR B|discussed]]). As such, that is $\frac{4}{35} + \frac{5}{14} = \frac{33}{70}$.</span>
# Bayes' Theorum
## Formula
$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$
## Logic
<span style="display: block; text-align: justify;">$P(A|B) \cdot P(B)$ and $P(B|A) \cdot P(A)$ are equal to each other. They are both ways of calculating the odds of both events occurring when they are dependent on the other. As such, they are equal to each other. So we just need to do some algebra to arrive at the formula:</span>
$$P(A|B) \cdot P(B) = P(B|A) \cdot P(A)$$
Divide both sides by $P(B)$:
$$P(A|B)= \frac{P(B|A) \cdot P(A)}{P(B)}$$
## Calculation by Hand
### Why this is Useful
<span style="display: block; text-align: justify;">This can be simpler to use sometimes, and it is more intuitive than the formula.</span>
### Steps
1. <span style="display: block; text-align: justify;">Make a tree map of all of the different possible outcomes.</span>
2. <span style="display: block; text-align: justify;">Disregard all of the possibilities that don't end with what actually occurred.</span>
3. <span style="display: block; text-align: justify;">You now have a ratio for all of the different possibilities which occurred from one side, and from the other.</span>
### Example 3
<span style="display: block; text-align: justify;">There is a bag with 3 coins. 2 are fair and 1 has heads on both sides. A coin is picked at random and tossed twice. It lands on heads both times. The odds that the double sides coin was picked can be calculated as follows:</span>
<span style="display: block; text-align: justify;">We start with a tree diagram with all of the different possibilities:</span>
![[Pasted image 20250920232923.png]]
<span style="display: block; text-align: justify;">As can be seen, there are 12 different possibilities for what could have happened, before taking in to account the results of the coin flip.</span>
<span style="display: block; text-align: justify;">Once we take the results of the coin flip into account, then we see that not all of these results are possible. We flipped the coin twice and landed on heads both times. That means that only a path that has heads both times is possible. Any path that has a tails could not have happened.</span>
<span style="display: block; text-align: justify;">Of all these paths, that leaves paths 1, 5, 9, 10, 11, and 12. And of these paths, 2 of them are from fair coins (path 1 and 5) and 4 are not (path 9, 10, 11, and 12). As such there are 4 ways that we could have achieved this result if we picked the unfair coin and only 2 if we picked the fair coin. As such, the odds that the double sided coin was picked is $4/6$ or $2/3$.</span>


