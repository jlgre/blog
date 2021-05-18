---
title: "Greentings"
date: 2021-05-17T21:09:39-05:00
draft: false
---

# Introduction
My name is Luke Green.
I am a Software Engineer working at [Therapy Brands](https://therapybrands.com/) with [Fusion Web Clinic](https://fusionwebclinic.com) and [Thera-LINK](https://thera-link.com).
All opinions are my own.

I am starting this blog as an exercise in learning more than anything, and if I can share some information along the way that is an added bonus.
A blog will give me an excuse to collect my thoughts about things that I think are important, as well as hopefully receive feedback from others and hear new opinions.
The primary focus of this blog will be Software Engineering, and how it relates to people, the world, and the future.
I cannot promise that will be the only thing mentioned here though.
It is likely that faith, current events, and whatever else I feel like writing about will be sprinkled throughout as well.

For this first post I want to talk about an ever dreaded buzzword: maintainability.

# Software as a Service
Gone are the days of software being finished.
Growing up, albeit in my earlier days, the common distribution of software was in bundled, finished products.
Microsoft Windows operated out of this mindset for much of its life until Windows 10.
Each version of Windows was finished (besides security updates), and to get the next hot version you had to buy it again.

Software now is subscription based, always adding new features, updating frequently.
This fundamentally changes how we must develop software.
In the past, implementation details needed to make sense in the current context.
Now, however, they must also make sense in *future contexts.*
Essentially this boils down do making desicions that are clear, extensible, and flexible.

I am not here to push a particular design methodology, be it Object Oriented or functional.
I do think it is beneficial to examine some common pitfalls and how to avoid them.

# Pitfalls
- Rushing: In the high-pressure, demanding work environment that many software companies can be, it is easy to rush the work you are doing.
In my experience *rushing always takes more time.* Whether it is a hotfix the next day because something got broken, or a rewrite 4 months down the line because of a poor design decision, it always takes more time.
This does not mean not to work quickly.
Quick work is extremely valuable and often necessary, rushing is not.
Take the time needed to adequately do the work.
- Relying on a framework: It can be easy in an opinionate framework (e.g. (Laravel)[https://laravel.com] to rely on the framework to make decisions for you.
In some cases, this may work wonderfully.
In others, not so much.
At the end of the day the responsibility relies on the developer to make good implementation decisions.
Speaking from experience, two of the applications I work on are written in PHP.
One is smaller, and written in Laravel.
The other is vastly larger, and written in a home-grown PHP framework.
The Laravel application is significantly more confusing to work with, because the original designer used the Laravel opinions *at any given time* to make decisions.
The decisions he made from year to year changed significantly in pattern based on the hip, new, Laravel opinion.
- Being lazy: It is more work now to design software well.
Do not take the easy way out.
Refactor, rethink, continue to question your decisions.
