---
toc: true
layout: post
description: Relfections and lessons I learned while participating in UW-Madison GI Tract Segmentation competition.
categories: [markdown]
title: What I Learned From My First Serious Kaggle Competition
---

# Introduction

Recently I decided that I want to be a Kaggle grand-master, and so I set it out to achieve this goal by breaking it down into multiple steps, the first of which was to win 3 medals (not necessarily gold) by the end of this year.

I participated in UW-Madison GI Tract Segmentation competition without knowing the first thing about semantic segmentation, and through steady effort I was able to win a silver medal and reach the 23rd place (out of 1565 teams - Top 2%).

But through out this time, I often felt unorganized in my approach and distracted by 

1. The shear amount of mistakes and bugs in my code that I want to fix
2. The amount of things and possible improvements that I want to implement
3. The amount of things that I want to learn

# What I learned

So along this way, I came up with a system that isn’t perfect, but currently suits the job.

Also, once the competition finished, I reflected upon this experience to extract some lessons to help me win more competitions, and hopefully you too.


## Make notebook templates to store your code in an organized way

Through out a competition you’ll need 4 kinds of notebooks

1. A notebook for data exploration
2. A notebook for developing ideas
3. A notebook for experimental runs
4. A notebook for inference 

Why do I think you need 4 notebooks? Well not exactly 4, it’s not carved on stone, but you need to organize your code in way that enables you to iterate quickly, and if all of your work is in just one notebook, you’ll find yourself distracted by the different parts you have in there. And whenever you try to reach a part or track something that you’ve written before, it’ll be a nightmare.

## Package the code that you have tested to enable using it in multiple places

Now say that you have written some code and organized it into functions or classes, does it make sense to keep copying it around all of your notebooks?

Or say that you are using something other than kaggle notebooks, does it make sense to copy all of your helper functions in your kaggle notebook?

That doesn’t make any sense. What makes sense is that you package any code that you have written and tested into a local package, and maybe you can even upload that package as a dataset, so whenever you are switching over to kaggle notebooks, you know that your functions will be there too without copying and pasting anything.

## Develop a robust validation plan

![cv-lb-score](https://www.datasciencecentral.com/wp-content/uploads/2021/10/CV_vs_LB.png)

What good are your ideas if you can’t test them? If you don’t have good CV, then you are basically sacrificing your precious work down the drain. 

If you only follow the public LB, you might get shaken up in the end. What you need to do instead is

1. Read the competition guidelines and try to replicate their validation strategy
2. Engage in the discussion forums with other participants and ask about CV if there is something that you don’t get
3. Take some time in the early days to validate the your validation plan by making arbitrary submissions and check CV - LB score correlation

## Keep a log to track what you did on a daily basis

Some days you’ll feel a little bit under the weahter, and maybe you’ll go check the LB and see that your rank is low. 

You’ll take a look at the top X% of the LB and compare yourself. 

You might feel that it’s hopeless to even try, because look at these people, they must be geniuses, and I’m struggling to move up my rank by 1 position.

Please don’t do that. Don’t compare yourself to others, and to avoid that, I suggest keeping a log of everything you do in the competition everyday.

Log every idea you have, every little win you made, every bug you fixed, etc..

![compound-effect](https://seeken.b-cdn.net/wp-content/uploads/2018/02/Compound-Effect-Can-Help-You.jpg)

A log will help you see the trail of compound improvements that you have made since starting the competition, and by the end you’ll be astonished by what you have achieved.

It’s okay to check the leader-board, but don’t get sucked into it. Instead, check this log and be proud of yourself. Compare yourself only with your past self and just keep on making little steps and wins one day at a time.

## Keep a list of any improvement and ideas that come to mind or that you have read which you can try

Often times you’ll get some new ideas that you want to implement, and you might be implementing something just to get a new idea while doing that or based on the results of that idea.

That’s why I suggest keeping a list with literally every idea that you get.

Sometimes you’ll have more ideas that you can implement, and sometimes you’ll have a shortage of ideas, which is why keeping a list is paramount to continuous improvement. 

## Keep a list of any problem that faces you and prioritize solving them

This goes without saying, once a problem occurs you have to make it top priority to solve. Once a problem occurs during submission, like a notebook timeout, or running out of memory, you need to prioritize fixing, or at least understanding why that happens.

Sometimes you can postpone fixing that, and then you might find later that your approach is incompatible and unsuitable for submission. 

So to avoid wasting time and energy, find the root cause of any problem that occurs and prioritize fixing it.

## Keep a list of the things that you need to educate yourself about

Often times you’ll find that you don’t understand something, and it can become overwhelming because this often times for me is like every 5 lines of code when I’m reading someone’s notebook.

So why not keep a list of everything you don’t understand?

Like when you are reading someone’s notebook, a blog post, or a previous competition winning solution. Whenever you encounter something that you don’t understand, add it to the the list, or a list particular to this thing you are reading, and then tackle it one by one.

You’ll find that it was easier than you expected, but the shear amount of things that you don’t know can sometimes be overwhelming.

And if there is something that I want you to take out of this post in general, it is to take everything one step at a time.

## Make a plan based on the three lists that you have for what you should be doing in the next X days

In kaggle competitions (and maybe in life in general), the perfect is the enemy of the good.

Without a plan you’ll find that you are distracted, and whenever you gather the will required to do something, you might procrastinate while saying that maybe what you are trying to implement, learn or fix isn’t going to improve your results anyway.

That’s where a plan comes into place. By now if you have the lists we were talking about, you already know some stuff which you should work on.

So make a plan, and start working on it. Period.

What if that didn’t work out as planned? Well, I guarantee you that most of the time, it won’t work out as planned, but you never know what you don’t know unless you try it.

Sometimes one step of your plan might open up a road that you didn’t know exist, and sometimes a failure or a bug can teach you lessons that you might have not learned otherwise.

The point is, you will be the winner every single time.

So make a plan, follow it, update it based on what you find, and repeat.

### Set a daily time to scan through new notebooks and discussions for any new ideas or information and jot them down in your log and lists accordingly

I can’t emphasize enough how important is this. The beautiful thing about these competitions is that you’ll often find people think a little bit different than you. 

That’s why keeping an open mind while checking the discussion and notebooks is an amazing way to generate new ideas, and maybe be borrow some.

Sometimes you’ll find ideas so simple can provide tremendous improvements, and they haven’t even crossed your mind.

One thing that I found pretty useful too is to sift through similar old competitions notebooks and discussions for useful information, and often times you’ll find some hidden gems.

For example, while working on data augmentation, I didn’t know where to start, and I thought the augmentations used in the public notebook of the competition were either too basic, or too complicated. 

So while looking into a previous competition winning solutions, I found a nice augmentation pipeline, so I tested that, and with a little tweaks I found that my models trained better.

## Believe in yourself

![believe](https://i.pinimg.com/736x/a1/fd/2c/a1fd2c8da7f90f91a59dddd13dbd9eeb.jpg)

I personally find this step a little bit hard, and I don’t know about you. But if you believe that you can’t be winner, you probably won’t be. 

That’s not because you can’t actually be a winner, but because you won’t see the ways that can make you one.

Over confidence is never good, but under selling yourself and having low self esteem won’t get you anywhere either.

Instead, understand your weaknesses and develop them. 

Know your strengths and improve them.

Understand that now one is born with kaggle gold medal (of course some people find it easier that others), but most people start somewhere, and if they want to improve their positioning, they work on themselves and do it.

# TL;DR

1. Make notebook templates to store your code in an organized way.
2. Package the code that you have tested to enable using it in multiple places.
3. Explore and develop and robust CV
4. Keep a log to track what you did on a daily basis
5. Keep a list of any improvement and ideas that come to mind or that you have read which you can try
6. Keep a list of any problem that faces you and prioritize solving them 
7. Keep a list of the things that you need to educate yourself about 
8. Begin everyday by reviewing the log to motivate yourself about the stuff that you have already worked on
9. Always make a plan based on the three lists that you have for what you should be doing in the next 3 days for example to avoid feeling distracted by all the information
10. Set a daily time to scan through new notebooks and discussions for any new ideas or information and jot them down in your log and lists accordingly
11. Don’t watch your models train
12. Last but not least, believe in yourself.
