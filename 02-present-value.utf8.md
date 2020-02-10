

# Present Value {#Present-Value}

Having \$100 today isn't the same as having \$100 next year. I want to buy new shoes, and I don't want to wait a year. I don't waiting any fun, and I don't think I'm alone in that. Buying my shoes has a cost, though. Not only am I out of \$100 today. I'll be out even more money later, because I won't be able to throw it the bank. It'll earn interest in a savings account, and I'll make a couple dollars a year just off the interest. 

This is the most important idea in all of finance: Having \$100 today isn't the same as having \$100 some other day. It's called the **time value of money**, and it exists because money saved up in bank account earns interest. We're going to spend the next few minutes figuring out what that actually means. 

## The Time Value of Money

Let's say I get wake up to find that \$100 has magically appeared under my pillow. I can buy those shoes I'm after, or I can put it in the bank. How much money am I "losing" if I buy them? That depends on two things - the *interest rate* my bank account earns, and *how long* I leave the money in the bank. We need to know two things - my *interest rate*, and how long I leave the \$100 in the bank. There's an entire chapter on how to choose what interest rate to use, but for now I'm going to assume I can get 1.5% per year from a savings account. 

As for how long I leave it in the bank, let's pretend that today is New Year's Day 2019, and see what happens if I leave \$100 in the bank for 1 year or 3 years. A quick-and-easy diagram will help us see what happens. I'll be drawing one every time I have to move money backwards or forwards in time, because I find visualizing the problem makes it so much easier to understand.  



### 1 Year

<!-- https://github.com/daattali/timevis/issues/45 -->
<img src="shoes_1year_Q.png" width="960" />

Here's our first diagram. The goal is to fill in the box that has no number. I've put a short question in that box so that we know what we're trying to find. The diagram shows that we deposited \$100 into the bank on January 1, 2019 and asks how much it will be worth on January 1, 2020. We know it gets 1.5% of interest in that first year, so it goes up by 1.5%. Starting off with \$100 and adding 1.5%, we get:

$$\begin{aligned}
  $100 + \$100 * 1.5\% &= \$100 * 101.5\% \\
                       &= \$101.50
\end{aligned}$$

I like using decimals instead of percent. If we do that, we get: 

$$\begin{aligned}
  $100 + \$100 * 0.015 &= \$100 * 1.015 \\
                       &= \$101.50
\end{aligned}$$

<img src="shoes_1year_A.png" width="960" />

You can use either decimals or percent, but either way we have number we're after - \$101.50. I've redrawn the diagram with \$101.50 filled in, so that I know I've got it. 

### 3 Years

If we want to know how much \$100 grows to in 3 years, we get a new diagram. And just so I can put in my back pocket, I'm also going to figure out how much \$100 grows to in 2 years. 

<img src="shoes_3year_Q.png" width="960" />

Putting it together, I get a diagram with two boxes filled in (2019 and 2020), and two boxes to fill in (2021 and 2022). I have two choices on how to find the number for the *"In 2021?"* box. I can bring the \$101.50 from 2020 forward by 1 year. 

$$\begin{aligned}
  $101.50 * 1.015 &= $103.02
\end{aligned}$$

Or, I can bring the \$100 from 2019 forward by 2 years. Since I'll be getting 2 years of interest, I have to multiply my \$100 by 1.015 *twice* to do that. 

$$\begin{aligned}
  $100 * 1.015 * 1.015 &= $100 * 1.015^2 \\
                       &= $100 * 1.03023 \\
                       &= $103.02
\end{aligned}$$

I get the same number either way - \$103.02 - but the second way is faster. To find out how much it would be worth *"In 2022?"*, I'll bring the \$100 forward by 3 years. 

$$\begin{aligned}
  $100 * 1.015^3 &= $100 * 1.015^3 \\
                 &= $100 * 1.04568 \\
                 &= $104.57
\end{aligned}$$

I've got the numbers I'm after - \$103.02 and \$104.57. I'll re-draw the diagram with these filled in, so I know I've got what I'm after. 

<img src="shoes_3year_A.png" width="960" />

### The Big Idea 

Here's the big idea: if the interest rate really is 1.5%, then \$100 in 2019 is the worth *the same* as \$101.50 in 2020, \$103.02 in 2021, and \$104.57 in 2022. I can save \$100 in 2019 and have that much in 2020, 2021, or 2022 if I get 1.5% in interest every year. They're literally worth *the same*. 

That might sound impossible, but let's go back to me trying to decide between getting \$100 today or next year. At 1.5%, we've seen that \$100 today grows to \$101.50 in a year. If I take \$100 next year, I'll just have \$100. If I want to get the same amount of money next year, I *have to* get \$101.50 next year to match what would be in my bank account. If I just get \$100 next year, I've lost the \$1.50 I would earned in interest. 

The same argument goes for any of the dollar amounts on the diagram, and even inflation doesn't change the picture. I just have to use the *real* interest rate (instead of the *nominal* interest rate, like I've done here), and I'll still be able move money backwards and forwards in time so that all the account values are worth *the same*. 

That's the big idea behind the **time value of money**: if we know the appropriate interest rates to use, we can know how much money is worth at any point in time (in the past *or* in the future).


## Finding Present Value 

You might ask: how much money *today* is the same as \$100 next year? That's just as easy to find. Let's draw our diagram and fill in the missing number. 

<img src="PV_1year_Q.png" width="960" />

To move money forward in time, we multiplied by the interest rate. To move money backwards in time, we have to divide by the interest rate. We're earning 1.5%, so we have to divide the \$100 we have in January 2020 by 1.015 to find it's value in January 2019. 

$$\begin{aligned}
  \frac{$100}{1.015} &= $98.52
\end{aligned}$$

<img src="PV_1year_A.png" width="960" />

This diagram says that \$98.52 today is worth *the same* as \$100 next year, if we earn 1.5% in interest from the bank. There's a special name for \$98.52 - it's the *present value* of \$100 one year from now. We also call it by a much more suggestive name - the *price*. That's because it's how much I have to "pay" the bank today to get \$100 next January. <!-- It's very important to understand the time value of money *and* present value, because we're going to be using them to price bonds for the rest of the book. -->

Before we get to bonds, let's do a more complicated present value calculation. This one has four \$5000 deposits made at the beginning of every year for the next four years. The game plan is that we're going pull back each \$5000 payment to it's price *today*, and then add those up. We have to bring the dollar amounts to the *same day* before adding them up because money at different points in time is *not comparable*. We *must* control for the interest the deposits can earn before we can add them. We're going to do that by bringing all the dollar amounts to January 1, 2019.

<!-- https://github.com/daattali/timevis/issues/45 -->
<!--
<img src="multiple-deposits.png" width="960" />
-->
