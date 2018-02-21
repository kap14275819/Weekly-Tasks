# Weekly-Tasks-Maths

## Greatest Common Divisor and Least Common Multiple:
#### In maths the Greatest Common Divisor (GCD) is the largest positive integer that divides into two or more intergers which are not all 0.
#### In maths the Least Common Multiple (LCM) is The least common multiple to appear in a list of multiplications of two or more intergers which are not all 0.

### Examples

#### What is the GCD of 22 and 32 ?
#### The divisors of 22 are 1, 2, 11, 12.
#### The divisors of 32 are 1, 2, 4, 8, 16, 32.
#### Both have 1 and 2 in their lists. This means that 2 is the GCD.
#### What is the LCM of 6 and 10 ?
#### The Multiplications of 6 are 6, 12, 18, 24, 30, 36, 42, ... And so on.
#### The Mulitplications of 10 are 10, 20, 30, 40, 50, 60, ... And so on.
#### The LCM in these lists is 30, therefore the LCM of 6 and 10 is 30.

## Conditional Probability:

#### Conditional probability is when the probability of an event (A), given that another event (B) has already occured.

### Examples

#### What is the probability of having a 8 when rolling two die?
#### Chances / Total = 6/36 = 1/6
#### What is the probability of having a 8 after rolling a 2?
#### Chances / Total = 1/6
#### What is the probability of having at least one 2 when rolling two die?
#### Chances / Total = 11/36

## Expectations of an event:

#### What is the probability of a random interger being divisible by 5?
#### Range 1-100 / Total = 20/100 = 1/5

#### What is the probability of a random interger being divisible by 10?
#### Range 1-100 / Total = 10/100 = 1/10

## Intergral calculus
#### The actual definition of ‘integral’ is as a limit of sums, which might easily be viewed as having to do with area. One of the original issues integrals were intended to address was computation of area.
#### First we need more notation. Suppose that we have a function f whose integral is another function F:
#### ![formula1](https://github.com/kap14275819/Weekly-Tasks-Maths/blob/master/Forumlas/formula%201.png)
#### Let a,b be two numbers. Then the definite integral of f with limits a,b is
#### ∫f(x)dx=F(b)−F(a)
#### The left-hand side of this equality is just notation for the definite integral. The use of the word ‘limit’ here has little to do with our earlier use of the word, and means something more like ‘boundary’, just like it does in more ordinary English.
#### A similar notation is to write
#### [g(x)]ba=g(b)−g(a)
#### #### for any function gg. So we could also write
#### ∫baf(x)dx=[F(x)]ba
#### For example,
#### ∫50x2dx=[x33]50=53−033=1253
#### As another example,
#### ∫323x+1dx=[3x22+x]32=(3/322+3)−(3/222+2)=212
#### All the other integrals we had done previously would be called indefinite integrals since they didn't have ‘limits’ a,ba,b. So a definite integral is just the difference of two values of the function given by an indefinite integral. That is, there is almost nothing new here except the idea of evaluating the function that we get by integrating.
#### But now we can do something new: compute areas:
#### For example, if a function ff is positive on an interval [a,b][a,b], then
#### ∫baf(x)dx= area between graph and x-axis, between x=a and x=b
#### It is important that the function be positive, or the result is false.
#### For example, since y=x2y=x2 is certainly always positive (or at least non-negative, which is really enough), the area ‘under the curve’ (and, implicitly, above the xx-axis) between x=0x=0 and x=1x=1 is just
#### ∫10x2dx=[x33]10=13−033=13
#### More generally, the area below y=f(x)y=f(x), above y=g(x)y=g(x), and between x=ax=a and x=bx=b is
#### area =∫baf(x)−g(x)dx=∫right limitleft limit(upper curve - lower curve)dx
#### area =∫abf(x)−g(x)dx=∫left limitright limit(upper curve - lower curve)dx
#### It is important that f(x)≥g(x)f(x)≥g(x) throughout the interval [a,b][a,b].
#### For example, the area below y=exy=ex and above y=xy=x, and between x=0x=0 and x=2x=2 is
#### ∫20ex−xdx=[ex−x22]20=(e2−2)−(e0−0)=e2+1
#### since it really is true that ex≥xex≥x on the interval [0,2][0,2].
#### As a person might be wondering, in general it may be not so easy to tell whether the graph of one curve is above or below another. The procedure to examine the situation is as follows: given two functions f,gf,g, to find the intervals where f(x)≤g(x)f(x)≤g(x) and vice-versa:
#### Find where the graphs cross by solving f(x)=g(x)f(x)=g(x) for xx to find the xx-coordinates of the points of intersection.
#### Between any two solutions x1,x2x1,x2 of f(x)=g(x)f(x)=g(x) (and also to the left and right of the left-most and right-most solutions!), plug in one auxiliary point of your choosing to see which function is larger.
#### Of course, this procedure works for a similar reason that the first derivative test for local minima and maxima worked: we implicitly assume that the ff and gg are continuous, so if the graph of one is above the graph of the other, then the situation can't reverse itself without the graphs actually crossing.
#### As an example, and as an example of a certain delicacy of wording, consider the problem to find the area between y=xy=x and y=x2y=x2 with 0≤x≤20≤x≤2. To find where y=xy=x and y=x2y=x2 cross, solve x=x2x=x2: we find solutions x=0,1x=0,1. In the present problem we don't care what is happening to the left of 00. Plugging in the value 1/21/2 as auxiliary point between 00 and 11, we get 12≥(12)212≥(12)2, so we see that in [0,1][0,1] the curve y=xy=x is the higher. To the right of 11 we plug in the auxiliary point 22, obtaining 22≥222≥2, so the curve y=x2y=x2 is higher there.
#### Therefore, the area between the two curves has to be broken into two parts:
#### area =∫10(x−x2)dx+∫21(x2−x)dx
#### since we must always be integrating in the form
#### ∫rightlefthigher - lowerdx
#### In some cases the ‘side’ boundaries are redundant or only implied. For example, the question might be to find the area between the curves y=2−xy=2−x and y=x2y=x2. What is implied here is that these two curves themselves enclose one or more finite pieces of area, without the need of any ‘side’ boundaries of the form x=ax=a. First, we need to see where the two curves intersect, by solving 2−x=x22−x=x2: the solutions are x=−2,1x=−2,1. So we infer that we are supposed to find the area from x=−2x=−2 to x=1x=1, and that the two curves close up around this chunk of area without any need of assistance from vertical lines x=ax=a. We need to find which curve is higher: plugging in the point 00 between −2−2 and 11, we see that y=2−xy=2−x is higher. Thus, the desired integral is
#### area=∫1−2(2−x)−x2dx.
