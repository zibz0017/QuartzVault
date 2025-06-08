# What it Means
$$\sum^{NumberOnTop}_{i=NumberOnBottom}Term$$
This can be viewed as a for loop (in programming). This means that we get calculate the term with i having the value of NumberOnBottom. We then calculate the term with i having the value of NumberOnBottom+1. We do that for i having the value of NumberOnBottom+2, +3…. We keep doing that until i has the value of NumberOnTop.

We then take all of those values and add them together.

## Steps
1. Calculate the term with i having the value of NumberOnBottom.
2. Calculate the term with i having the value of NumberOnBottom+1.
3. Calculate the term with i having the value of NumberOnBottom+2.
4. Calculate the term…
5. Calculate the term with i having the value of NumberOnTop.
6. Add all of these numbers together.
## Example 1
$$\sum^{5}_{i=1}i$$
In the first pass, i=1, so the term (which is just i) equals 1. In the second, i=2, so the term equals 2. Then i=3, so the term equals 3, then i=4 so the term equals 4, and i=5, so the term equals 5.

So in all, we have 1, 2, 3, 4, and 5. We add them up and that is out answer:
$$1+2+3+4+5=\textbf{15}$$
## Example 2
$$\sum^{5}_{i=1}2$$
In the first pass, i=1, but the term doesn't have an i. It is just 2. In the second, i=2, but once again, the term doesn't have an i, so it is still 2. Then i=3, but the term still equals 2, then i=4 but the term still equals 2, and i=5, but the term still equals 2.

In all, we have 2, 2, 2, 2, and 2, which gives us:
$$2+2+2+2+2=\textbf{10}$$
## Example 3
$$\sum^{5}_{i=1}2i+4$$
(Going to go a little faster in this one.)

This equals:
$$(2 \cdot 1 + 4)+(2 \cdot 2 + 4)+(2 \cdot 3 + 4)+(2 \cdot 4 + 4)+(2 \cdot 5 + 4) \Rightarrow (6)+(8)+(10)+(12)+(14)=\textbf{50}$$
# Manipulations/Simplification
## Turn Into Multiplication
If there is a constant value, this can be turned into multiplication.
### Example 4
$$\sum^{5}_{i=1}3$$
$$\Rightarrow (3) + (3) + (3) + (3) + (3) = \textbf{15}$$
You can also think of this as:
$$3 \cdot 5 = \textbf{15}$$
### Rational
The reason is that this is what multiplication means. It means add a certain number to itself a certain amount of times. This is how you explain what multiplication means to someone who only knows addition.
## Turn Into Multiplication (Continued)
Even if the constant value is multiplying $i$, you can pull the constant out, and multiple the whole summation by the constant.
### Example 5
$$\sum^{5}_{i=1}3i$$
$$\Rightarrow (3 \cdot 1) + (3 \cdot 2) + (3 \cdot 3) + (3 \cdot 4) + (3 \cdot 5)$$
$$\Rightarrow (3) + (6) + (9) + (12) + (15) = \textbf{45}$$
Is the same as:
$$3 \cdot \sum^{5}_{i=1}i$$$$\Rightarrow 3((1) + (2) + (3) + (4) + (5)) \Rightarrow 3(15) = \textbf{45}$$
### Rational
the previous rational applies here, as well.

Another way of thinking about it is that we are using the distributive property. The same way we can "pull the 3 out" of the following: $(3x+3y) \Rightarrow 3(x+y)$, we are similarly "pulling the 3 out" in our problem:
$$(3 \cdot 1) + (3 \cdot 2) + (3 \cdot 3) + (3 \cdot 4) + (3 \cdot 5)$$
pulling the 3 out gives us:
$$3 \cdot((1) + (2) + (3) + (4) + (5))$$
### Note
You can't pull the $i$ to the left side. It wouldn't really make sense to. What would its value be?
## Split the Summation
If the term has two parts which are added together, this can be split into two separate summations.
### Example 6
$$\sum^{5}_{i=1}i + 2^i$$$$ \Rightarrow (1 + 2^1) + (2 + 2^2) + (3 + 2^3) + (4 + 2^4) + (5 + 2^5) \Rightarrow (3) + (6) + (11) + (20) + (37) = \textbf{77}$$
This is the same as this:
$$\left( \sum^{5}_{i=1}i \right) + \left( \sum^{5}_{i=1}2^i \right)$$
$$\Rightarrow ((1) + (2) + (3) + (4) + (5)) + ((2^1) + (2^2) + (2^3) + (2^4) + (2^5))$$
$$\Rightarrow ((15)) + ((2) + (4) + (8) + (16) + (32)) = \textbf{77}$$
### Rational
The associative property of addition. Order doesn't matter when it comes to addition. When we split the term into two separate summations, we are just changing the order of what we are adding together. Compare the following:
$$(1 + 2^1) + (2 + 2^2) + (3 + 2^3) + (4 + 2^4) + (5 + 2^5)$$
and:
$$((1) + (2) + (3) + (4) + (5)) + ((2^1) + (2^2) + (2^3) + (2^4) + (2^5))$$
You can see that all of the numbers are the same. The only difference is the order and the parentheses.
### Note
This is only true when the two parts of the term are *added* or *subtracted*. This would not apply to *multiplication* or *division*.