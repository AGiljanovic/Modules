<h1>
    <center>Probability & Statistics </center>
</h1>

<center>Antea Giljanovic, Spring Semester, 2021</center>

## Table of Content

1. ### [Introduction](#introduction) 

2. ### [Probability](#probability)

   1. #### [Basic Probability](#Basics-of-Probability)

      - ##### [Terms](#terms)

      - ##### [Sample Space](#sample-space)

      - ##### [Events](#events)

      - ##### [Expectation](#expectation)

   2. #### Set theory

      1. [fill this in]
      
   3. #### [Types of Probability](#types-of-probability)

      1. ##### [Theoretical probability](#theoretical-probability)
      2. ##### [Experimental probability](#Experimental-probability)
      3. ##### [Conditional probability](#Conditional-probability)
      4. ##### [Subjective probability](#Subjective-probability)

   4. #### Combinatorics

      1. Permutations 
      2. Combinations
      3. Binomial coefficients
      4. Binomial theorem

   5. #### [Probability Distribution](#probability-distribution)

      1. Random Variable
      2. Discrete and Continuous
      3. Central Limit Theorem

3. ### Statistics

   1. #### Introduction

   2. Descriptive Statistics

      1. Types of variables
      2. Central tendency and spread measurements
      3. Univariate, bivariate and multivariate analysis

   3. Mean, variance, quantiles

   4. Inferential Statistics

      1. Population and sample
      2. Sampling distributions, central limit theorem
      3. Hypothesis testing with one and two group means; categorical data; more than two group means (ANOVA) one and two way
      4. Quantitative data; correlation and regression

   5. #### Frequent Inference

      1. Point Estimation
      2. Confidence Interval
      3. The Bootstrap

   6. #### [Spread & Measurement](#Spread-&-Measurement)

      1. ##### [Range](#range)

      2. ##### [Variance](#Variance)

      3. ##### [Standard Deviation](#standard-deviation)

   7. #### [Empirical Rule](#empirical-rule)

   8. #### Regression Analysis

      1. ##### Ordinary Least Squares

      2. ##### Correlation and Causality

      3. ##### Analysis of Variance

   9. #### Bayesian Inference

      1. ##### Bayes' Theorem

      2. Frequentist vs Bayesian statistics

      3. ##### Likelihood Function

      4. ##### Prior to Posterior

      5. Test for significance; Bayes factor, credibility interval

4. ### [Learning Resources](#learning-resources)



# Introduction

Before we get into it, I would like to explain that this portfolio is to be a learning guide for anybody who has an interest in probability and statistics, whether it be a newcomer or not. I believe concepts should be explained simply enough to spark interest even in those who never imagined reading through a math book.

So take your time, and read through and learn together with me, as this portfolio is also my learning journey.



With that said, how would I actually explain probability and statistics, you ask? Well, all probability questions are out to get the an answer from the same type of a question:

> Out of X amount of possible outcomes, how often will Y happen?

To simplify it even further, we can use simple problems. For example, take three plastic cups and a coin. ![cup and coin](C:\Users\Chloe\Desktop\Main\Statistics images\cup and coin.png)So, now we want to know what is the probability of the coin being under cup A. Let's look at all of the possibilities:

> 1. The coin is under cup A
> 2.  The coin is under cup B
> 3. The coin is under cup C

Next thing you would do is count how many of those cases the coin is under cup A.![cup and coin1](C:\Users\Chloe\Desktop\Main\Statistics images\cup and coin1.png)

Turns out, it's just one. This means that the odds are 1/3. You can also do this in reverse, for example, what are the odds that the coin is not under the cup? It's not under B or C, so it's 2/3.

That's what statistics is, but as the problems get more complicated (a thousand cups and a hundred coins; or even trying to figure out the odds that a coin will be under the same cup 10 times in a row), the math of how you calculate the estimate of the total outcomes gets steadily more and more complex.



<center><h1>Probability</h1></center>

![cards](C:\Users\Chloe\Desktop\Main\Statistics images\cards.png)



# Basics of Probability

> **Probability theory**, a branch of mathematics concerned with the analysis of random phenomena. The outcome of a random event cannot be determined before it occurs, but it may be any one of several possible outcomes. The actual outcome is considered to be determined by chance.

Probability theory is a mathematical framework we use to analyze these random events in a logically sound manner.

Before I dive deeper into the topic, I want you to familiarize yourself with the basic of probability, to avoid any confusion that may come up later on.

## Terms

##### Population

The entire group that you gather information from

##### Sample

Subset of the population you're gathering the data from, because analyzing  the entire population is not possible as it is too large. However, its characteristics are still representative of the population.

##### Mean

Otherwise known as arithmetic mean or average. Click [here](#Expected-Value) to read more about it.

##### Median

The value separating the lower from the higher half of the population. We get this value by arranging all the values from the lowest to the highest and taking the middle one.

##### Variance

Measures dispersion around the mean. Click [here](#variance) to read more about it.

##### Standard Deviation

Square root of the variance, also measures the dispersion around the mean, but in the same units as the values. Click [here](#standard-deviation) to read more about it.

##### Standard Error

##### 



## Sample Space

The entire possible set out outcomes is called a sample space, and it's most often marked with the Greek letter Omega(**Ω**).

Put simply, if we have a die, the sample space, or all of the possible rolls we can get, would be be between the numbers 1 and 6, written so:

<center><b>Ω = {1,2,3,4,5,6}</b></center>

## Events

While doing an experiment, we're often doing it with the intent of looking for an outcome — an event. Depending on the outcome, there's various types of events, too.![bubble](C:\Users\Chloe\Desktop\Main\Statistics images\bubble.png)

### Impossible and Sure Events

The probability of an event happening is a number indicating how likely that event will occur. This number is always either 1 **(sure event)**, meaning certainty that the event will occur, and 0 indicating that it's impossible **(impossible event)**. 

*For example:*

> **Impossible event**
>
> ​		Obtaining 7 on a fair number cube throw
>
> **Sure event**
>
> ​		Obtaining a number less or equal to a 6 on a fair number cube throw



### Simple Events

An event with a single outcome. 

If we are rolling a die, and only looking for 1, we would write it so:

<center><b>E = {1}</b></center>



### Compound Events

Contrary to the simple event, if an event consists of more than one point of sample space, then we call this a **compound event**. 

For example, if we're only looking for uneven numbers while throwing a die.

<center><b>E = {1,3,5}</b></center>



### Independent Events and Dependent Events

If the occurrence of one event is not affected by another, then this is called an **independent event** *(left image)*. The opposite would be called a **dependent event** *(right image).*

![bubble ab](C:\Users\Chloe\Desktop\Main\Statistics images\bubble ab.png)

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



### Mutually Exclusive Events

If the the occurrence of one event excludes another, it's called an **exclusive event**, or in other words, those two events have nothing in common.

*For example:*

> if the sample space of a die is S = {1 , 2 , 3 , 4 , 5 , 6}, and E1 and E2 are such events that E1 is numbers less than 3, and E2 is only numbers greater than 4.
>
> This would make E1 and E2 **mutually exclusive.**



### Exhaustive Events

If the event consumes the entire sample space, we call this an **exhaustive event.**

*For example:*

> A coin is tossed, and we have 2 events.
>
> Event H = if head is tossed
>
> Event T = if tails appears

Because either one of the events will occur during the conduct of the experiment, both events together are an exhaustive event.



### Complementary Events

For every single E event, there's a corresponding Ē, which is the set out outcomes that are not included in the event space, but are a part of the sample space. They are called **complementary events.**

In the example of odd numbers, the complementary events are the odd numbers.

<center><b>E = {1,3,5}</b></center>

The outcome of an event combined with the complementary events make up the entire sample space. 

E and Ē are disjoint, and it **is impossible for an event and its complement to occur at the same time.**

The rule for complementary events is the following:



<center><b>P(Ē) = 1 - P(E)<br> P(E) + P(Ē) = 1 <br> P(E) = 1 - P(Ē)</b></center>



## **Expected Value**

The expected value of a random variable X, is a number that represents the weighted average of that random variable's distribution. It is defined as the probability-weighted sum of all possible values in the random variable's support. In other words, it's *"the value you will get on average".*

The expected value is more commonly known as the **average** or **mean**. 

*To explain it a bit easier:*

> Let's play a game with a coin. We flip if and if it lands on tails, you pay me 1 Euro, and if it lands on heads, I will pay you 1 Euro. If we keep this going long enough, the outcome will be 0.
>
> What I'm the only one who's paying? If the coin lands on heads, I give you a Euro, but you won't give me anything when it lands on tails. What's the expected value going to be? 0.5 Euro.
>
> Why? You're still winning either 1 or nothing, so the EV is 0.5 because you're not winning every single time; rather the average amount you win each time will be 0.5 Euro.
>
> If we flip the scenario around, and make you the one who has to pay me, while I give nothing in return, your EV would be -0.5.

You've probably already done this in school at some point, to find the mean, you add up all of the grades, then divide them by the number of grades you have.
$$
m=\frac{\text { sum of the terms }}{\text { number of terms }}
$$



# Types of Probability



## Theoretical probability

Also called the classical probability, it's the mathematical way of calculating how likely something is going to occur; it's a probability based on an ideal situation. Performing an experiment is not necessary. 
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



### Addition rule

When two events, A and B, are mutually exclusive events in the same sample space, then the probability of occurring is the sum of these:
$$
P(A or B) = P(A) + P(B)
$$
For example:

> We have a 6-sided die, and we're interested in the probability of rolling a 1 or a 6.
> $$
> P(1) = \frac{\text { 1 }}{\text { 6 }}
> \\
> P(6) = \frac{\text { 1 }}{\text { 6 }}
> \\
> P(1or6) = P(1) + P(6)
> \\
> = \frac{\text { 1 }}{\text { 6 }} +\frac{\text { 1 }}{\text { 6 }}
> \\
> =\frac{\text { 1 }}{\text { 3 }}
> $$



### Multiplication rule

When two events, A and B, are independent events in the same same sample space, then the probability of occurring is the following product:
$$
P(A ∩ B) = P(A)*P(B)
$$
Perfect to use when calculating more than one event that happens one after another. Simplest example would be a coin toss.:

> Two coins are flipped, what's the probability they both land heads up?
> $$
> P(A and B) = P(A∩B)
> \\
> \text { A: 1st coin lands heads up } P(A)=\frac{\text { 1 }}{\text { 2 }}
> \\
> \text { B: 2nd coin lands heads up } P(B)=\frac{\text { 1 }}{\text { 2 }}
> \\
> P(A∩B) = P(A)*P(B)=\frac{\text { 1 }}{\text { 2 }}*\frac{\text { 1 }}{\text { 2 }} =\frac{\text { 1 }}{\text { 4 }}
> $$
> Since the first coin toss does not influence the second coin toss whatsoever, we can use the formula here.



## Experimental probability

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



## Conditional probability

It's the probability that the event will occur given the knowledge that an event *A* has already occurred *P(B|A)*.  In the case where events *A* and *B* are independent, the conditional probability of event *B* given event *A* is simply the probability of event *B*, that is *P(B)*.

If events and A and B are not independent, then the probability that both events, A and B, occur is defined by:
$$
P(A and B) = P(A)P(B|A)
$$
From here, we need to obtain the conditional probability P(B|A), which is obtained so:
$$
P(B|A)=\frac{\text { P(AandB) }}{\text { P(A) }}
$$
*For example:*

> We're playing a card game, and in order to win, I have to draw 2 cards of the same suit in a row. Out of 52 cards, there are 13 cards in each suit.
>
> Suppose we draw clubs on our first try. This directly influences the desk, as now there are 12 clubs left in the deck of 51 cards.
> $$
> \text { P(Draw second club|First card a club) = 12/51. }
> $$
> 
>
> Another example would be someone applying to collage, with a roughly 80% chance to get accepted. Thing is, this student knows that the dorms will be provided for only 60% of the accepted students. The chance for this student to get accepted *and* to receive dormitory housing is as follows:
> $$
> \text { P(Accepted and Dormitory Housing) = P(Dormitory Housing|Accepted)P(Accepted) = (0.60)*(0.80) = 0.48. }
> $$
> 
>
> If we want to make it a bit more interesting, let's see what happens if our student wants to get accepted by the university, get the dormitory housing *and* not have a roommate. We're adding an extra event here, so to correctly calculate the intersection of more than two events, we have to take into consideration *all* of the preceding events. In which case, it would look something like this:
> $$
> \text { P(A and B and C) = P(A)P(B|A)P(C|A and B) }
> $$
> 
>
> Right, so how are the odds looking like for our student now? Let's say that students who are accepted (A = 80% acceptance rate), and live in dormitory housing (B = 60% have housing in dorms) have roommates 80% of the time. Our student doesn't want a roommate, but would like the two previous conditions to be met, so it would be calculated:
> $$
> P(Accepted and Dormitory Housing and No Roommates)\\ = P(Accepted)P(Dormitory Housing|Accepted)P(No Roomates|Dormitory Housing and Accepted) 
> \\= (0.80)*(0.60)*(0.20) = 0.096
> $$
> 
>
> So, he has roughly 10% of a chance to get a single room at the collage. Tough luck.



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
> \text {P(Voter lives in state B|Voter supports liberal candidate) = }
> \\
> \text { P(Voter supports liberal candidate|Voter lives in state B)P(Voter lives in state B)/}
> \\
> \text { (P(Voter supports lib. cand.|Voter lives in state A)P(Voter lives in state A) + }
> \\
> \text { P(Voter supports lib. cand.|Voter lives in state B)P(Voter lives in state B) + }
> \\
> \text {  P(Voter supports lib. cand.|Voter lives in state C)P(Voter lives in state C))
>  }
> \text {= (0.60)*(0.25)/((0.50)*(0.40) + (0.60)*(0.25) + (0.35)*(0.35)) }
> \\
> \text {= (0.60)*(0.25)/((0.50)*(0.40) + (0.60)*(0.25) + (0.35)*(0.35)) }
> \\\text{= (0.15)/(0.20 + 0.15 + 0.1225) = 0.15/0.4725 = 0.3175.}
> $$
> 
>
> The probability that the voter lives in state B is approximately 0.32.



## Subjective probability

aa







# Probability Distribution

















<center><h1>Statistics</h1></center>



[image]





## Spread & Measurement

![dispersion example](C:\Users\Chloe\Desktop\Main\Statistics images\dispersion example.png)

**Dispersion**, or spread, helps us understand the distribution of data; the extend to which a numerical data is likely to vary, so how spread out a set of data is.

*For example , let's take 2 data sets:*

> X₁ = { 97,98,99,100,101,102,103 }
>
> X₂ = { 70,80,90,100,110,120,130 }

The median for these two data sets is the same (100), but they're different! So, what now? Well, lucky for us, we can calculate the dispersion.



### Range

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

#### Empirical Rule![empirical rule](C:\Users\Chloe\Desktop\Main\Statistics images\empirical rule.png)

If you have a normal distribution, the standard deviation and the mean together tell you where most of your values lie. The empirical rule, or the three-sigma rule or 68-98-99.7 rule, is a rule that tells us that pretty much all data observed will fall within those 3 standard deviations of the mean or average.

So, following this rule, it would mean that 68% of the data falls within one SD, 95% within two SDs, and 99.7% falls within all three standard deviations from the mean.





## Probability Distribution

[what is it]

### Types of distributions

[explain]

#### Normal distribution



#### Chi square distribution



#### Binominal distribution



#### Poisson distribution

# Learning resources

---

https://www.probabilitycourse.com/chapter1/1_5_0_chapter1_problems.php

https://seeing-theory.brown.edu/

https://www.britannica.com/science/probability-theory

https://byjus.com/maths/types-of-events-in-probability/

https://www.scribbr.com/statistics/normal-distribution/\

https://www.investopedia.com/terms/p/probabilitydistribution.asp#:~:text=A%20probability%20distribution%20is%20a,take%20within%20a%20given%20range

https://www.mathgoodies.com/lessons/vol6/addition_rules#:~:text=appropriate%20Addition%20Rule%3A-,Addition%20Rule%201%3A%20When%20two%20events%2C%20A%20and%20B%2C,the%20probability%20of%20each%20event.&text=between%20these%20events.-,The%20probability%20that%20A%20or%20B%20will%20occur%20is%20the,%2D%20P(A%20and%20B)

https://www.encyclopedia.com/education/news-wires-white-papers-and-books/probability-and-law-large-numbers#:~:text=Theoretical%20and%20experimental%20probabilities%20are,theoretical%20probability%20of%20that%20outcome

http://www.stat.yale.edu/Courses/1997-98/101/condprob.htm