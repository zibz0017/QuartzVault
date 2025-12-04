# Definition
<span style="display: block; text-align: justify;">The amount of different groups one can make of a specific size from a different group.</span>
<span style="display: block; text-align: justify;">For example, you may have 5 people, and you want to know how many different groups of 3 people you can make.</span>
<span style="display: block; text-align: justify;">The difference between combinations and [[Permutations|permutations]] is that in a permutation, the order matters. In a combination, the order does not matter.</span>
<span style="display: block; text-align: justify;">So, for example, in a permutation, A, B, C is different than C, B, A. Even though the letters are the same, the order is different, and so it is a new permutation. However, these are both considered the same combination as only the things in the group matter, but not the order.</span>
# Calculation
<span style="display: block; text-align: justify;">First we start off with the [[Permutations#If Only Some of the Items Must be Used|permutations formula when not all of the items are picked]]. The formula is $\frac{n!}{(n-m)!}$ where $n$ is the total amount of things and $m$ is the amount of things being chosen (see there for more details).</span>
<span style="display: block; text-align: justify;">For example, if I have 5 things (which I will call A, B, C, D, and E) and I am choosing 3, I get $\frac{5!}{(5-3)!} \Rightarrow \frac{5!}{2!} = 60$.</span>
<span style="display: block; text-align: justify;">However, this gets us the amount of *permutations*, not that amount of *combinations*.</span>
<span style="display: block; text-align: justify;">We need to find out how many different permutations there are for every unique group selected and divide by that amount.</span>
<span style="display: block; text-align: justify;">So going back to the example, let's say I selected A, B, and C. When I calculate permutations, I need to figure out how many different ways I have of lining this group up. I can order them as:</span>
1. A, B, C
2. A, C, B
3. B, A, C
4. B, C, A
5. C, A, B
6. C, B, A
<span style="display: block; text-align: justify;">When it comes to permutations, these all count as permutations. When it comes to combinations, these all count as 1. For every group of 3 letters that I choose, I will have only 1 combination (because the only thing that matters is the letters I chose, not the order I put them in) and I will have 6 combinations, as shown above.</span>
<span style="display: block; text-align: justify;">But we don't need to write out all of the different permutations to be able to know how many different permutations there are. We can [[Permutations#If Every Item Must be Used|calculate]] it using $n!$. In this case, since we have 3 things, it is $3!$, which is 6.</span>
<span style="display: block; text-align: justify;">This is how we calculate combinations: First we start with the permutations formula. We then divide by the amount of permutations that can be made with the group of items that we selected.</span>
<span style="display: block; text-align: justify;">As such, we get:</span>
$$\frac{permutation \space formula}{amount \space of \space permutations \space for \space the \space group \space of \space items \space selected}$$
<span style="display: block; text-align: justify;">which becomes:</span>
$$\frac{\left(\frac{n!}{(m-n)!}\right)}{m!}$$
<span style="display: block; text-align: justify;">where $m$ is the amount of items being selected. And this gets simplified into:</span>
$$\frac{n!}{m!(m-n)!}$$
<span style="display: block; text-align: justify;">Replacing the symbols, this means the following:</span>
$$\frac{(Total \space amount \space of \space things)!}{(Amount \space of \space things \space we \space are \space choosing)! \times (Amount \space of \space things \space we \space are \space not \space choosing)!}$$
<span style="display: block; text-align: justify;">Going back to our example, we would get:</span>
$$\frac{5!}{3!(5-3)!} \Rightarrow \frac{5!}{3! \times 2!} \Rightarrow \frac{120}{6 \times 2} \Rightarrow \frac{120}{12} = \boxed{10}$$
# Notations
## Notation 1
$${}_n{C}_{k}$$
<span style="display: block; text-align: justify;">Where $n$ is the total amount of things to choose from and $k$ is the amount of things that you are choosing. The $C$ in the middle just means that it is a combination.</span>
<span style="display: block; text-align: justify;">So, for example, if there are 5 things and you are choosing 3 of them, you would write ${}_{5}C_{3}$.</span>
## Notation 2
$$\binom{n}{k}$$
<span style="display: block; text-align: justify;">Where $n$ is the total amount of things to choose from and $k$ is the amount of things that you are choosing.</span>
<span style="display: block; text-align: justify;">So, for example, if there are 5 things and you are choosing 3 of them, you would write $\binom{5}{3}$.</span>