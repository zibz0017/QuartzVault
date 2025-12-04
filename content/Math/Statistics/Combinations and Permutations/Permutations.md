# Definition
<span style="display: block; text-align: justify;">The amount of possible ways of putting a number of things in some sort of order without reusing any.</span>
<span style="display: block; text-align: justify;">For example, you can have 5 people and you want to know how many possible ways you can line them up.</span>
<span style="display: block; text-align: justify;">Or you may have a number lock in which every number can only be used once and you want to know how many possible permutations there are.</span>
<span style="display: block; text-align: justify;">The difference between [[Combinations|combinations]] and permutations is that in a permutation, the order matters. In a combination, the order does not matter. So, for example, in a permutation, A, B, C is different than C, B, A. Even though the letters are the same, the order is different, and so it is a new permutation. However, these are both considered the same combination as only the things in the group matter, but not the order.</span>
# How to Calculate
## If Every Item Must be Used
### Formula
<span style="display: block; text-align: justify;">If every item must be chosen, then the formula is: $n!$ where $n$ is the number of things that there are.</span>
### Example 1
<span style="display: block; text-align: justify;">I have 5 people that I want to line up. We will call them A, B, C, D, and E. I can figure out the permutations as follows:</span>
<span style="display: block; text-align: justify;">In the first spot, I have 5 different options. I can put either A, or B, or C, or D, or E there.</span>
<span style="display: block; text-align: justify;">In the next spot, I only have 4 options. Whoever I put in the first spot can't go in the second spot.</span>
<span style="display: block; text-align: justify;">The same is true for the next 3 spots. In the third spot, there are three options. There are 2 options for the 4th spot, and only 1 option for the last spot.</span>
<span style="display: block; text-align: justify;">I then multiply all of these numbers together. The reason is as follows: For the first spot, we have 5 different options (A, B, C, D, E). No matter who we chose for the first spot, there are now 4 different options for the second spot. If we chose A for the first spot there is B, C, D, and E. If we chose B, then there is still A, C, D, and E. And the same is true if we chose C, D, or E for the first spot.</span>
<span style="display: block; text-align: justify;">From every one of the 5 people we chose in the first spot, there are 4 possibilities that "come out" of them as can be seen in the illustration (the dotted white line is just to make it clearer what is pointing to what. It doesn't actually mean anything):</span>
![[Pasted image 20250928003107.png]]
<span style="display: block; text-align: justify;">This give us $5 \times 4$ which equals $20$. If you look at the above picture, you can count all of the different possibilities and see that there are 20 options.</span>
<span style="display: block; text-align: justify;">We then keep going from here. There are 3 possibilities that come out of each one of these 20 possibilities ($20 \times 3 = 60$), 2 possibilities out of each of those 60 possibilities ($60 \times 2 = 120$) and then only 1 possibility from all of those 120 options ($120 \times 1 = 120$).</span>
<span style="display: block; text-align: justify;">As such, there are $\textbf{120}$ different possibilities.</span>
## If Only Some of the Items Must be Used
### Formula
<span style="display: block; text-align: justify;">In the following, $n$ is the total amount of items and $m$ is the amount of items that are being chosen.</span>
$$\frac{n!}{(n-m)!}$$
### Example 2
<span style="display: block; text-align: justify;">I have 5 people. We will call them A, B, C, D, and E, I want to line up only 3 of them. I can figure out the permutations as follows:</span>
<span style="display: block; text-align: justify;">Similar to last time, in the 1st spot, we have 5 possible options. In the 2nd spot, I now only have 4 options. And for the 3rd spot I only have 3 options.</span>
<span style="display: block; text-align: justify;">I am not filling in any more spots so I stop here.</span>
<span style="display: block; text-align: justify;">Just like we said before, from every one of my 5 options, I have 4 options that "come out" of them so I multiple them together ($5 \times 4 = 20$). I then have 3 options that "come out" of each one of those, so once again I multiply them together ($20 \times 3 = 60$).</span>
<span style="display: block; text-align: justify;">And now I am done. I don't keep going any farther because I am not lining anyone else up. I am only lining up 3 people and that's it.</span>
<span style="display: block; text-align: justify;">A way of thinking about this is kind of like we started doing $5!$ but we stopped partway through. We stopped after doing $5 \times 4 \times 3$. We didn't finish with the $\times 2 \times 1$.</span>
<span style="display: block; text-align: justify;">We can now understand the formula. First we start off with $5!$. The problem is that this is $5 \times 4 \times 3 \times 2 \times 1$, and we need only $5 \times 4 \times 3$. The way we "get rid" of the $\times 2 \times 1$ in the formula is to divide the $5!$ by $2!$. So it looks like this:</span>
$$\frac{5 \times 4 \times 3 \times 2 \times 1}{2 \times 1} \Rightarrow \frac{5 \times 4 \times 3 \times \cancel{2 \times 1}}{\cancel{2 \times 1}} \Rightarrow 5 \times 4 \times 3$$
<span style="display: block; text-align: justify;">We then cross out the $2 \times 1$ on the top and on the bottom. That gives us $5 \times 4 \times 3$, which is what we are looking for.</span>
<span style="display: block; text-align: justify;">But how did we get that $2!$ on the bottom? The 2 is the amount of things we didn't choose. If we start off with 5 people and choose 3, we didn't choose 2. In other words, $5-3=2$.</span>
<span style="display: block; text-align: justify;">And this is our formula:</span>
$$\frac{(Total \space amount \space of \space things)!}{(Total \space amount \space of \space things - Amount \space of \space things \space we \space are \space choosing)!}$$
<span style="display: block; text-align: justify;">Which is really the same as:</span>
$$\frac{(Total \space amount \space of \space things)!}{(Amount \space of \space things \space we \space are \space not \space choosing)!}$$
<span style="display: block; text-align: justify;">Plugging in the values in out example, we get:</span>
$$\frac{5!}{(5-3)!} \Rightarrow \frac{5!}{2!} \Rightarrow 5 \times 4 \times 3 = \boxed{\textbf{60}}$$
## Permutations with Combinations
Sometimes, you may want to figure out the amount of permutations there are for a group of items, but for some items, the order doesn't matter. You have to calculate the total amount of permutations and then divide by the amount of permutations there are for the things that the order doesn't matter for
### Example 3
For example, let's say you want to figure out the amount of ways you can order the letters A, B, C, D, A, A. There are 3 letter 'A's in this group. Obviously, all 'A's are the same. It doesn't matter which letter 'A' is first, second, or third. The order doesn't matter. However, the order for all of other letters does not matter. How do we figure this out?
First we calculate the total amount of permutations there are (pretending that the order of the 'A's does make a difference). There are 6 things and we are using all 6, so it is $6!$.
However, this calculation only works if the order of the 'A's matters. We need to divide the total by the amount of different permutations which are really the same, but just have the 'A's in different positions. (For the following, I am going to refer to the 'A's as $A_1$, $A_2$, and $A_3$ to make things easier).
So, for example, I can make the permutation A, A, A, B, C, D either by:
1. $A_1, \space A_2, \space A_3, \space B, \space C, \space D$
2. $A_1, \space A_3, \space A_2, \space B, \space C, \space D$
3. $A_2, \space A_1, \space A_3, \space B, \space C, \space D$
4. $A_2, \space A_3, \space A_1, \space B, \space C, \space D$
5. $A_3, \space A_1, \space A_2, \space B, \space C, \space D$
6. $A_3, \space A_2, \space A_1, \space B, \space C, \space D$
In terms of what we want, though, these are all the same. All 'A's are the same. We have to divide by 6 to get rid off all of these extra permutations which to us, don't count.
We don't need to count up all of the different permutations there are with the 'A's to figure this out. We can calculate it. There are 3 'A's and we are trying to figure out the amount of permutations there are. This is just $3!$., which is 6.
Getting back to the question, the calculation would be as follows: We have 6 total items, and we have 3 things that we don't care about the order for. The formula is as follows:
$$\frac{total \space amount \space of \space items}{amount \space of \space items \space that \space the \space order \space doesn't \space matter}$$Plugging in the numbers, we get:
$$\frac{6!}{3!} \Rightarrow \frac{720}{6} = \boxed{120}$$
### Example 4
<span style="display: block; text-align: justify;">Let's say I have multiple groups of items that I don't care about the order. Let's say I have the letters A, A, A, B, B, B and I want to know the amount of permutations that there are, but I don't care about the order of the 'A's, (meaning, it doesn't matter which 'A' comes first) and I don't care about the order of the 'B's (meaning, it doesn't matter which 'B' comes first). However, if an 'A' comes before a 'B' and vice-versa, that does matter.
Once again, we start with the total amount of permutations, which is $6!$.</span>
<span style="display: block; text-align: justify;">From there, we need to figure out the amount of permutations that we don't care about. As said earlier, because there are $3!$ different permutations which have the 'A's in the same places in the word, but they are swapping orders with each other. Like if I have A, B, A, B, A, B, there are $3!$ ways I can keep the 'A's in these spots (meaning, the 1<sup>st</sup>, 3<sup>rd</sup>, and 5<sup>th</sup>) positions but change the order of the 'A's.</span>
<span style="display: block; text-align: justify;">Because there are 3 'B's, the same is true for the 'B's, too. There are $3!$ different positions for the 'B's.</span>
<span style="display: block; text-align: justify;">However, we need to combine the 2. For every one of those $3!$ positions of 'A's, there is $3!$ positions of 'B's.</span>
<span style="display: block; text-align: justify;">For example, there are many ways I can make the permutation A, A, A, B, B, B. Let's say the 'A's are ordered $A_1, \space A_2, \space A_3$, there are $3!$ ways to order the 'B's. Let's say the 'A's are ordered $A_1, \space A_3, \space A_2$, the 'B's can still be arranged in $3!$ ways. And it keeps going. For every of the $3!$ ways to order the 'A's with keeping the placement of the 'A's in the arrangement (meaning, in the example, the 'A's will remain the 1<sup>st</sup>, 2<sup>nd</sup>, and 3<sup>rd</sup> numbers, just which 'A' comes 1<sup>st</sup>, 2<sup>nd</sup>, and 3<sup>rd</sup> changes) there are $3!$ ways to arrange the 'B's. In other words, for every single order of items, there are $3! \times 3!$ permutations, but we only care about 1 of them. Like in our example, $A_1, \space A_2, \space A_3, \space B_1, \space B_2, \space B_3$ is the same as $A_1, \space A_2, \space A_3, \space B_1, \space B_3, \space B_2$, which is the same as $A_1, \space A_3, \space A_2, \space B_3, \space B_2, \space B_1$, etc. We don't care about the order of the same type of letter (meaning, it doesn't matter which 'A' or which 'B' comes 1<sup>st</sup>). The only thing that matters is the order of the letters compared to the other type of letter (meaning, we only care about the order 'A's compared to the 'B's and vice-versa).</span>
<span style="display: block; text-align: justify;">As such, for such an example, we need to get the total possibilities, and then divide it by the all of the different ways that we can arrange the 'A's amongst themselves but leaving the 'A's in the same spot compared to the 'B's, times all of the different ways that we can arrange the 'B's amongst themselves but leaving the 'B's in the same spot compared to the 'A's. Plugging it in, we get:</span>
$$\frac{6!}{3! \times 3!} \Rightarrow \frac{720}{36}=\boxed{20}$$
# Notation
$${}_{n}P_{k}$$
<span style="display: block; text-align: justify;">Where $n$ is the total amount of things to choose from and $k$ is the amount of things that you are choosing. The $P$ in the middle just means that it is a permutation.</span>
<span style="display: block; text-align: justify;">So, for example, if there are 5 things and you are choosing 3 of them, you would write
${}_{5}P_{3}$. If there were 5 things and you were choosing all 5, it would be ${}_{5}P_{5}$.</span>


