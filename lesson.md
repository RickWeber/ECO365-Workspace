# Scripts

## TL;DR

A script is a clear set of instructions we give to the computer so it can do (some of) our work for us. 


For example, instead of manually looking at sales data and coming up with a guess at how much to ramp up production for Christmas,
a script can load that data, apply a model, generate a prediction, and (with some work that's outside the scope of this class) automatically send an email to the factory manager every week with an updated prediction of the number of orders she should make for each of the upcoming four weeks.

## Intro

Programming languages are often split into "interpretted" and "compiled" languages (warning: I'm about to over-simplify here). R is an interpretted language which means we can interact with it on the console. You type something in, and the R interpretter converts that into "machine code" (the code your computer actually understands), runs that code, gets the result, and displays it appropriately.

```R
> print("hello world")
[1] "hello world"
> sqrt(1 + 1)
[1] 1.414214
```

With a compiled language, we have to write out the whole program, then another program converts the whole thing into machine code, *then* you can run the program. This way creates faster programs, but it can also be harder to write the source code because you don't get the instant feedback of an interpretted language.



### Example

In your job at Schnikey Schneakers you need to help coordinate production in response to fluctuating demand. 

The "simple" but high effort solution is to spend a lot of your time reading spreadsheets and make an educated guess. Then send emails to each of your factory managers: "Hey Susan, I'm *pretty* sure you should get ready for a lot more orders of 'Air Gordons'."

With a bit of effort up front, you can automate this with an R script. You create a simple program that: 
1. Gets the relevant data from the company's databases,
2. creates a model and applies it to the data,
3. then creates some visualizations to show predicted orders (with confidence bars) for each of your product lines, and finally
4. sends an automated email to you and your factory managers.

This has two big advantages. 

First, it's repeatable. The "educated guess" method leaves a lot up to your mental state. Will you make worse decisions when you're sick? What if you get promoted and need to pass this task off to someone new? How do you help them make good predictions without needing access to your hunches and intuition?

Second, it frees up your time to focus on other problems. For example, now that you're getting automated reports sent out, maybe it's time to give even more refined predictions that you wouldn't otherwise have time to make.

It's just a few more lines of code to update your predictions to account for shoe size. You create a new report and find out that only children are wearing 'Air Gordons' so you can cut costs in half by not ordering 
any units in large sizes.

## What are scripts?

## Common Errors and how to prevent them

