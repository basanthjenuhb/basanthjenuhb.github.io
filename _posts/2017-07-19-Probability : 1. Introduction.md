---
published: true
---
Welcome to my first post on Probability. This is a series of posts giving you a glimpse of an undergraduate course on Probability and statistics. These posts are are an overview of <a href="https://projects.iq.harvard.edu/stat110" target="_blank">Statistics 110: Probability</a> by Harvard.
<!--more-->

Before diving right in, I recommend you to go through the <a href="https://projects.iq.harvard.edu/files/stat110/files/math_review_handout.pdf" target="_blank">Math review.</a>.

I would like to start by telling you that **Probability** deals with the measure of uncertainty. So, all we will be doing here is quantifying uncertainty. Now, before I give you a definition of probability, I should tell you what a **Sample space** and an **Event** is.

> **Sample Space** - It is a set of all possible outcomes of an experiment. Here we will denote it by "S".

> **Event** - An event is a subset of a sample space.

You can have numerous examples for this. If you experiment is flipping a coin, then the sample space would be **S = { Head, Tail }**. An event here would occurrence a head or a tail or both. Likewise, if your experiment is rolling a dice, then the sample space would be **S = { 1, 2, 3, 4, 5, 6 }**. An event here would be occurrence of 1 or 2 or 3 ...etc or a combination of those. Now, the **naive** definition of probability is very simple. Consider a sample space **S** and an event **A** we are interested in. The probability **P** of occurrence of an event **A**, written as **P(A)**, is given by:

$$ P(A) = \frac{\#\ Favourable\ outcomes}{\#\ Possible\ outcomes} $$

We will solve a simple problem. Consider rolling a dice. What is the probability that a number less than 4 occurs. Now, the set of all possible outcomes(Sample Space) is **S = { 1, 2, 3, 4, 5, 6 }** and the set of favourable outcomes is **A = { 1, 2, 3 }**. So,

$$ P(A) = \frac{\#\ Favourable\ outcomes}{\#\ Possible\ outcomes} = \frac{|\ A\ |}{|\ S\ |} = \frac{3}{6} = \frac{1}{2}  $$

Now, I call this definition of probability **naive** because it fails at many places:
1. It assumes that all outcomes are equally likely. That is, **P(Head) = P(Tail)**. But, this definition would fail when the coin used in the experiment is biased. i.e the coin for which the probability is not 1/2 is called a biased or unfair coin.
2. It assumes that the sample space is finite. Now, this definition would fail when the sample space is, say a set of real numbers in $[-3,\ 3]$. This set contains infinitely many numbers and we would end up substituting $\infty$ in the denominator.

Still, this definition should be able to take us far in understanding probability.

So, this was a very brief introduction to probability. In the next post, we will see how we **count** stuff. By that what I mean is, you can easily count the number of possible outcomes of an experiment with a single die or a single coin. What would you do if you had, say a 100 dice in the experiment or a 100 coins in the experiment.

Feel free to comment if you have any queries or suggestions. See you in the next post.
