<h1>
    <center>Probability & Statistics </center>
</h1>
<center>Portfolio</center>
<center>Antea Giljanovic, Spring Semester, 2021</center>

[TOC]

# `Before We Begin`

Before we get into it, I would like to explain that this portfolio is to be a learning guide for anybody who has an interest in probability and statistics, whether it be a newcomer or not. I believe concepts should be explained simply enough to spark interest even in those who never imagined reading through a math book.

So take your time, and read through and learn together with me, as this portfolio is also my learning journey.



With that said, how would I actually explain probability and statistics, you ask? Well, all probability questions are out to get the an answer from the same type of a question:

> Out of X amount of possible outcomes, how often will Y happen?

To simplify it even further, we can use simple problems. For example, take three plastic cups and a coin. ![cup and coin](images\cup and coin.png) 

So, now we want to know what is the probability of the coin being under cup A. Let's look at all of the possibilities:

> 1. The coin is under cup A
> 2.  The coin is under cup B
> 3. The coin is under cup C

Next thing you would do is count how many of those cases the coin is under cup A.![cup and coin1](images\cup and coin1.png)

Turns out, it's just one. This means that the odds are 1/3. You can also do this in reverse, for example, what are the odds that the coin is not under the cup? It's not under B or C, so it's 2/3.

That's what statistics is, but as the problems get more complicated (a thousand cups and a hundred coins; or even trying to figure out the odds that a coin will be under the same cup 10 times in a row), the math of how you calculate the estimate of the total outcomes gets steadily more and more complex.



---

![cards](images\cards.png)



# `Probability`

> **Probability theory**, a branch of mathematics concerned with the analysis of random phenomena. The outcome of a random event cannot be determined before it occurs, but it may be any one of several possible outcomes. The actual outcome is considered to be determined by chance.

Probability theory is a mathematical framework we use to analyze these random events in a logically sound manner.

Before I dive deeper into the topic, I want you to familiarize yourself with the basic of probability, to avoid any confusion that may come up later on.



## **Terms**

**Population**

- The entire group that you gather information from

**Sample**

- Subset of the population you're gathering the data from, because analyzing  the entire population is not possible as it is too large. However, its characteristics are still representative of the population.

**Mean**

- Otherwise known as arithmetic mean or average. Click [here](#Expected-Value) to read more about it.

**Median**

- The value separating the lower from the higher half of the population. We get this value by arranging all the values from the lowest to the highest and taking the middle one.

**Variance**

- Measures dispersion around the mean. Click [here](#variance) to read more about it.


**Standard Deviations**

- Square root of the variance, also measures the dispersion around the mean, but in the same units as the values. Click [here](#standard-deviation) to read more about it.

**Standard Error**

- An estimate of the standard deviation, and it reflects the extent to which a statistic changes from sample to sample.



---

## **Sample Space**

![sample space](images\sample space.png)The entire possible set out outcomes is called a sample space, and it's most often marked with the Greek letter Omega(**Ω**).

Put simply, if we have a die, the sample space, or all of the possible rolls we can get, would be be between the numbers 1 and 6, written so:

<center><b>Ω = {1,2,3,4,5,6}</b></center>



## **Events**

While doing an experiment, we're often doing it with the intent of looking for an outcome — an event. 

Depending on the outcome, there's various types of events, too.![bubble](images\bubble.png)

### Simple Events

An event with a single outcome. 

If we are rolling a die, and only looking for 1, we would write it so:

<center><b>E = {1}</b></center>



### Compound Events

Contrary to the simple event, if an event consists of more than one point of sample space, then we call this a **compound event**. 

For example, if we're only looking for uneven numbers while throwing a die.

<center><b>E = {1,3,5}</b></center>



### Impossible and Sure Events

<img src="images\likelyhood.png" alt="likelyhood" style="zoom: 50%;" />



The probability of an event happening is a number indicating how likely that event will occur. This number is always either 1 **(sure event)**, meaning certainty that the event will occur, and 0 indicating that it's impossible **(impossible event)**. 

*For example:*

> **Impossible event**
>
> ​		Obtaining 7 on a fair number cube throw
>
> **Sure event**
>
> ​		Obtaining a number less or equal to a 6 on a fair number cube throw



### Independent Events and Dependent Events

If the occurrence of one event is not affected by another, then this is called an **independent event** *(left image)*. The opposite would be called a **dependent event** *(right image).*![bubble ab](images\bubble ab.png)

For example:

> **Dependent Events:**
>
> 1. If you park illegally, you're likely to get a parking ticket.
> 2. Committing a crime, such as robbery, increases your odds of getting caught and going to jail.
>
> 
>
> **Independent Events:**
>
> 1. Growing the perfect strawberry and owning three cats
> 2. Finding a dollar on the street and winning the lottery



### Complementary Events

For every single E event, there's a corresponding Ē, which is the set out outcomes that are not included in the event space, but are a part of the sample space. They are called **complementary events.**

In the example of odd numbers, the complementary events are the odd numbers.

<center><b>E = {1,3,5}</b></center>

The outcome of an event combined with the complementary events make up the entire sample space. 

E and Ē are disjoint, and it **is impossible for an event and its complement to occur at the same time.**

The rule for complementary events is the following:



<center><b>P(Ē) = 1 - P(E)<br> P(E) + P(Ē) = 1 <br> P(E) = 1 - P(Ē)</b></center>



### Mutually Exclusive Events

If two events are mutually exclusive, or in other words, disjointed, they cannot happen at the same time.

*For example:*

> You cannot run backwards and forwards at the same time.
>
> You cannot toss a coin and land both heads *and* tails.



### Exhaustive Events

If the event consumes the entire sample space, we call this an **exhaustive event.**

*For example:*

> A coin is tossed, and we have 2 events.
>
> Event H = if head is tossed
>
> Event T = if tails appears

Because either one of the events will occur during the conduct of the experiment, both events together are an exhaustive event.



## **Expected Value**

<img src="images\expected value.png" alt="expected value" style="zoom: 50%;" />



The expected value of a random variable X, is a number that represents the weighted average of that random variable's distribution. It is defined as the probability-weighted sum of all possible values in the random variable's support. In other words, it's *"the value you will get on average".*

**The mean and the expected value are so closely related they are basically the same thing.** 

*To explain it a bit easier:*

> For example, if you take a 20 question multiple-choice test with A,B,C,D as the answers, and you guess all “A”, then you can expect to get 25% right (5 out of 20). 
>
> The **math** behind this kind of expected value is:
>The probability (P) of getting a question right if you guess: .25
> The number of questions on the test (n)*: 20
>
> **P x n = .25 x 20 = 5**

The basic expected value formula is the probability of an event multiplied by the amount of times the event happens:
$$
(P(x) * n)
$$

### Expected Value for Multiple Events

> You buy one $10 raffle ticket for a new car valued at $15,000. Two thousand tickets are sold. What is the EV of your gain?  

You would use the following formula to find out:
$$
E(X) = ΣX * P(X)
$$



### Expected Value Formula for an Arbitrary Function

If an event is represented by a function of a random variable (g(x)) then that function is substituted into the EV for a continuous random variable formula to get:
$$
\mathrm{E}[g(X)]=\sum_{x} g(x) f(x)
$$





# `Set theory`

A *set* is a collection of things, called *elements*, without any repeats. Sets are usually written with curly brackets and commas to distinguish between the various elements:

<center><i>A = {1, 2, 3}</i></center>



## **Standard Sets**

There are a few sets that occur naturally in math,

- Set of natural numbers. *(ℕ = {1, 2, 3, …})*
- Set is for integers. ℤ = {…, -2, -1, 0, 1, 2,…}
- Set of all rational numbers. ℚ = {9/4, -1, 0.5, 4/6, …}
- Set of all real numbers. ℝ = {3.14…, 2/5, 8, …}
- Set of complex numbers. ℂ = {√-4, 3 + 4i, …}.
- The universal set. Its symbol is *S* and it is the set that contains every value of the population that you are interested in and the subset.



## **Union**

Sets can overlap. *For example, set A = {1, 2, 3, 4} and B = {2, 4, 6, 8}.*

This overlap is written as A ∪ B = {1, 2, 3, 4, 6, 8}

![Set-Drawings-300x277](images\Set-Drawings-300x277.png)



## **Intersect**

Sometimes, we are only concerned with the overlap of two or more sets. If A = {1, 2, 3, 4, 5, 6} and B ={2, 4, 6} the overlap would be 2, 4, and 6. We call this an **intersect** in set theory and we write it like A ∩ B.

![Set-Drawings-1-300x208](images\Set-Drawings-1-300x208.png)



## **Complement**

Sometimes, we are concerned with what is *not* in the set, or what the set takes away from the universal set. 

We can consider the **complement** of a set to be the elements that are in the universal set, *S* but not in the set itself.

![Set-Drawings-2-300x208](images\Set-Drawings-2-300x208.png)

*For example:*

> You have a six-sided die. The universal set is *S* = {1, 2, 3, 4, 5, 6}. 
>
> Let’s take it a step further and say that set A within the universal set is A = {2, 4, 6}. That means that 1, 3, and 5 are left over in the universal set. These elements make up the complement of A (Ac) because they are in the universal set, but *not* in A, or Ac = {1, 3, 5}



## **Difference**

Sets can be subtracted from one another. In the case of A – B, subtraction means not only taking out B, but also the components that intersect A and B.

So, if we had A = {1, 2, 3, 4, 5, 6} and B = {2, 4, 6, 8} then A – B = {1, 3, 5}. 

![Set-Drawings-3-300x208](images\Set-Drawings-3-300x208.png)

The subtraction of sets is not entirely like the subtraction of numbers. A – B does not equal B – A because the sets contain different elements, so you may not be removing the same elements from both sets.



## **Disjoint**

If the sets do not overlap or have no elements in common, they are called **disjoint** sets. This means that if were were to think about an overlap (A ∪ B) there would be none or A ∪ B = Ø.

![Set-Drawings-4-300x208](images\Set-Drawings-4-300x208.png)



## **Partition**

When a set is divided into distinct and disjoint sets, each of those sets are **partitions** of the larger *(usually universal)* set.

In a partitioned set, the union of the partitions gives the overall set. So in the diagram below, A1, A2, A3, and A4 are partitions of the overall set A.

![Set-Drawings-5-300x208](images\Set-Drawings-5-300x208.png)



## **Bijection, Injection, and Surjection**

<img src="images\bijection, injection, surgection.png" alt="bijection, injection, surgection" style="zoom: 50%;" />

**These are the following functions:**

**Injections** (**one-to-one functions**)

- A function that always maps the distinct  element of its domain to the distinct element of its codomain.

- *f* is *injective* if distinct elements of X are mapped to distinct elements of *Y*.

$$
\text {if } f(x₁) =f(x₂)\text{, then } x₁ = x₂
$$



**Surjections** (**onto functions**)

- A function that maps one or more elements of A to the same element of B

- *f* is *surjective* if every element of *Y* is the image of at least one element of X.

$$
\forall y \in Y, \exists x \in X \text { such that } f(x)=y
$$



**bijections** (both **one-to-one** and **onto**)

- A function that is both injective and surjective.

- *f* is *bijective* if it is both of the previous cases; that is, every element  y ∈ *Y* is the image of *exactly one* element  x *∈* X.

$$
\text { A → B}
$$
- The above function is a bijective function if every element b ∈ B and every element a ∈ A, such that f(a) = b.
- This concept allows us to compare cardinalities of sets, with proofs comparing the sizes of both finite and infinite sets.




## **Cardinality**

Cardinality of a set is the measure of the set's size, so, how many elements there are in a set. If we look at the example set *A={1,2,3}*, we can see that it has a cardinality of 3 for the 3 elements that it has in it. The cardinality of a set is denoted by vertical bars, for example ∣*A*∣.
$$
\text{Two sets A and B are the same cardinality if there exists a bijection A→B}
$$
To avoid possible confusion, read the definition as: 
$$
\text{f:{integers} → {even integers} where f(n) = 2n}
$$

> In terms of cardinality, the size of the set of all integers is exactly the same as the size of the set of even integers.



### Countability and Uncountability

An infinite set **A** is called countably infinite (or countable) if it has the same cardinality as **N**. In other words, there is a bijection **A** to **NA→N**.

An infinite set **AA** is called uncountably infinite (or uncountable) if it is not countable. In other words, there exists no bijection **A** to **NA→N**.



**Countable:**

> Let Z = {…,−2,−1,0,1,2,…} denote the set of integers. Is Z countable or uncountable?
>
> Consider the following map from N to Z :N→Z:
> $$
> \text{{1,2,3,4,5,6,7,8,9,…}↦{0,1,−1,2,−2,3,−3,4,−4,…}.}
> $$
> Each integer is mapped to by some natural number, and no integer is mapped to twice. Thus, this is a bijection. We conclude Z is countable.



**Uncountable:**

> Consider the interval [0,1] As a set, is [0,1] countable or uncountable?
>
> Suppose [0,1] is countable, so that we may write [0,1] ={*a*₁,*a*₂,*a*₃,…}, where each aᵢ ∈ [0,1]. For each aᵢ, write (one of) its binary representation(s):
> $$
> a_{i}=0 . d_{i 1} d_{i 2} d_{i 3} \ldots_{2},
> $$
> where each dᵢ ∈ {0,1}.
>
> For each i, let eᵢ = 1 - dᵢᵢ, so that eᵢ = 0 if dᵢᵢ = 1 and eᵢ = 1 if dᵢᵢ =0. Now, construct a number x ∈ [0,1] by writing down its binary representations:
> $$
> x=0 . e_{ 1} e_{2} e_{3} \ldots_{2},
> $$
> Since x differs from aᵢ in the iᵗʰ binary digit, we know x ≠ aᵢ for all i ∈ N.
>
> But...this means x is not in the list {*a*₁,*a*₂,*a*₃,…}, even though x ∈ [0,1]. Thus, the list does not include every element of the set [0,1], contradicting our assumption of countability.



## **De Morgan's Law**

**De Morgan’s Laws** are the theoretical way that sets can be transformed. 

<img src="images\de-morgans-law.png" alt="de-morgans-law" style="zoom: 67%;" />

Think of A1 ∩ A2 is the intersection of two sets. So, what is the complement of the intersection? Everything else! So, the complement of an intersection is the union of remaining complements. It is typically written as

(A1 ∩ A2)' = A1' ∪ A2'

The opposite is also true

(A1 ∪ A2)' = A1' ∩ A2'



## **Distributive Law**

Using the **distributive law**, you can relate sets through union and intersection. The law states that taking the union of a set to the intersection of two other sets is the same as taking the union of the original set and both the other two sets separately and then taking the intersection of the results.

<img src="images\distrib2.gif" alt="distrib2" style="zoom:150%;" />



It is written as:

A ∩ (B ∪ C) = (A ∪ B) ∩ (A ∪ C) or A ∪ (B ∩ C) = (A ∩ B) ∪ (A ∩ C)





# `Combinatorics`

<img src="images\9b65a21.png" alt="9b65a21" style="zoom:67%;" />



Combinatorics is the mathematics of counting and arranging, especially when it comes to quantities that are much too large to be counted the conventional way.



## Rule of Product and Sum

**Rule of Product**

- *If there are m ways to arrange something, and then n ways to arrange something else after that, then the number of ways to arrange both of those things is m×n.*

**Rule of Sum**

- *If there are m ways to arrange something, and there are n ways to arrange something else, and these arrangements cannot both happen, then the number of ways to arrange either of those things is m+n.*



The wording of the two rules is extremely similar, but the main difference is that arrangements counted with the rule of product happen consecutively or simultaneously, while arrangements counted with the rule of sum *cannot* happen consecutively or simultaneously.

*Example:*

> How many integers between 1 and 100 are divisible by 7 or 13?
>
> ---
>
> The number of integers between 1 and 100 that are divisible by 7 is 100 / 7 = 14.
>
> The number of integers between 1 and 100 that are divisible by 13 is 100 / 13 = 7.
>
> The sum of integers between 1 and 100 that are divisible by 7 and 13 is 100 / (7x13) = 1
>
> The rule of sum would apply here, 7 + 14 = 21, but to avoid double counting, we will subtract the 1 that we just calculated.
>
> ---
>
> Therefore, there are 20 integers between 1 and 100 that are divisible by 7 or 13.



## Permutations and Combinations

### **Permutation** 

A **permutation** is an arrangement of objects with regard to order.

*Example:*

> How many permutations are there of the letters ABC?
>
> ABC, BCA, ACB, CAB, BAC, CBA.
>
> So, 6 permutations.

There are *n* ways to choose the first object in the order. Then, there are *n*−1 ways to choose the second object in the order. This continues until there is only 1 way to select the last object in the order. 



- By the rule of product, the number of permutations of *n* objects is:

$$
n \times(n-1) \times(n-2) \times \cdots \times 2 \times 1=n !
$$



- Given a set of *n* objects, let the set of permutations of *k* of those objects be *S*. Then,

$$
|S|=\frac{n !}{(n-k) !}
$$

*Example:*

> If there are 25 railway stations on a railway line, how many types of single second-class tickets must be printed, so as to enable a passenger to travel from one station to another?
> $$
> |S|=\frac{25!}{(25-2) !} = 600
> $$
> It's like picking two stations from 25 stations. The order of (start & destination) stations matter, i.e. A->B is not same as B-> A.



---

### **Combination**

A **combination** is an arrangement of objects without regard to order.



- Given a set of *n* distinct objects, let *C* be the set of combinations of *k* of those objects. Then,

$$
|C|=\left(\begin{array}{l}
n \\
k
\end{array}\right)=\frac{n !}{k !(n-k) !}
$$



- The number of permutations of *k* objects from a set of *n* objects is n! / (n-k)! . For each subset of *k* objects from the set of *n* objects, there are k*! permutations of that subset. Therefore, the number of combinations of *k* objects from a set of *n* objects is:

$$
\frac{n !}{(n-k) !} \div k !=\frac{n !}{k !(n-k) !}=\left(\begin{array}{l}
n \\
k
\end{array}\right)
$$

*Example:*

> How many distinct triangles can be formed from 10 points on a plane, no 3 of which are co-linear?
>
> ---
>
> Each triangle can be formed from any 3 of the 10 points. This corresponds to combinations of 3 objects out of 10. 
>
> So, the number of triangles that can be formed is:
> $$
> \binom{10}{3}=\boxed{120}
> $$
> The assumption that "no 3 of the points are co-linear" is important for this problem. Without this assumption, a combination of 3 points would not make a triangle if those points were on the same line.



*Example:*

> A bag contains 4 of each color of marble: red, orange, green, blue, and purple. 3 marbles are drawn from the bag (without replacement).
>
> If a/b is the probability that the drawn marbles are different colors, where *a* and *b* are coprime positive integers, then what is a*+*b*?
>
> ---
>
> Treat each marble in the bag as distinct, and consider the combinations of 3 marbles that are different colors. 
>
> When it comes to selecting the color of those 3 marbles, there are this many ways to do it:
> $$
> \left(\begin{array}{c}
> 5 \\
> 3
> \end{array}\right)
> $$
> There's also the following number of ways to select the marbles from each of those colors:
> $$
> \left(\begin{array}{c}
> 4 \\
> 1
> \end{array}\right)^{3}
> $$
> Finally, the total number of ways to select 3 marbles from the bag is:
> $$
> \left(\begin{array}{c}
> 20 \\
> 3
> \end{array}\right)
> $$
> Knowing all of this now, the probability that the 3 drawn marbles are different color is:
> $$
> \frac{\left(\begin{array}{c}
> 5 \\
> 3
> \end{array}\right)\left(\begin{array}{c}
> 4 \\
> 1
> \end{array}\right)^{3}}{\left(\begin{array}{c}
> 20 \\
> 3
> \end{array}\right)}=\frac{640}{1140}=\frac{32}{57}
> $$
>
> $$
> a+b=\boxed{89}
> $$



## Binomial theorem

The Binomial Theorem is a quick way of expanding a binomial expression that has been raised to some power. 

For instance, the expression (3*x* – 2)¹⁰ would be very painful to multiply out by hand. Good thing that we have a formula for this expansion, and we can plug the binomial 3*x* – 2 and the power 10 into that formula to get that expanded form.



**Binominal expansion:**
$$
\left(\begin{array}{l}n \\ k\end{array}\right)=\frac{n !}{(n-k) ! k !}
$$

$$
(x+y)^{n}=\sum_{r=0}^{n}\left(\begin{array}{l}
n \\
r
\end{array}\right) x^{n-r} y^{r}=\sum_{r=0}^{n}\left(\begin{array}{l}
n \\
r
\end{array}\right) x^{r} y^{n-r}
$$



**Binominal theorem states that for any positive integer n, we have:**
$$
(x+y)^{n}=\left(\begin{array}{l}
n \\
0
\end{array}\right) x^{n}+\left(\begin{array}{l}
n \\
1
\end{array}\right) x^{n-1} y+\cdots+\left(\begin{array}{c}
n \\
n-1
\end{array}\right) x y^{n-1}+\left(\begin{array}{l}
n \\
n
\end{array}\right) y^{n}
$$

$$
=\sum_{k=0}^{n}\left(\begin{array}{l}
n \\
k
\end{array}\right) x^{n-k} y^{k}
$$



*Example:*

> A friend says that she will flip a coin 5 times. Each time the coin comes up heads, she will give you $10, but each time the coin comes up tails, she gives nothing. What is the probability that you will win $30 playing this game?
>
> ---
>
> The binomial theorem tells us that 5 chose 3 = 10 of the 2⁵ = 32 possible outcomes of this game have us win $30. Therefore, the probability we seek is
> $$
> \frac{\left(\begin{array}{l}
> 5 \\
> 3
> \end{array}\right)}{2^{5}}=\frac{10}{32}=0.3125
> $$



### Binomial coefficient

Binomial coefficients are the ones that appear as the coefficient of powers of *x* in the expansion of (1+x)ⁿ:
$$
(1+x)^{n}=n_{c_{0}}+n_{c_{1}} x+n_{c_{2}} x^{2}+\cdots+n_{c_{n}} x^{n}
$$
where n꜀ₖ = n! / (k!(n-k)!). The terms from n꜀ₒ and n꜀ₙ are called binominal coefficients. So, from here on out I will write n꜀ₖ as:
$$
\left(\begin{array}{l}
n \\
k
\end{array}\right)
$$
*Example:*

> In how many ways could you choose a three-topping pizza based on the following menu?
>
> Pizza toppings: pepperoni, sausage, ham, bacon, chicken, onion, mushroom, pepper, olives, pineapple.
>
> ---
>
> The number of ways to choose 3 elements out of a set of 10 is:
> $$
> \left(\begin{array}{c}
> 10 \\
> 3
> \end{array}\right)=\frac{10 !}{7 ! 3 !}=\frac{10 \cdot 9 \cdot 8}{3 \cdot 2 \cdot 1}=\frac{720}{6}=120
> $$



### Pascal's Triangle

Another way to calculate the value of ₙCᵣ is Pascal's Triangle.

To make this triangle, we start with a pyramid of three 1s.

![binom06](images\binom06.gif)

Then we can start get the second row of numbers by adding the pairs of numbers of above. (If there's nothing to combine, it continues with 1.)

![binom07](images\binom07.gif)

And we keep going, always adding pairs from the previous row. 

To find 6C4, you would go down to the row where it says 6, and then over to the 5th entry, to find out that 6C4 is 15.

![binom09](images\binom09.gif)

While the triangle visually explains what's going on, it's a very time consuming process.



# `Probability and Counting Rules`

There are thee basic interpretations of probability:

- *Classical probability*

- *Experimental probability*

- *Subjective probability*

  

## **Probability rules**

- **For any event A, 0 ≤ P(A) ≤ 1.**

  - *Example: Doing research on the frequency of occurrence of blood types:*

    > ​	What is the probability of a person having blood type A?
    >
    > |   BLOOD TYPE    |  O   |  A   |  B   |  AB  |
    > | :-------------: | :--: | :--: | :--: | :--: |
    > | **PROBABILITY** | 0.44 |  ?   | 0.10 | 0.04 |
    >
    > Summing the probabilities of A,B, and AB we get: 0.44 + 0.1 + 0.04 = **0.58**
    > Therefore, the probability of A is the remaining **0.42** *(1-0.58=0.42)*

  

- **The sum of the probabilities of all possible outcomes is 1.**

  * This directly ties in with the previous task, summing all of the outcomes together, we get 1. 

    > ‎![image012](images\image012.gif)
    >
    > *(0.44+0.42+0.10+0.04 = 1)*
    
    

- **The probability that an event does not occur is 1 minus the probability it does occur,** **P(notA) = 1 - P(A)**

  - *Going back to the blood type example:*

    > What is the probability that a randomly chosen person does not have blood type O?
    >
    > ‎![image014](images\image014.gif)
    >
    > Using the rule we get: P(not O) = 1 – P(O) = 1 – 0.44 = 0.56. 
    >
    > The odds that the person does not have blood type O is 56%.



- **If A and B are disjoint events, then P(A or B) = P(A) + P(B).**

  ![image015](images\image015.gif)

  ![image016](images\image016.gif)
  
  - *Example:*
  
    > What is the probability that a random person is a potential donor for a person with blood type A?
    >
    > In order to donate blood to A, you have to have blood type A or O, and since those 2 events are disjoint we can calculate them like this:
    >
    > ​	P(A or O) = P(A) + P(O) = 0.42 + 0.44 = **0.86.**



- **General addition rule states that for any two events, P(AorB) = P(A) + P(B) - P(A and B)**

  - in the case of disjoint events, we would use the following: **P(A or B) = P(A) + P(B)**.

  - *Example:*

    > We are sending a parcel, and it's necessary that it reaches its destination within one day. These are the following probabilities:
    >
    > 0.90 for service A, 0.80 for service B, 0.75 for both being on time<img src="images\probabilityrule5c.png" alt="probabilityrule5c" style="zoom:80%;" />
    >
    > **P(A or B)= P(on-time delivery using this strategy)= 0.90 + 0.80 – 0.75 = 0.95.**



- **Multiplication rules for Probability**

  - Used to find the probabilities of two or more events that occur in sequence

    - **When two events A and B are independent, then P(A and B) = P(A)P(B)**

    - *Example:*

      > You're playing lottery, and you're curious the odds that your specific sequence will be chosen. We can use the following rule to calculate 	the likelihood of our specific sequence occurring:
      > $$
      > \mathrm{P}(\text { Sequence } 9-1-1)=\frac{1}{10} \times \frac{1}{10} \times \frac{1}{10}=\frac{1}{1000}=0.001
      > $$




- **Rounding rule for Probability**
  
  - In general you should carry probabilities to at least 4 decimal places for intermediate steps.
  - We often round our final answer to two or three decimal places.
  - For extremely small probabilities, it is important to have 1 or two significant digits (non-zero digits), such as 0.000001 or 0.000034, etc.



## **Theoretical probability**

Also called the classical probability, it's the mathematical way of calculating how likely something is going to occur; it's a probability based on an ideal situation. 

- Performing an experiment is not necessary. 
- We assume that all outcomes are equally likely to occur

$$
P(\text { event })=\# \text { of favorable outcomes : total # of outcomes }
$$
*For example let's take the die example:*

> We're interested in the probability of throwing a die and getting a 6.
>
> First of all, what are all of the possible outcomes:
>
> E = {1,2,3,4,5,6} ... So, the total possible outcomes is 6.
>
> Second, we're going to look at the number of favorable outcomes: 
>
> Favorable outcome = rolling a 6
>
> And then we can find the ratio using the formula from above
> $$
> P(\text { event })=\# \text { of favorable outcomes : total # of outcomes }
> \\ P(6) = 1:6
> $$



## **Experimental probability**

Unlike the theoretical probability, experimental, or otherwise known as the empirical probability, is found by repeating an experiment and observing the outcomes.
$$
(\text { Probability of an Event })P(E)=\ \frac{\text { Number of times an event occurs }}{\text { Total number of tries }}
$$
*For example a coin toss:*

> We toss a coin 10 times in a row, and it turns out that we get 2 tails and 8 heads.  With these experiments we can easily calculate the probability.
> $$
> P(tails)=\frac{\text { 2 }}{\text { 10 }} = 0.2
> \\P(heads)=\frac{\text { 8 }}{\text { 10 }} = 0.8
> $$
> Weird, that's not exactly what was expected according to the theoretical probability (50/50). 

This is because experimental probability is tied to the **law of large numbers.** 



### Law of Large Numbers

What this means is that, as the number of flips increases, the long-run frequency of heads is bound to get closer and closer to 50%. 

*Let's repeat the experiment again a 1000 times:*

> This time, we have a much different and more realistic result; 515 heads and 485 tails.
> $$
> P(tails)=\frac{\text { 485 }}{\text { 1000 }} ≈ 0.49
> \\P(heads)=\frac{\text { 515 }}{\text { 1000 }} ≈ 0.52
> $$
> Once this experiment has been repeated enough times, we can see that the experimental probability is nearing the theoretical probability of 0.5.



## **Conditional probability**

It's the probability that the event will occur given the knowledge that an event *A* has already occurred *P(B|A)*.  In the case where events *A* and *B* are independent, the conditional probability of event *B* given event *A* is simply the probability of event *B*, that is *P(B)*.

If events and A and B are not independent, then the probability that both events, A and B, occur is defined by:
$$
P(A and B) = P(A)P(B|A)
$$
From here, we need to obtain the conditional probability P(B|A), which is obtained so:
$$
P(B|A)=\frac{\text { P(AandB) }}{\text { P(A) }}
$$
*Example:*

> We're playing a card game, and in order to win, I have to draw 2 cards of the same suit in a row. Out of 52 cards, there are 13 cards in each suit.
>
> Suppose we draw clubs on our first try. This directly influences the desk, as now there are 12 clubs left in the deck of 51 cards.
> 
> P(Draw second club|First card a club) = **12/51**.



*Example number 2:*

> A student is applying to a university with a 80% acceptance rate, out of which 60% of the accepted students get dormitory housing. The chance to get both accepted and get dormitory housing is:
>
> *P(Accepted and Dormitory Housing) = P(Dormitory Housing | Accepted) P(Accepted) = (0.60)(0.80) = **0.48***
>
> 
>
> What if the student doesn't want to have a roommate though? We have to take all events into consideration now:
>
> P(A and B and C) = P(A)P(B|A)P(C|A and B)
>
> 
>
> Let's say that the accepted students, who have dormitory housing have a roommate 80% of the time. What are the odds that the student gets all 3 outcomes?
>
> P(Accepted and Dormitory Housing and No Roommates) =
>
> ​								= P(Accepted) P(Dormitory Housing|Accepted) P(No Roommates | Dormitory housing and accepted)
>
> ​								= (0.80) * (0.60) * (0.20) = **(0.096)**	
>
>
> So, he has roughly 10% of a chance to get a single room at the collage.



### Bayes's Formula

*The formula is based on the following expression:*
$$
P(B)=P(B \mid A) P(A)+P\left(B \mid A^{c}\right) P\left(A^{c}\right)
$$
What this means is that the probability of event *B* is the sum of the conditional probabilities of event *B* given that event *A* has or has not occurred. 

*For independent events A and B, it's the following:*
$$
P(B) P(A)+P(B) P\left(A^{c}\right)=P(B)\left(P(A)+P\left(A^{c}\right)\right)=P(B)(1)=P(B)
$$


>  since the probability of an event and its complement must always sum to 1 

*And finally the Bayes's formula is defined as follows:*
$$
P(A \mid B)=\frac{P(B \mid A) P(A)}{P(B \mid A) P(A)+P\left(B \mid A^{c}\right) P\left(A^{c}\right)}
$$
*Example of Bayes's formula in use  ([source](http://www.stat.yale.edu/Courses/1997-98/101/condprob.htm)):*

> A voting poll takes place in three different states. One state (A) has a 50% of voters who are supporting the liberal candidate, in the second state (B), 60% of the voters are supporting the liberal candidate, and finally in the third state (C), 35% of the voters are supporting the liberal candidate.
>
> Taking the population into consideration, 40% live in state A, 25% live in state B, and 35% live in state C. What are the odds that a voter who supports the liberal candidate lives in state B?
> $$
> P(StateB|LibVoter)=\frac{P(LibVoter|StateB)P(StateB)}
> {(P(LibVoter|StateA)P(StateA) + P(LibVoter|StateB)P(StateB) + P(LibVoter|StateC)P(StateC))}
> $$
>
> $$
> =\frac{(0.60)*(0.25)}
> {((0.50)*(0.40) + (0.60)*(0.25) + (0.35)*(0.35))}
> $$
>
> $$
> =0.3175.
> $$
>
>
> The probability that the voter lives in state B is approximately 0.32.



## **Subjective probability**

Refers to the probability of something happening based on the individuals own's assumptions or estimates. It's not based on market data or historical information, and it differs from one person to another, since it's based on an opinion and not facts. It's also subject to high degree of personal bias.

*Example:*

> My pet is sick, and I have to take it to the vet. I've been there before, so I'm pretty sure I'll need to bring more than 100 Euros with me.
>
> You think you have a 50/50 chance of getting the job, since the other candidate was as equally qualified.





# `Random Variable`

A random variable, usually written *X*, is a variable whose possible values are numerical outcomes of a random phenomenon. Actually, most of our observations are in the form of numerical data that are observed values of what is called a random variable.

Example:

> ‎![random-variable-1](images\random-variable-1.svg)
>
> Taking a coin example, let's assign Heads = 0, and Tails = 1
>
> X = {0,1}

The probability that X takes on a value in a measurable set  S ∈ E is written as:
$$
\mathrm{P}(X \in S)=\mathrm{P}(\{\omega \in \Omega \mid X(\omega) \in S\})
$$
There are two types of random variables, **discrete** or **continuous**. The main difference between the two categories is the type of possible values that each variable can take.

Random variables that can assume only a countable number of values are called **discrete**, while random variables that can take on any of the countless number of values in an interval are called **continuous**.



## **Discrete Random Variable**

![screte-probability-distrib](images\screte-probability-distrib.svg)

Discrete means countable, so a random variable that has a finite number of possible values or an infinite sequence of countable real numbers. They represent the number of distinct values that can be conducted in an event.

*Example:*

> The number of cars a car dealer sold in a month.
>
> The number of grammatical errors in an essay.
>
> The heights of students in the school.



**The probabilities pi must satisfy two requirements:**

1. Every probability pi is a number between 1 and 0.
2. p1 + p2 + p3  +... pₖ = 1

You can find the probability of any event by adding the probabilities pᵢ of the particular values xᵢ that make up the event.

*Example:*

> Coin toss has the outcomes of Ω = {heads, tails}. Let's introduce a real-valued random variable Y that models a 1$ payoff for a successful bet on heads as follows:
> $$
> Y(\omega)=\left\{\begin{array}{ll}
> 1, & \text { if } \omega=\text { heads } \\
> 0, & \text { if } \omega=\text { tails }
> \end{array}\right.
> $$
> if the coin is a far coin, Y has the probability mass function (exactly equal to some value) of:
> $$
> f_{Y}(y)=\left\{\begin{array}{ll}
> \frac{1}{2}, & \text { if } y=1 \\
> \frac{1}{2}, & \text { if } y=0
> \end{array}\right.
> $$



### Find an Expected Value for a Discrete Random Variable

 A discrete random variable is a random variable that can only take on a **certain number of values**. 

> For example, if you were rolling a die, it can only have the set of numbers {1,2,3,4,5,6}. 

The expected value formula for a discrete random variable is:
$$
E(X)=\sum_{x \in \Omega} x m(x)
$$



## **Continuous Random Variable**

![standard-deviation-diagram](images\standard-deviation-diagram.svg)

On the other hand, continuous random variable takes on values that vary continuously within one or more real intervals, and have a cumulative distribution function (CDF) that is absolutely continuous. Because of that, the continuous random variable has an uncountable infinite amount of possible values, all of which have a probability 0.



For any continuous random variable with a probability density function, is written so:
$$
\int_{\text {all } x} f(x) d x=1
$$


### Expected Value for Continuous Random Variables

The expected value of a random variable is just the **mean** of the random variable. You can calculate the EV of a continuous random variable using this formula:
$$
\mathrm{E}(x)=\int_{-\infty}^{\infty} x f(x) \mathrm{dx}
$$



# `Probability Distributions`

A probability distribution is a mathematical function that gives us the probabilities of occurrences of different possible kinds of outcomes for our experiments. 



## **Discrete distributions**

A discrete distribution is a statistical distribution that shows the probabilities of discrete, or countable, outcomes, such as 1, 2, 3, 4, 5...



###  Bernoulli distribution

A distribution with two possible outcomes that are labelled with: **n=0** and **n=1**.

**n=1** (*success*) occurs with the probability **p** ,while **n=0** occurs with the probability **1-p**.



The function that w write with a Bernoulli variable is:
$$
f(x)=\left\{\begin{array}{ll}
p^{x} *(1-p)^{1-x} & \text { if } x=0,1 \\
0 & \text { otherwise }
\end{array}=\left\{\begin{array}{cc}
p & \text { if } x=1 \\
1-p & \text { if } x=0
\end{array}\right.\right.
$$


The probability success of p is the parameter of the Bernoulli distribution.

If a discrete variable X follows that distribution we write it as:
$$
X \sim B e(p)
$$
*Example:*

> Betting on a coin flip that the outcome is going to be tails. The probability of getting tails is p=1/2. Therefore, once set tail=1 (win), and head (loss), we can calculate the probability of success like so:
> $$
> P(X=1)=f(1)=p=\frac{1}{2}
> $$



### Binomial distribution

![Binomial_distribution_pmf.svg_](images\Binomial_distribution_pmf.svg_.png)

The easiest way to remember and understand this distribution, is to understand it as a probability of either failure or success outcome in an experiment that is repeated several times.

#### *Conditions*

- The number of observations or trials is fixed
- Each observation or trial is independent
- The probability of success is the same from one trial to another.



*Example:*

> Let's continue with the coin experiment. You won your first bet and now you want to bet on more coins. So, now we're gonna flip a coin 5 times in a row, but how would we calculate the odds of winning?
>
> ![1_NIYiMJNSgYpnSy2drCNGqw](images\1_NIYiMJNSgYpnSy2drCNGqw.png)
>
> We flipped the coin 5 times and lost in the first three tries, and won in the final two.
>
> ![1_ng_nBgeOpMnBZLF9dT8EQw](images\1_ng_nBgeOpMnBZLF9dT8EQw.png)
>
> The zeroes representing losses (1-p), and ones representing victories (p), we get an idea how to calculate it.



#### *Properties of the Binomial distribution*

- The expected value, of a distribution gives useful information about what average one would expect from a large number of repeated trials.
- The median of a distribution is another measure of central tendency, useful when the distribution contains outliers that make the mean misleading.
- The mode of a distribution is the value that has the highest probability of occurring.
- The variance of a distribution measures how "spread out" the data is. Related is the standard deviation, the square root of the variance, useful due to being in the same units as the data.



### Poisson distribution

Used to model the number of events occurring in a given time period, given the average number of times the event occurs in said time period.



#### *Conditions*

- An event can occur any number of times during a time period.
- Events occur independently.
- The rate of occurrence is constant, so it does not change based on time.
- The probability of an event occurring is proportional to the length of the time period.



We calculate Poisson Distribution with the following formula:
$$
P(X=k)=\frac{\lambda^{k} e^{-\lambda}}{k !}
$$


*Example:*

> In the World Cup, an average of 2.5 goals are scored each game. What's the probability that *k* goals are scored in a game?
>
> In this λ=2.5. The above formula applies directly:
> $$
> \begin{array}{l}
> P(X=0)=\frac{2.5^{0} e^{-2.5}}{0 !} \approx 0.082 \\
> P(X=1)=\frac{2.5^{1} e^{-2.5}}{1 !} \approx 0.205 \\
> P(X=2)=\frac{2.5^{2} e^{-2.5}}{2 !} \approx 0.257 \\
> P(X=3)=\frac{2.5^{3} e^{-2.5}}{3 !} \approx 0.213 \\
> P(X=4)=\frac{2.5^{4} e^{-2.5}}{4 !} \approx 0.133
> \end{array}
> $$
> 
><img src="https://brilliant-staff-media.s3-us-west-2.amazonaws.com/tiffany-wang/4aJGBfZMzH.png" alt="The Poisson distribution with \(\lambda=2.5\)" style="zoom: 25%;" />
> 
>There is no upper limit on the value of *k* for this formula, though the probability rapidly approaches 0 as *k* increases. 



#### *Properties of the Poisson Distribution*

**Expected Value of Poisson Random Variable:**
$$
E[X]=λ
$$
**Variance of Poisson Random Variable:**
$$
Var[X]=λ
$$
**Mode of Poisson Random Variable:**

If λ is not an integer, the mode of a PD with parameter λ is ⌊*λ*⌋. Otherwise, both λ and *λ*−1 are modes.

**Median of Poisson Random Variable:**
$$
\lambda-\ln 2 \leq \rho \leq \lambda+\frac{1}{3}
$$
**Sum of Independent Poisson Random Variables:**
$$
P(X+Y=k)=\frac{\left(\lambda_{1}+\lambda_{2}\right)^{k} e^{-\left(\lambda_{1}+\lambda_{2}\right)}}{k !}
$$
**Poisson Limit Theorem:**
$$
\left(\begin{array}{l}
n \\
k
\end{array}\right) p^{k}(1-p)^{n-k} \simeq \frac{\lambda^{k} e^{-\lambda}}{k !}
$$




## **Continuous distributions**

A continuous distribution describes the probabilities of the possible values of a [continuous random variable](#continuous random variable). 

Only ranges of values can have a nonzero probability. The probability that a continuous random variable equals some value is always zero.



### Normal distribution

The most commonly used continuous distribution, also known as the Gaussian distribution, is used to model phenomena such as physical characteristics (height, weight, etc.) and test scores. Because of it's signature shape, it's also referred to as the bell curve.

![enBFdM8LyU-basic-normal-distribution](images\enBFdM8LyU-basic-normal-distribution.png)

- Symmetric and single-peaked, meaning its mean, median, and mode are all equal. 

- It additionally has "skinny tails", meaning it "tapers off" quickly.
- Nearly all of the X values fall within 3 standard deviations of the mean (99.7% values), 68% are within 1 standard deviation and 98% are within 2 standard deviations.



**Normal Probability Density Function:**
$$
F(x)=\frac{1}{\sigma \sqrt{2 \pi}} e^{-(x-\mu)^{2} / 2 \sigma^{2}}
$$


**All normal distributions can be converted to the standard distribution with the following formula:**
$$
Z=\frac{X-\mu}{\sigma}
$$
*Example:*

We want to see what's the probability that a randomly selected blue crab has a weight greater than 1kg. Based on research we see that the distribution of weights (kg) of adult blue crabs are normally distributed with a population mean (μ) of 0.8 kg and a standard deviation (σ) of 0.3 kg. 
$$
Z=\frac{1-0.8}{0.3}
$$

$$
Z=0.6667
$$



We can then look in our z table to determine the p(z>0.6667) is roughly 1-0.748 (pulled from the chart, somewhere between 0.7454 and 0.7486) = 0.252. Therefore, based on our normality assumption, we conclude that the likelihood that a randomly selected adult blue crab weighs more than one kilogram is roughly 25.2%.

<img src="images\crabnorm1.jpeg" alt="crabnorm1" style="zoom: 50%;" />





# `Statistics`

![statis](images\statis.png)

---

**Statistics** is all about data, and how we can manipulate it in order to answer our desired questions. Wait, don't mistake any kind of a question for a statistical one. 

The good old "How are you" wouldn't really fit into this scenario, so throw that idea out of the window. We can clearly answer these questions.

In comparison, the kind of questions I'm talking about are more along the lines of:

- Do women get paid less than men on average?

- Does it snow more in Berlin or Duisburg?

There are no immediate clear solutions for those questions, so we've now to use our statistical toolkit to come to a conclusion.



# `Variables`

## Qualitative & Quantitative

Variables can be classified in one of two ways: **qualitative** (categorical) or **quantitative** (numerical).

- Qualitative variables take on values that are names or labels. The color of a ball (e.g., red, green, blue) or the breed of a dog (e.g., collie, shepherd, terrier) would be examples of qualitative or categorical variables.

- Quantitative variables are numeric. They represent a measurable quantity. For example, when we speak of the population of a city, we are talking about the number of people in the city - a measurable attribute of the city. Therefore, population would be a quantitative variable. In algebra, these variables are represented with symbols (x,y,z)



## Discrete & Continuous

We can further classify quantitative (categorical) variables: **discrete** or **continuous**.

If a variable can take on any value between its minimum and maximum value, it's called a **continuous** variable.

- Suppose the fire department mandates that all fire fighters must weigh between 150 and 250 pounds. The weight of a fire fighter would be an example of a continuous variable; since a fire fighter's weight could take on any value between 150 and 250 pounds.

If the aforementioned state does not apply, then you have a **discrete** value.

- Suppose we flip a coin and count the number of heads. The number of heads could be any integer value between 0 and plus infinity. However, it could not be any number between 0 and plus infinity. We could not, for example, get 2.3 heads. Therefore, the number of heads must be a discrete variable.



## Univariate vs. Bivariate Data

We classify statistical data according to the number of variables being studied.

- **Univariate data**. When we conduct a study that looks at only one variable, we say that we are working with univariate data. 
  - For example, that we conducted a survey to estimate the average weight of high school students.
- **Bivariate data**. When we conduct a study that examines the relationship between two variables, we are working with bivariate data. 
  - For example, a study of the relationship between the height and weight of high school students.



# `Central Tendency`

Also called measures of central location, as it identifies the central position within a set of data. The 3 most common measures of central tendency are the mode, median, and mean.

- **Mean:** the most frequent value, the arithmetic average

- **Median:** the middle number in an ordered data set

- **Mode:** the sum of all values divided by the total number of values



## Mean

Equal to the sum of all the values in the data set divided by the number of values in the data set.



**Sample mean**

It's not feasible to gather data from the entire population, so we randomly sample.
$$
\bar{x}=\frac{\sum x}{n}
$$
It's easier to comprehend if you assign numbers to the formula:
$$
\bar{x}=\frac{33+29+21+23+20+25+32+23}{8}=25.75
$$


**Population mean**

To acknowledge that we are calculation the population mean and not the sample mean, we use the lower Greek letter "mu".
$$
\mu=\frac{\sum x}{n}
$$

## Median

The middle number in a  group of numbers. For example:
$$
12, 22, 42, 17, 6, 37
$$
Numbers are ordered from smallest to the largest, and we get **17** and **22** as the median numbers.
$$
6, 12, 17, 22,37, 42
$$
Since there's two of them, we have to average them.
$$
\frac{17+22}{2}=19.5
$$
If you've an odd number of values, simply skip this step as it's immediately clear what is the median value.



## Mode

The most frequent score in the dataset. In a histogram it represents the highest bar. Normally, the mode is used for categorical data where we wish to know which is the most common category, so you can also sometimes consider it as the most popular option.

<img src="images\mode-1.png" alt="mode-1" style="zoom:67%;" />



# `Spread & Measurement`

![dispersion example](images\dispersion example.png)

**Dispersion**, or spread, helps us understand the distribution of data; the extend to which a numerical data is likely to vary, so how spread out a set of data is.

*For example , let's take 2 data sets:*

> X₁ = { 97,98,99,100,101,102,103 }
>
> X₂ = { 70,80,90,100,110,120,130 }

The median for these two data sets is the same (100), but they're different! So, what now? Well, lucky for us, we can calculate the dispersion.



### Range

<img src="images\range1.png" alt="range1" style="zoom:50%;" />



One of the quickest and simplest ways is to calculate the range. What range tells us is how spread apart the data really is, so to calculate it, we take the highest number and deduct the lowest.
$$
R=x_{\max }-x_{\min }
$$
If we take the 2 examples from above, it would look something like this:
$$
R₁= 103 - 97 = 6
\\
R₂ = 130 - 70 = 60
$$
With that, we can now confidently say that R₁ is a lot more dispersed.



### Variance

With the range out of the way, we now have variance. Variance, or (S²) is the  average squared deviation of values from mean, it is the measure of variability. What variance tells us is the degree of spread in our data set. Which means, the more spread in our data, the larger the variance is going to be in relation to the mean.

*Why do we even calculate variance, you ask? Well, it matters for a few reasons:*

> Variance is important to consider before performing parametric tests. We don't want skewed results which can happen if we have uneven variances.
>
> We also use variance to asses group differences, for example, whether or not the population differs from one another.



#### Calculating Variance

If you're not completely sure about what I said above, that's alright. Very often variance can be calculated automatically anyway with software, but it's handy to know how to do it yourself, as it helps to further understand what's going on. So, get a dataset, and follow the steps with me.
$$
\begin{array}{cccccc}
{\text { Data set }} \\
\hline 46 & 69 & 32 & 60 & 52 & 41
\end{array}
$$

<center><br><b>Step 1: Find the mean!</b></center>

<center><i>If you're unsure how to do this, look at the steps discussed <a href="#expectation">above</a>.</i></center>

$$
\begin{array}{cccccc}
{\text { Mean (x̅) }} \\
\hline x̅ = (46 + 69 + 32 + 60 + 52 + 41) ÷ 6 = 50
\end{array}
$$



<center><b>Step 2: Find each score's deviation from the mean</b></center>

<center><i>Subtract the mean from each score's result to get the deviations from the mean</i></center>

<center><i>In our case, the mean is 50, so we're going to subtract that from each score</i></center>

$$
\begin{array}{cc}
\text { Score } & \text { Deviation from the mean } \\
\hline 46 & 46-50=-4 \\
69 & 69-50=19 \\
32 & 32-50=-18 \\
60 & 60-50=10 \\
52 & 52-50=2 \\
41 & 41-50=-9
\end{array}
$$



<center><b>Step 3: Square the deviations from the mean</b></center>

<center><i>Now with the deviations from the mean that we have, square them. Say goodbye to the negative numbers.</i></center>

$$
\begin{array}{l}
\text { Squared deviations from the mean } \\
\hline(-4)^{2}=4 \times 4=16 \\
19^{2}=19 \times 19=361 \\
(-18)^{2}=-18 \times-18=324 \\
10^{2}=10 \times 10=100 \\
2^{2}=2 \times 2=4 \\
(-9)^{2}=-9 \times-9=81
\end{array}
$$



<center><b>Step 4: Find out the sum of squares</b></center>

<center><i>Add up all of the previous results, to get a sum of squares.</i></center>

$$
\begin{array}{cccccc}
{\text { Sum of squares }} \\
\hline 16 + 361 + 324 + 100 + 4 + 81 = 886
\end{array}
$$

<center><b><br>Step 5: Divide the sum of squared by n-1 or N</b></center>

<center><i>Final step, this is what we're after. Divide either by n-1 (if you have a sample) or N (if you have a population).<br> Our example is a sample, so we use n-1.</i></center>

$$
\begin{array}{cccccc}
{\text { Variance }} \\
\hline  886 ÷ (6 – 1) = 886 ÷ 5 = 177.2
\end{array}
$$



#### Population vs Sample Variance

I mentioned above that you calculate differently depending on whether or not you have a population or a sample.



##### Population variance

If you're lucky and you have gathered data from every single member of the population that you're researching, you can get a precise value for a population variance.
$$
\sigma^{2}=\frac{\Sigma(X-\mu)^{2}}{N}
$$


##### Sample variance

This is the more common case, when you collect data only from the sample. In this case, we only get estimates about the population variance. To avoid possible biased estimates, we use n-1.
$$
s^{2}=\frac{\Sigma(X-\bar{x})^{2}}{n-1}
$$


### Standard Deviation

With this we calculate the average amount of variability in the dataset, so, on average how far away each value lies from the mean. We use it to measure normal distributions. A high standard deviation means the values are far away from the mean, and a low one means they're close. 

> *Wait, that's a bit confusing, why does it sound similar to variance?* ...

I felt the same, but just keep in mind that the standard deviation is derived from the variance itself; it's the square root of the variance. While both measure variability, their units also differ:

> **Standard deviation** is expressed in the same units as the original value (meters)
>
> **Variance** is expressed in much larger units (meters squared)



#### Calculating Standard Deviation

<center>To keep this shorter, repeat the steps from <a href="#calculating-variance">calculating variance</a> until you obtain the variance number (177.2).<br>After that it's pretty simple, just take the square root of the variance.</center>

$$
\begin{array}{cccccc}
{\text { Standard Deviation }} \\
\hline  √177.2 = 13.31
\end{array}
$$

With this, we can see that the standard deviation is 13.31, which means that the score deviates 13.31 points on average.



#### Population standard deviation

Same as before, if you have gathered data from the entire population, you can get the exact value for the population standard deviation.
$$
\sigma=\sqrt{\frac{\Sigma(X-\mu)^{2}}{N}}
$$

#### Sample standard deviation

If you only have data from a sample, you would use this formula to make estimates about the standard deviation, and same as before, use n-1 to avoid bias.
$$
s=\sqrt{\frac{\Sigma(X-\bar{x})^{2}}{n-1}}
$$

#### Empirical Rule![empirical rule](images\empirical rule.png)

If you have a normal distribution, the standard deviation and the mean together tell you where most of your values lie. The empirical rule, or the three-sigma rule or 68-98-99.7 rule, is a rule that tells us that pretty much all data observed will fall within those 3 standard deviations of the mean or average.

So, following this rule, it would mean that 68% of the data falls within one SD, 95% within two SDs, and 99.7% falls within all three standard deviations from the mean.



# `Univariate, bivariate and multivariate analysis`

## Univariate analysis

The simplest of all forms of statistical data analysis techniques. If we have data that has a single variable, does not deal with causes or effects relationships, then the univariate analysis is the perfect technique to use. The purpose is to describe the data we have, and to find patterns and tendencies, whether by looking into the mean, mode, median, dispersion, variance, range, standard deviation etc.

*For example – in a survey of a class room, the researcher may be looking to count the number of boys and girls. In this instance, the data would simply reflect the number, i.e. a single variable and its quantity as per the below table.* 

<img src="images\Capture2.png" alt="Capture2" style="zoom: 67%;" />

**How Univariate analysis is conducted:**

- Frequency Distribution Tables
- Histograms
- Frequency Polygons
- Pie Charts
- Bar Charts



## Bivariate analysis

This one is a bit more complex than the previous one, but comes in handy if our dataset contains two variables  that we want to compare. 

*For example – in a survey of a classroom, the researcher may be looking to analysis the ratio of students who scored above 85% corresponding to their genders. In this case, there are two variables – gender = X (independent variable) and result = Y (dependent variable). A Bivariate analysis is will measure the correlations between the two variables as shown the table below.*

<img src="images\Capture1-768x207.png" alt="Capture1-768x207" style="zoom:67%;" />

**How Bivariate analysis is conducted:**

- Correlation coefficients

  - *The strength of relationship between two variables is observed, where 1 is a perfect direct correlation, –1 is a perfect inverse correlation, and 0 is no correlation.*

- Regression analysis

  - Used for estimating the relationships between two different variables, and helps to understand how the value of the dependent variable changes when any one of the independent variables is changed. Used for advanced data modelling like prediction and forecasting.

  - There are a range of different regression techniques:

    - Linear regression
    - Simple regression
    - Polynomial regression
    - General linear model
    - Discrete choice
    - Binomial regression
    - Binary regression
    - Logistic regression

    

## Multivariate analysis

This one is used when there are more than two variables in the data set, and we want to understand the relationships of each variable with one another.

*For example - a doctor has collected data on cholesterol, blood pressure, and weight. She also collected data on the eating habits of the subjects (e.g., how many ounces of red meat, fish, dairy products, and chocolate consumed per week). She wants to investigate the relationship between the three measures of health and eating habits?*



**How Multivariate analysis is conducted:**

- Factor Analysis
- Cluster Analysis
- Variance Analysis
- Discriminant Analysis
- Multidimensional Scaling
- Principal Component Analysis
- Redundancy Analysis



# `Central Limit Theorem`

The Central Limit Theorem (CLT) states that the sampling distribution of the sample means approaches a normal distribution as the sample size gets larger — no matter what the shape of the population distribution. This fact holds especially true for sample sizes over 30.

So, the more samples we have, the more our graph of the sample mean will look like a normal distribution.

A simple example to visualize it would be rolling a die and visualizing it on a graph. The more we roll the die, the closer it gets to a bell curve.

<img src="images\500px-Dice_sum_central_limit_theorem.svg_-250x300.png" alt="500px-Dice_sum_central_limit_theorem.svg_-250x300"  />



# `Confidence Intervals`

A **confidence interval** gives an estimated range of values which are likely to include an unknown population parameter, the estimated range being calculated from a given set of sample data.

The common notation for the parameter in question is ![img](http://www.stat.yale.edu/Courses/1997-98/101/theta.gif). Often, this parameter is the population mean ![img](http://www.stat.yale.edu/Courses/1997-98/101/mu2.gif), which is estimated through the sample mean ![img](http://www.stat.yale.edu/Courses/1997-98/101/xbar.gif).

The ***level C*** of a confidence interval gives the probability that the interval produced by the method employed includes the true value of the parameter ![img](http://www.stat.yale.edu/Courses/1997-98/101/theta.gif).

> **Example**
>
> Suppose a student measuring the boiling temperature of a certain liquid observes the readings (in degrees Celsius) 102.5, 101.7, 103.1, 100.9, 100.5, and 102.2 on 6 different samples of the liquid. He calculates the sample mean to be 101.82. If he knows that the standard deviation for this procedure is 1.2 degrees, what is the confidence interval for the population mean at a 95% confidence level?
>
> In other words, the student wishes to estimate the true mean boiling temperature of the liquid using the results of his measurements. If the measurements follow a normal distribution, then the sample mean will have the distribution ***N(µ,<img src="http://www.stat.yale.edu/Courses/1997-98/101/smvar.gif" alt="img" style="zoom: 50%;" />)***. Since the sample size is 6, the standard deviation of the sample mean is equal to 1.2/sqrt(6) = 0.49.

![confdiag](images\confdiag.gif)



## Confidence Intervals for Unknown Mean and Known Standard Deviation

For a population with unknown mean **µ** and known standard deviation **σ**, a confidence interval for the population mean, based on a simple random sample (SRS) of size *n*, is <img src="http://www.stat.yale.edu/Courses/1997-98/101/xbar.gif" alt="img" style="zoom:67%;" />  ± z*<img src="http://www.stat.yale.edu/Courses/1997-98/101/smvar.gif" alt="img" style="zoom:67%;" />, where \*z\** is the upper (1-C)/2 critical value for the standard normal distribution.

- *This interval is only exact when the population distribution is normal. For large samples from other population distributions, the interval is approximately correct by the [Central Limit Theorem.](#central limit theorem)*

  

---

An increase in sample size will decrease the length of the confidence interval without reducing the level of confidence. This is because the standard deviation decreases as *n* increases. 

The **margin of error m** of a confidence interval is defined to be the value added or subtracted from the sample mean which determines the length of the interval:
$$
m=z^{*} \frac{\sigma}{\sqrt{n}}
$$


## Confidence Intervals for Unknown Mean and Unknown Standard Deviation

In most practical research, the standard deviation for the population of interest will now be known. In this case, the standard deviation  **σ** is replaced by the estimated standard deviation *s*, also known as the ***standard error***. Since the standard error is an estimate for the true value of the standard deviation, the distribution of the sample mean <img src="http://www.stat.yale.edu/Courses/1997-98/101/xbar.gif" alt="img" style="zoom:67%;" /> is no longer normal with mean  **µ** and standard deviation <img src="http://www.stat.yale.edu/Courses/1997-98/101/smvar.gif" alt="img" style="zoom:67%;" />. 

Instead, the sample mean follows the ***t distribution*** with mean **µ** and standard deviation <img src="http://www.stat.yale.edu/Courses/1997-98/101/tvar.gif" alt="img" style="zoom:67%;" />. 



*For a population with unknown mean  µ and unknown standard deviation, a confidence interval for the population mean, based on a simple random sample (SRS) of size n, is <img src="http://www.stat.yale.edu/Courses/1997-98/101/xbar.gif" alt="img" style="zoom:67%;" /> + t<img src="http://www.stat.yale.edu/Courses/1997-98/101/tvar.gif" alt="img" style="zoom:67%;" />, where t is the upper (1-C\)/2 critical value for the t distribution with n-1 degrees of freedom, t(n-1)\.*



# `Distributions`

## Sampling Distribution

A sampling distribution is a probability distribution of a statistic obtained from a larger number of samples drawn from a specific population that shows us every possible results a statistic can take on, in every possible sample from a population, and how that can happen.

The common distributions are:

- Mean
- Mean absolute value of the deviation from the mean
- Range
- Standard deviation of the sample
- Unbiased estimate of variance
- Variance of the sample



### Standard Deviation of Sampling Distribution of the Proportion

The “standard deviation of the sampling distribution of the proportion” in simpler words means that we are calculating the standard deviation. This is repeated for all possible samples from the population.

**Example:**

> A survey is held to find out the average students' grades and the calculated standard deviation is 1. It's highly unlikely that a same result will pop up if the survey is repeated, so we want to repeat it the maximum amount of times possible. From that we will get a range of samples - one from each same. Th probability distribution of all of the standard deviations is called a sampling distribution of the standard deviation.



#### Sampling Distribution of a Proportion

When you repeat your survey for all possible samples of the population. 

**Example:** 

> Instead of polling 100 people once to ask if they are democrat, you’ll poll them multiple times to get a better estimate of your statistic.

#### Standard Deviation of Sampling Distribution of the Proportion

If our random sample of n observations is taken from a binomial population with a parameter p, the sampling distribution will have a standard deviation of:
$$
σp = √[\frac{pq}{n}] \text{ where } q=1-p.
$$
When the sample is large, the sampling distribution of a proportion will have an approximate normal distribution.



### Mean of the sampling distribution of the mean

Simply put, the mean of the sampling distribution of the mean is the same as the population mean. 

**Example:**

> If your population mean (μ) is 99, then the mean of the sampling distribution of the mean, μm, is also 99 (as long as you have a sufficiently large sample size). If you want to understand *why*, watch the video or read on below.



#### The mean of the sampling distribution of the mean formula

The mean of the sampling distribution of the mean formula is μM = μ, where μM is the mean of the sampling distribution of the mean.



### Mean of Sampling Distribution of the Proportion

The **sampling distribution of a proportion** is when you repeat your survey or poll for all possible samples of the population. For example: instead of polling asking 1000 cat owners what cat food their pet prefers, you could repeat your poll multiple times.



**Example:** 

> 100 people are asked if they are democrat. If 50 people respond “yes” then the sample proportion p = 50/100. A sample proportion is where a random sample of objects *n* is taken from a population P; if x objects have a certain characteristic then the sample proportion “p” is: p = x/n.

The **sampling distribution of a proportion** is when you repeat your survey or poll for all possible samples of the population. Instead of polling asking 1000 cat owners what cat food their pet prefers, you could repeat your poll multiple times.



## **Cumulative Distribution Function **(CDF)

The cumulative distribution function, or CDF for short, is the probability that the variable takes a value less than or equal to x. The advantage of the CDF is that it can be defined for any kind of random variable (discrete, continuous, and mixed).

The cumulative distribution function (CDF) of random variable X is defined as:
$$
F_{X}(x)=P(X \leq x), \text { for all } x \in \mathbb{R}
$$
The cumulative distribution function (CDF) is found by integrating the PDF between the minimum and maximum value of X and t. 

CDF for continuous distribution:
$$
F(x)=\int_{-\infty}^{x} f(\mu) d \mu
$$
CDF for a discrete distribution:
$$
F(x)=\sum_{i=0}^{x} f(i)
$$


### Probability Mass Function (PMF)

Function that gives the probability that a discrete random variable is exactly equal to some value. 

Probability mass function is the probability distribution of a discrete random variable, and provides the possible values and their associated probabilities. It is the function ![{\displaystyle p:\mathbb {\mathbb {R} } }](https://wikimedia.org/api/rest_v1/media/math/render/svg/7c4ff98f9f72b0fdfc42ea5b9494359011735b5c) {\displaystyle \rightarrow [0,1]}![{\displaystyle \rightarrow [0,1]}](https://wikimedia.org/api/rest_v1/media/math/render/svg/6bfdb731e92ac585a0336ba3a48696cb21ea36fc) defined by
$$
p_{X}\left(x_{i}\right)=P\left(X=x_{i}\right)
$$



### Probability Density Function (PDF)

Also known as PDF, it's used to specify the probability of a random variable falling within a particular range of values, as opposed to taking on any one value. The probability density function is nonnegative everywhere, and its integral over the entire space is equal to 1.

A PDF must be integrated over an interval to yield a probability.

Since for continuous distributions the probability at a single point is zero, this is often expressed in terms of an integral between two points:
$$
\int_{a}^{b} f(x) d x=\operatorname{Pr}[a \leq X \leq b]
$$
For discrete distributions:
$$
f(x)=\operatorname{Pr}[X=x]
$$



# `Hypothesis testing` 

A hypothesis is an educated guess about something in the world. It has to be testable, be it by experiment or by observation. So, hypothesis testing is a way to test if the results of our experiment have any real meaningful results. We're testing if the results are valid, since if it only happened by chance, the experiment is not repeatable and has little use.



## P Values

A p value is a number that you get by running a hypothesis test on your data. A P value of 0.05 (5%) or less is usually enough to claim that your results are repeatable. It's also the evidence against a null hypothesis. The smaller the p-value, the stronger the evidence that you should reject the null hypothesis.

![p-value](images\p-value.png)



## Z score

<img src="images\zimg.jpg" alt="zimg" style="zoom:67%;" />



A z-score or a standard score gives us an idea how far a data from is from the mean, and they're a way to compare results to a normal population. 

**One sample z score formula:**
$$
z = \frac{(x – μ)}{σ}
$$
**Example:**

There's a test with a score of 190. That test has a mean μ of 150 and a standard deviation σ of 25. Assuming a normal distribution, the z score would be:
$$
z = \frac{x-μ}{σ} \\
z = \frac{190-150}{25} \\
z=1.6
$$


### **Z-score Standard Error of the Mean**

If we're dealing with multiple samples and we want to describe the standard deviation of those sample means (standard error), we use this formula:
$$
z=\frac{x – μ}{\frac{σ}{√n}}
$$
**Example:** 

The mean height of a woman is 65" with a standard deviation of 3.5". What is the probability of us finding a random sample of 50 women with a mean height of 70", assuming the heights are normally distributed?
$$
z=\frac{x – μ}{\frac{σ}{n}}\\
=\frac{70-65}{\frac{3.5}{√50}}
\\=10,10
$$


## Null Hypothesis

The null hypothesis assumes that there's no real relationship between two variables and that controlling one variable has no effect on another. Testing the null hypothesis tells us whether our results are because of chance, or due to the effect of manipulating variable.



### Stating the Null Hypothesis

<img src="images\null-hypothesis-examples-609097_FINAL-100262e70b70426fb0633304eb2f49f4.webp" alt="null-hypothesis-examples-609097_FINAL-100262e70b70426fb0633304eb2f49f4" style="zoom:67%;" />

In order to write a null hypothesis, we take a question, and rephrase it in a way that we assume that there's no relationship between the variables. 



### Rejecting the null hypothesis

You don't really need to believe that the null hypothesis is true to test it, you're actually more likely to suspect that there is in fact a relationship between a set of variables. One of the ways to prove it is to reject the null hypothesis. 

**Example:**

Up until 2006, there were 9 planets in our solar system, one of which was Pluto. The null hypothesis of "Pluto is a planet" was replaced by "not a planet". 



## The Alternate Hypothesis

As the name says, it's an alternate hypothesis to the null. In many cases, it's a **direct opposite of the null hypothesis**. For example, if you're gambling, and hoping to win up to 1000 euros, an alternate hypothesis would be that you will win more than 1000 euros. What we're looking for in the alternate hypothesis is enough of a change to be able to reject the null hypothesis. 

This is usually the hypothesis we will be testing, and is the statement that can ultimately lead us to reject the null hypothesis and replace it with the alternate one.

> **Example:** 
>
> A classroom of students happened to be performing rather poorly this year on all of their tests. The low test scores are thought to be due to teacher's poor performance. However, you have a theory that the students are performing poorly because they are forced into online schooling. 
>
> **Null hypothesis:** Low test scores are due to teacher's poor performance
>
> **Alternate hypothesis:** Low test scores are due to forced online schooling



## T-Test

It tells us how significant the difference between the groups are, so how likely it is that the difference have happened by chance. 

**Example:** You get a cold and you try a home remedy; the cold lasts a few days. A little later down the road you get a cold again, and you buy over-the-counter medication from the pharmacy; the cold lasts over a week. You ask your friends and they all tell you that their colds lasted much shorted when taking home remedies. With a t-test we can know the probability of those results happening by chance. 



### T-Score

A ratio between the difference of the two groups and the difference within the groups. The larger the score, the more difference there is between the groups, and the smaller it is, the more similar they are. 

The [t score](https://www.statisticshowto.com/probability-and-statistics/t-distribution/t-score-formula/) is a [ratio ](https://www.statisticshowto.com/ratios-and-rates/)between the **difference between two groups and the difference within the groups**. The larger the t score, the more difference there is between groups. 



### Paired T-Test

Also called correlated pairs t-test, dependent samples t-test, is when you run a t-test on dependent samples. It's used to compare related observations. ,so it's a test run on the same person, or a thing.

- Two vision tests
- Two MRI tests in different hospitals
- Two blood pressure tests with different equipment



### One sample T-Test

In this tests, we compare the mean of our sample data to a known value. For example, you're curious how your sample mean compares to the population mean. In this case, when we don't know the population standard deviation, or we have a small sample size, we run a one sample t-test.

In order for the test to be valid, the data has to meet the following criteria:

- Data is independent
- Data is collected randomly
- The data is approximately normally distributed



**Example:**

> You want to improve sales. We know that past sales show us the average of 100 Euros per transaction. You train 25 random staff, and the average sales how 130 Euros, with a SD of 15 Euros. Did the training work? Well, let's test the hypothesis at a 5% alpha level.
>
> **Step 1:** Write the null hypothesis. Meaning no difference in sales: H0: μ = $100.
>
> **Step 2:** Write the alternate hypothesis. This is the one we will test. Meaning there is a difference in sales: H1: μ > $100.
>
> **Step 3:** Insert the items from above into the t score formula:
> $$
> t=\frac{\overline{\mathrm{x}}-\mu}{\frac{S}{\sqrt{n}}}
> $$
> t = (130 – 100) / ((15 / √(25))
> t = (30 / 3) = 10
>
> Now we have the calculated t-value.
>
> **Step 4:** Find the t-table value. You need two values to find this:
>
> 1. The alpha level: given as 5% in the question.
> 2. The degrees of freedom, which is the number of items in the sample (n) minus 1: 25 – 1 = 24.
>
> From the table we get 1.711, this is our one-tailed critical t-value. What this means is that we expect most values to fall under this range. If the calculated t-value falls within it, the null hypothesis is true. The calculated value from step 3 does not fall into the range of 1.711, so we can reject the null hypothesis. The value of 10 falls into the rejection region. 
>
> With this we now know that the training was a success and we really did sell more.



### Independent samples T-Test

The most common form of the T-test, which compares the means of two sets of data. 

If you would run a t-test to see if the average test scores of men and women are different; the test answers the question, “Could these differences have occurred by random chance?” 

You should use this test when:

- You do not know the population mean or standard deviation.
- You have two independent, separate samples.

#### Assumptions for the Independent Samples T Test

- **Assumption of Independence:** you need two independent, categorical groups that represent your independent variable. In our example, “men” or “women” would be your independent variable.
- **Assumption of normality**: The dependent variable should be approximately normally distributed, and measured on a continuous scale. In our example, the “test score” would be the dependent variable.
- **Assumption of Homogeneity of Variance:** The variances of the dependent variable should be equal.



## ANOVA

An ANOVA, or Analysis of variance, is a test to find out if the results are significant. We're testing groups to see if there's a difference between them.

For example:

- All students take the same final exam; we want to see if one school outperforms the other
- A factory has two different ways to make lightbulbs, and we want to know if one process is better than the other
- A patient is trying a few different therapies, and wants to know if one is better than the other



### One-Way & Two-Way

There are two main types: one and two way. Two way can be done with or without replication.

- **One-way ANOVA:** Used when you want to see if there's a difference between two groups
- **Two way ANOVA without replication:** If you have one group and you're double testing them. For example, before and after administering medication.
- **Two way ANOVA with replication:** Two groups, and the members of those groups are doing more than one thing. For example, two groups of patients who are in different hospitals trying two different medications.



# `Quantitative Data`

Quantitative data is, quite simply, information that can be counted or measured, and given a numerical value. It can be counted or measured, and given a numerical value—such as length in centimeters or revenue in dollars. If you have questions popping up that sounds something like “How many?”, “How often?” or “How much?”, quantitative data can help you find the answers you're looking for.

**Examples of quantitative data:**

- Weight in kilograms
- Age in months or years
- Length in centimeters



**How it's collected:**

- Analytics tools, such as Google Analytics
- Probability sampling
- Questionnaires and surveys
- Open-source datasets on the web



## Types of quantitative data

**Discrete data**

- Can only take on certain numerical values that are fixed and cannot be broken down
- For example, if a person has two children, the number of children is fixed—it’s not possible to have 1.5 children

**Continuous data**

- Can be infinitely broken down into smaller parts, and this type of quantitative data can be placed on a measurement scale

- For example, the length of a piece of wood in meters, or the temperature in degrees Celsius

- Can take any value; it’s not limited to fixed values, and can also fluctuate over time—the room temperature will vary throughout the day, for example

- Usually represented using a line graph

  

## Quantitative Data Analysis

There's a whole lot of these, but these are the most common and useful methods when it comes to quantitative data analysis:

- **Regression analysis**
  - Used to estimate the relationship between a set of variables to see if there's some kind of a correlation between them.
  - Useful for making predictions and forecasting future trends
- **Monte Carlo simulation** 
  - Considers a range of possible outcomes and then calculates how likely it is that each of those outcomes is going to occur based on our dataset.
  - Used for advanced risk analysis to accurately predict what's going to happen
- **Cohort analysis** 
  - A cohort is a group that shares a common thing over a period of time; for example, everyone who started university in 2020
  - Divides your dataset into cohorts and analyzes how they behave over time
  - Useful for identifying customer behavior and patterns and tailoring products and services to them
- **Cluster analysis** 
  - Used to identify structures within our dataset
  - The aim is to sort different data points within a cluster that are similar to each other, but dissimilar to data points in other clusters
  - Used to see how data is distributed in a given dataset, or as a pre-processing step for other algorithms
- **Time series analysis** 
  - Used to identify trends and cycles over time
  - Measures the same variable at different points in time, such as weekly tickets sold, monthly subscriptions, etc. 
  - Used to forecast how the variable of interest may fluctuate in the future, handy when making business decisions



## Bayes Factor

The Bayes factor is the ratio of the likelihood of one hypothesis to the likelihood of another one. It gives us the possibility to evaluate data in comparison to a null hypothesis by telling us the weight of the hypothesis evidence. 

The way we define it is:
$$
B_{10}=\frac{\text { likelihood of data given } H_{1}}{\text { likelihood of data given } H_{0}}=\frac{P\left(D \mid H_{1}\right)}{P\left(D \mid H_{0}\right)}
$$
The factor can be any number as long as it is positive. The following table gives us a good overview of the most common interpretations of the factor:
$$
\begin{array}{|c|c|}
\hline \text { If } B_{10} \text { is... } & \text { Then you have... } \\
\hline>100 & \text { Extreme evidence for } H_{1} \\
30-100 & \text { Very strong evidence for } H_{1} \\
10-30 & \text { Strong evidence for } H_{1} \\
3-10 & \text { Moderate evidence for } H_{1} \\
1-3 & \text { Anecdotal evidence for } H_{1} \\
1 & \text { No evidence } \\
1 / 3-1 & \text { Anecdotal evidence for } H_{1} \\
1 / 3-1 / 10 & \text { Moderate evidence for } H_{1} \\
1 / 10-1 / 30 & \text { Strong evidence for } H_{1} \\
1 / 30-1 / 100 & \text { Very strong evidence for } H_{1} \\
<1 / 100 & \text { Extreme evidence for } H_{1} \\
\hline
\end{array}
$$


## Credibility Interval

<img src="images\credible-interval.jpg" alt="credible-interval" style="zoom: 50%;" />

The Bayesian equivalent of the confidence interval, but this one is dependent on the prior distribution.



**Choosing a credible interval**

- Choosing the highest posterior density interval (HPDI)
- Choosing the equal-tailed interval
- Assuming the mean exists, choosing the interval for which the mean is the central point

**Example:**

Let's say we're running an experiment on the distribution of newborns' weights. If the subjective probability that the birthweight β is between 2.8kg and and 3.5kg is 90%, we can say that this interval β is in a 90% credible interval.



# `Frequentist & Bayesian Statistics` 

<img src="images\frequentists_vs_bayesians.webp" alt="frequentists_vs_bayesians" style="zoom: 67%;" />

## The Frequentist Approach

This approach makes predictions on the underlying truths of the experiment by using data only from that experiment. Frequentists use narrowly defined sets of formulas, tables, and solution steps. 

Basically, **a Frequentist method makes predictions on the underlying truths of the experiment using only data from the current experiment.**



## The Bayesian Approach

This one is a polar opposite to frequentist statistics. These guys also like spicing things up by adding a few unknowns into the mix. 

The most important distinction here is that there is some prior probability such as:

- Has this already happened?
- Based on my current knowledge, is it likely to happen?



Usually, the approach would go something along these lines:

1. Gather the prior distribution that has your beliefs about a parameter, this can be both informative or informative
2. Gather the data
3. To get the posterior distribution update the prior one with the Bayes' theorem
4. Analyze the posterior distribution and summarize it (mean, median, sd, quantiles…)



## Reasonings Explained

The above explanations might be kind of unclear, so I will explain it with a day to day example.

I'm a rather forgetful person, so I lose my phone quite regularly. Luckily I can use a phone locator device to help me find it. Once I activate it, the phone will start to beep.

**Problem:** Which areas of the house should I search?



**Frequentist Reasoning**

I can hear the phone beeping! I can identify where the sound is coming from, therefore upon hearing it, I can conclude where the sound originated from and where I must search to locate it.

**Bayesian Reasoning**

I can also hear the phone beeping! But, apart from being able to tell where the sound comes from, I also know the locations where I have misplaced my phone in the past. Now I can combine those two inferences in order to identify where I have to look for the phone.



# `Bayesian Inference` 

<img src="images\iStock-1205583077-2-1.jpg" alt="iStock-1205583077-2-1" style="zoom: 50%;" />

Let's say we were still at the start of this global pandemic, and you're worried you might've gotten infected. You've read online that the chance to catch the disease is P(disease)=0.001. Just to be sure, you go to a doctor to get tested, and the doctor tells you that the test is 95% accurate. 

You're now really curious how likely it is that you have the disease. We can calculate this with Bayes' Theorem:
$$
P\left(Y_{j} \mid X\right)=\frac{P\left(X \mid Y_{j}\right) P\left(Y_{j}\right)}{\sum_{i=1}^{k} P\left(X \mid Y_{j}\right) P\left(Y_{j}\right)}
$$


If we fill out the formula with the example we're dealing with it we get this:
$$
\begin{aligned}
P(\text { disease } \mid+) &=\frac{P(+\mid \text { disease }) P(\text { disease })}{P(+\mid \text { disease }) P(\text { disease })+P(+\mid \text { healthy }) P(\text { healty })} \\
&=\frac{0.95 * 0.001}{0.95 * 0.001+0.05 * 0.999} \\
& \approx 0.019
\end{aligned}
$$


Roughly 2%, but we can safely infer that the probability that you have the disease is much lower, based on the fact, that most of the population (at the time) was still pretty healthy. 



## Bayes Procedure

Right, so if you want to replicate this test again, but for a different parameter, how would one go about it? You would follow this general guideline:

1. Start by expressing your initial beliefs about said parameter in the form of a prior distribution

2. Go and collect data with observations, surveys or experiments.

3. Update your beliefs using Bayes' Theorem
   $$
   P(A \mid B)=\frac{P(B \mid A) P(A)}{P(B)}
   $$

4. Repeat this entire process if you receive more data 



## Prior 

Also known as prior probability distribution is a distribution about our knowledge of a parameter before we receive any additional data about it. In the example above with the pandemic disease, we used the probability that it was unlikely that a lot of people were already infected.

There's three different subtypes of priors:

- **informative priors**
  - Specific and definite information about a variable
- **weakly informative priors**
  - Only partial information about a variable
  - used to keep inferences in a reasonable range
- **uninformative priors**
  - vague or general information about a variable



## Likelihood Function

If you get two heads in a row, your likelihood function for the probability of a coin landing heads-up will look something like this:

<img src="images\hh.jpg" alt="hh" style="zoom: 80%;" />

If you toss once more and get tails (Heads-Heads-Tails), you get this:

<img src="images\hht.jpg" alt="hht" style="zoom: 80%;" />

A likelihood function takes the data set as a given, and represents the likeliness of different parameters for your distribution.

The likelihood is the probability of a parameter θ given data X is P (X|θ):
$$
L(θ |X) = P(X |θ)
$$

- constant of proportionality,it's an equivalence class of functions.
- In the likelihood function, sample point x is a constant and θ to varies over the whole range of possible parameter values

- Two different parameter points are compared; for example, if we find that L(θ1 | x) > L(θ2 | x), we know that our observed point x is more likely to have been observed under parameter conditions θ = θ1 rather than θ = θ2

- Unlike PDF, likelihoods aren’t normalized, so the area under their curves doesn't have to add up to 1



## Posterior Belief

The posterior belief is the revised or updated probability of an event occurring after taking into consideration new information that we have gathered. It's calculated by updating the prior probability using the Bayes' theorem. Basically, the probability of event A occurring given that event B has already occurred. 



# Learning resources

---

**Introduction to Probability, Harvard:** https://learning.edx.org/course/course-v1:HarvardX+STAT110x+2T2020/home

**Probability Course, probabilitycourse:** https://www.probabilitycourse.com/chapter1/1_5_0_chapter1_problems.php

**Probability Unit, Khan Academy:** https://www.khanacademy.org/math/statistics-probability/probability-library

**Seeing Theory, Brown University:** https://seeing-theory.brown.edu/

**Probability Theory, Britannica:** https://www.britannica.com/science/probability-theory

**Types of Events in Probability, Byjus:** https://byjus.com/maths/types-of-events-in-probability/ (VPN outside of EU needed to access)

**Modeling Data Distributions, Khan Academy:** https://www.khanacademy.org/math/statistics-probability/modeling-distributions-of-data

**Normal Distribution, Scribbr:** https://www.scribbr.com/statistics/normal-distribution/

**Random Variable, Khan Academy:** https://www.khanacademy.org/math/statistics-probability/random-variables-stats-library

**Probability Distribution, Investopedia:** https://www.investopedia.com/terms/p/probabilitydistribution.asp#:~:text=A%20probability%20distribution%20is%20a,take%20within%20a%20given%20range

**Probability and the Law of Large Numbers, Encyclopedia:** https://www.encyclopedia.com/education/news-wires-white-papers-and-books/probability-and-law-large-numbers#:~:text=Theoretical%20and%20experimental%20probabilities%20are,theoretical%20probability%20of%20that%20outcome

**Conditional Probability, Yale University:** http://www.stat.yale.edu/Courses/1997-98/101/condprob.htm

**Cardinality, Brilliant:** https://brilliant.org/wiki/cardinality/#:~:text=The%20cardinality%20of%20a%20set,elements%20that%20are%20in%20it.

**Intro to Descriptive Statistics, Udacity:** https://www.udacity.com/course/intro-to-descriptive-statistics--ud827

**Descriptive Statistics, Khan Academy**: https://www.khanacademy.org/math/engageny-alg-1/alg1-2

**Expected Value in Statistics, Statistics How To:** https://www.statisticshowto.com/probability-and-statistics/expected-value/

**Basic Probability Rules, University of Florida:** https://bolt.mph.ufl.edu/6050-6052/unit-3/module-6/

**Understanding Bernoulli and Binomial Distributions, Towards Science:** https://towardsdatascience.com/understanding-bernoulli-and-binomial-distributions-a1eef4e0da8f

**Central Tendency, Scribbr:** https://www.scribbr.com/statistics/central-tendency/

**Measures of Central Tendency, Laerd:** https://statistics.laerd.com/statistical-guides/measures-central-tendency-mean-mode-median.php

**Confidence Intervals, Yale University:** http://www.stat.yale.edu/Courses/1997-98/101/confint.htm

**Sampling Distribution, Khan Academy:** https://www.khanacademy.org/math/statistics-probability/sampling-distributions-library/what-is-a-sampling-distribution/v/introduction-to-sampling-distributions?modal=1

**Sampling Distribution, Statistics How To:** https://www.statisticshowto.com/sampling-distribution/#:~:text=%3D%20x%2Fn.-,The%20sampling%20distribution%20of%20a%20proportion%20is%20when%20you%20repeat,repeat%20your%20poll%20multiple%20times.

**Bayesian vs Frequentist, CXL:** https://cxl.com/blog/bayesian-frequentist-ab-testing/#:~:text=In%20summary%2C%20the%20difference%20is,without%20being%20assigned%20a%20probability.

**Likelihood Function, Humboldt University:** http://sfb649.wiwi.hu-berlin.de/fedc_homepage/xplore/tutorials/mvahtmlnode45.html