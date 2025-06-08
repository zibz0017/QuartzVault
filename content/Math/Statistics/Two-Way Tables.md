# Basic Definition with Examples
Two way tables compare how two different statistics line up with each other. For example:

|                     | Men | Women | Total |
| ------------------- | --- | ----- | ----- |
| Yankees fan         | 9   | 1     | 10    |
| Mets fan            | 5   | 4     | 9     |
| Fan of another team | 2   | 7     | 9     |
| Total               | 16  | 12    | 28    |

We can also look at relative frequencies.
Going down the columns (may be slightly off because of rounding):

|                     | Men            | Women          | Total           |
| ------------------- | -------------- | -------------- | --------------- |
| Yankees fan         | **56%** (9/16) | **8%** (1/12)  | **36%** (10/28) |
| Mets fan            | **31%** (5/16) | **33%** (4/12) | **32%** (9/28)  |
| Fan of another team | **12%** (2/16) | **58%** (7/12) | **32%** (9/28)  |
| Total               | 16             | 12             | 28              |

Going across the rows:

|                     | Men             | Women           | Total |
| ------------------- | --------------- | --------------- | ----- |
| Yankees fan         | **90%** (9/10)  | **10%** (1/10)  | 10    |
| Mets fan            | **56%** (5/9)   | **44%** (4/9)   | 9     |
| Fan of another team | **22%** (2/9)   | **78%** (7/9)   | 9     |
| Total               | **57%** (16/28) | **43%** (12/28) | 28    |

Or both:

|                     | Men                                   | Women                                 | Total |
| ------------------- | ------------------------------------- | ------------------------------------- | ----- |
| Yankees fan         | Of column: **56%**<br>Of row: **90%** | Of column: **8%**<br>Of row: **10%**  | 10    |
| Mets fan            | Of column: **31%**<br>Of row: **56%** | Of column: **33%**<br>Of row: **44%** | 9     |
| Fan of another team | Of column: **12%**<br>Of row: **22%** | Of column: **58%**<br>Of row: **78%** | 9     |
| Total               | 16                                    | 12                                    | 28    |
(In the previous examples, the actual number and the ratio were given. This does not always have to be the case. At times, you may receive one or the other.)
# Potential Mistakes
1. Make sure that you are looking at the row/column to address the question.
   
   For example, what percentage of Yankees fans are men? And what percentage of men are Yankees fans?
   
   For the first question, you look at the Yankees fans/men cell and compare that to the rest of the **row** (90%). For the second question, you look at the Yankees fans/men cell and compare that to the rest of the **column** (56%).
   
   It's not complicated, but it is easy to make mistakes.
   
2. When only given only column or row ratios (and you aren't given total amounts), there are some questions you will not be able to answer from the data.
   
   In the following example, ratios are given for the columns:

|                    | Has driver's license | Doesn't have driver's license |
| ------------------ | -------------------- | ----------------------------- |
| Got into accident  | 20%                  | 45%                           |
| Never had accident | 80%                  | 55%                           |
It may appear that more people without driver's licenses get into accidents than people with one. However, that isn't necessarily the case from the data. It is possible that there are far more people with driver's licenses than without. For example, if 100 people have driver's licenses and 20 don't, then 20 people with driver's licenses got into an accident (20% of 100), and 9 people without a driver's license did (45% of 20). So if all you know about someone is that they got into an accident, it would be more likely that he/she has a driver's license than doesn't have one (20/29). 

This makes sense because in our example, there are far more people with driver's licenses, so the baseline assumption should be that someone has a driver's license if you nothing about them at all (100 people have a license/120 total people). Getting into an accident makes it less likely that the person has a license (100/120=83% vs 20/29=69%) but there is still a greater than 50% chance that the person has a license.

You can answer questions about relative frequency. You can say that it is more likely for someone who doesn't have a driver's license to get into an accident (45%) than it is for someone who does (20%).