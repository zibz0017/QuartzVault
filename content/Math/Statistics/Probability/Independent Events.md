# Definition
<span style="display: block; text-align: justify;">Independent events means that the result of one event do not affect the results of the next event. For example, all coin flips have a 50% of being heads and a 50% chance of being tales, regardless of what the results of the previous tests were.</span>
# Probability of Event A OR B
## Definition
<span style="display: block; text-align: justify;">We have a single random event (and event with different possible results with certain probabilities that they will occur). We would like to know the probability that one of two different possible results will occur.</span>
## Calculation
### Standard Procedure and Explanation
<span style="display: block; text-align: justify;">The way to calculate this is to get the probability of event A, add it to the probability of event B, and subtract the probability of both of these events occurring.</span>
<span style="display: block; text-align: justify;">The reason why we subtract the probability of event A and B occurring is because if we did not, we would be double counting it.</span>
<span style="display: block; text-align: justify;">When we calculate the probability of event A, we add up all of the different ways that event A can occur and divide it by the total amount of events that can occur. Included in this count is the event which would also satisfy event B. When we calculate the probability of event B, we include the event that satisfies event A. This event is being counted in the calculation of the probability of event A and also being counted in the calculation for event B. It is being double counted. As such, we have to subtract by that amount to make sure it is not double counted.</span>
### Formula
$$P(A)+P(B)-P(A\space and \space B)$$
### Mutually Exclusive Events
<span style="display: block; text-align: justify;">Some possible results may be mutually exclusive of some other result, meaning, that if one happens, the other can't happen. In such a situation, $P(A \space and \space B)$ is 0. As such, we can just drop it from the formula (subtracting by 0 doesn't change anything).</span>
## Example 1
<span style="display: block; text-align: justify;">Calculating the probability of selecting either a King or heart from a standard deck of cards without jokers. In this example we will refer to selecting a king as event $A$ and selecting a heart as event $B$. (It would be the same if we reversed it.)</span>
<span style="display: block; text-align: justify;">Total amount of cards in a standard deck: 52</span>
<span style="display: block; text-align: justify;">Total amount of Kings in a standard deck (event $A$): 4</span>
<span style="display: block; text-align: justify;">Total amount of hearts in a standard deck (event $B$): 13</span>
<span style="display: block; text-align: justify;">Total amount of Kings which are hearts in a standard deck (event $A$ and $B$): 1</span>
<span style="display: block; text-align: justify;">Plugging this information into the formula we get:</span>
$$\frac{4}{52}+\frac{13}{52}-\frac{1}{52} \Rightarrow \frac{16}{52} \Rightarrow \boxed{ \frac{4}{13}}$$
<span style="display: block; text-align: justify;">We have to subtract $\frac{1}{52}$ because that is double counted. There are 4 kings, and there are 13 hearts. However, one of those cards is a king *and* a heart. If we count all 4 kings and all 13 hearts, we will be counting the king of hearts into both groups.</span>
## Example 2
<span style="display: block; text-align: justify;">Calculating the probability of selecting either a King or Jack from a standard deck of cards without jokers. In this example we will refer to selecting a king as event $A$ and selecting a Jack as event $B$. (It would be the same if we reversed it.)</span>
<span style="display: block; text-align: justify;">Total amount of cards in a standard deck: 52</span>
<span style="display: block; text-align: justify;">Total amount of Kings in a standard deck (event $A$): 4</span>
<span style="display: block; text-align: justify;">Total amount of Jacks in a standard deck (event $B$): 4</span>
<span style="display: block; text-align: justify;">Total amount of cards which are both a King and Jack in a standard deck (event $A$ and $B$): 0</span>
<span style="display: block; text-align: justify;">Plugging this information into the formula we get:</span>
$$\frac{4}{52}+\frac{4}{52}-0 \Rightarrow \frac{8}{52} \Rightarrow \boxed{ \frac{2}{13}}$$
# Probability of Event A AND B
### Calculation
<span style="display: block; text-align: justify;">This is simply the probability of event A times the probability of event B. The formula looks like this:</span>
$$P(A) \cdot P(B)$$
### Example 3
<span style="display: block; text-align: justify;">The odds of flipping a heads, a tails, and a heads, is 1/8. This is calculation is as follows:</span>
$$\frac{1}{2} \cdot \frac{1}{2} \cdot \frac{1}{2} \Rightarrow \frac{1}{8}$$
<span style="display: block; text-align: justify;">This is because the probability of flipping a heads (or tails) is $\frac{1}{2}$, and since we want 3 particular events that each have a probability of $\frac{1}{2}$, we multiply $\frac{1}{2}$ by 3.</span>
# Probability of NOT Event A
## Calculation
<span style="display: block; text-align: justify;">The probability of not having A occur is the probability of any other event occurring (yes, this is obvious, but this is important for the calculation):</span>
<span style="display: block; text-align: justify;">As such, the easy way to calculate this is to subtract the probability of event A occurring from 1 (meaning 100%). The formula is as follows:</span>
$$1-P(A)$$
## Example 4
<span style="display: block; text-align: justify;">The probability of not spinning a 6 is:</span>
$$1-\frac{1}{6} \Rightarrow \frac{5}{6}$$
# Probability of AT LEAST ONE Event A
## Definition
<span style="display: block; text-align: justify;">There are many events occurring and we want to know the probability that at least one of them will have a certain result.</span>
## Calculation
### The "Wrong" Way
<span style="display: block; text-align: justify;">One way to do it would be to find all of the different permutations that have at least one event A and then adding the odds together, like we do whenever we are talking about the probability of one event or another (see [[#Probability of Event A OR B|here]]).</span>
<span style="display: block; text-align: justify;">However, this may take a very long time to do and is extremely inefficient. </span>
### The "Right" Way
<span style="display: block; text-align: justify;">A simpler way of calculating this would be to calculate the probability that all of the events are not A, and then subtract that from 1 (or 100%). In other words, we are trying to calculate the odds that this doesn't happen (meaning, we are calculating the odds that a series of events that do not contain event A, does not happen). We subtract from 1, as [[#Probability of NOT Event A|discussed]].</span>
<span style="display: block; text-align: justify;">This can be much simpler because there can be far fewer permutations that don't have a single A. In events that only have two possible results, then there is only one series of permutations that don't have a single A, in it: if every single result is B.</span>
## Example 5
<span style="display: block; text-align: justify;">The probability of flipping at least one heads in 3 coinflips can be calculated as follows:</span>
### Trying the "Wrong" Way
<span style="display: block; text-align: justify;">We need to add the probabilities of all of the different possible ways that there can be at least 1 heads in 3 coin flips together. All of the different possibilities are:</span>
1. <span style="display: block; text-align: justify;">HHH</span>
2. <span style="display: block; text-align: justify;">HHT</span>
3. <span style="display: block; text-align: justify;">HTH</span>
4. <span style="display: block; text-align: justify;">HTT</span>
5. <span style="display: block; text-align: justify;">THH</span>
6. <span style="display: block; text-align: justify;">THT</span>
7. <span style="display: block; text-align: justify;">TTH</span>
8. <span style="display: block; text-align: justify;">TTT</span>
<span style="display: block; text-align: justify;">Out of this list, the first 7 contain at least one heads. As such, this is 7/8 chance of flipping at least 1 head in 3 coin flips.</span>
### Trying the "Right" Way
<span style="display: block; text-align: justify;">The only way it can be that there are no heads is if there are only tails. To accomplish this, we need to flip a tails, and then another tails, and then another tails. If we take this and subtract it from 1. The way to calculate the probability of this is by multiplying the odds of each event together, as [[#Independent Events|discussed]].</span>
<span style="display: block; text-align: justify;">The odds of any coin flip (for a fair coin) is $\frac{1}{2}$. As such, the calculation is:</span>
$$1 - \left(\frac{1}{2}\right)^3 \Rightarrow 1 - \frac{1}{8} \Rightarrow \frac{7}{8}$$
<span style="display: block; text-align: justify;">This is can be far easier than going though all of the different permutations and writing them down.</span>
## Example 6
<span style="display: block; text-align: justify;">The probability of flipping at least 1 heads in 10 coinflips can be calculated as follows:</span>
<span style="display: block; text-align: justify;">In this example, it is clear that it is going to take a long time to go through all of the different possible permutations, so this time we are not even going to try the "wrong" way.</span>
<span style="display: block; text-align: justify;">Going with the "right" way, the only way there can be no heads is if we flip a tails on all 10 flips. As long as that doesn't happen, we flip at least one heads. The way to calculate that is as follows:</span>
$$1 - \left(\frac{1}{2}\right)^{10} \Rightarrow 1 - \frac{1}{1024} \Rightarrow \frac{1023}{1024}$$