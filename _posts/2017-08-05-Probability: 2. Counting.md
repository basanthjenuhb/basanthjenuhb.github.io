---
published: true
---
Welcome to my second post on probability and today will be all about counting. This post will give you a brief understanding of how to count different possibilities when there are many sub experiments involved in an experiment.

<!--more-->
Before diving right in, I recommend you to go through my <a href="https://basanthjenuhb.github.io/2017/07/19/Probability-1.-Introduction/" target="_blank">previous post</a>.

I'll start by giving you an example. Let's say that Ross is tired after work and wants to have an ice cream. He goes to the ice cream shop and has a lot of options to choose from. When it comes to con, he can choose between a **cake** cone and a **waffle** cone.
<center>![Cone](http://media.gettyimages.com/photos/two-ice-cream-cones-picture-id78907703?s=612x612)</center>
When it comes to flavors, he can choose between **chocolate**, **vanilla** or **strawberry**. So, the experiment of choosing ice-cream consists 2 sub-experiments:
1. Choose a cone - 2 possibilities ( **Cake** or **waffle** )
2.  Choose a flavor - 3 possibilities ( **chocolate**, **vanilla** or **strawberry** )

So, the total number of possibilities to choose an ice-cream would be: 
$$\# sub\ experiment\ 1\  \times \# sub\ experiment\ 2 = 2 \times 3 = 6$$For every cone you choose, you can choose to have any of the flavors on it. It can also be:
$$\# sub\ experiment\ 2\  \times \# sub\ experiment\ 1 = 3 \times 2 = 6$$ This is because the owner of the ice-cream shop is not going to force you to choose the waffle or the flavor first.

This brings us to the **multiplication rule**.

> Consider a compound experiment **$A$** consisting of $r$ sub experiments. Let the sub experiment $A_1$ consist of $n_1$ possibilities, $A_2$ consist of $n_2$ possibilities.... $A_r$ consist of $n_r$ possibilities. Then the total possibilities of overall experiment would be:

> $$n_1 \times n_2 \times n_3 ... n_r$$

Now, we will move on to make something called a **Sampling table**. Consider you have a bag of balls labelled $1,2,3...n $.

![Labelled balls](https://image.shutterstock.com/z/stock-photo-isolated-colored-pool-balls-numbers-to-and-zero-ball-77575132.jpg)

From this bag, you have to choose $k$ balls with some constraints. The different constraints are:
### **1. With replacement, Order matters**
So, you have to fill up $k$ positions using $n$ balls. Since it is with replacement, the same ball can be chosen multiple times. Let us see the different $\#$ possibilities for different positions.
1. The bag contains $n$ balls to choose from, so we have $n$ possibilities for position 1.
2. The bag still contains $n$ balls because the previous ball is replaced after choosing. So, again we have $n$ possibilities for position 2.
And the same goes on till position $k$. So, the total possibilities in the overall experiment are:
$$n \times n \times n \ .....(k\ times) = n^k$$

### **2. Without replacement, order matters**
The different $\#$ possibilities for different positions are:
1. The bag contains $n$ balls to choose from, so we have $n$ possibilities for position 1.
2. Since the previous ball is not replaced, we have $n-1$ balls to choose from for position 2.
3. Since none of the previous balls are replaced, we have $n-2$ balls to choose from for position 3.
$k$. In the same way, we have $n-k+1$ balls to choose from for the $k^{\textrm{th}}$ position.
This goes on till we fill all $k$ positions. So, the total $\#$ possibilities in the overall experiment are:
$$n \times (n-1) \times (n-2) \times (n-3)\ ...\ (n-k+1) = \ ^nP_k = \frac{n!}{(n-k)!}$$
### **3. Without replacement, order doesn't matter**
We can derive this using the above equation. Since order doesn't matter to us, we just need to divide the above equation by $k!$ since we have overcounted. The equation would be:
$$\frac{n \times (n-1) \times (n-2) \times (n-3)\ ...\ (n-k+1)}{k!} = \ ^nC_k = \frac{n!}{(n-k)!\times k!}$$

### **4. With replacement, order matters**
The total $\#$ of possibilities is $\ ^{n+k-1}C_k$. Please refer to <a href="https://youtu.be/FJd_1H3rZGg?list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo&t=706" target="_blank">Stat 110 - Lecture 2</a> for the proof.

With this, we can go on and fill the sampling table.

|      Type/Order     	| Order matters 	| Order doesn't matter 	|
|:-------------------:	|:-------------:	|:--------------------:	|
|   With replacement  	|     $n^k$     	|    $\ ^{n+k-1}C_k$   	|
| Without replacement 	|   $\ ^nP_k$   	|       $\ ^nC_k$      	|

These lectures are based on [Stat 110](https://www.youtube.com/watch?v=KbB0FjPg0mw&list=PL2SOU6wwxB0uwwH80KTQ6ht66KWxbzTIo). Please feel free to comment in case of any queries or suggestions.
