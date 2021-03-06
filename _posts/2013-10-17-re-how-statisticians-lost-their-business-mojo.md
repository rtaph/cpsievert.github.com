---
layout: post
title: "RE: How Statisticians Lost Their Business Mojo"
author: Carson Sievert
categories: [statistics, business]
tags: [statistics, business]
---
{% include JB/setup %}

I recently stumbled across [@statwonk](https://twitter.com/statwonk)'s post on [how statisticians
lost their business
mojo](http://statwonk.github.io/blog/2013/10/11/how-statisticians-lost-their-business-mojo/). The
article starts out with some very strong points about our obsession with p values and their lack of
relevance in a business setting. While I agree that effect sizes (i.e., confidence intervals) are
more useful in many situations, I don't agree with everything in this post. In particular, this
excerpt got my blood boiling:

"Refrain from imposing linearity and variable selection by tests of significance (p-values).
Instead minimize rates of error in held out test set data using a training set. This opens up a
HUGE new space to do analysis, all without p values! Non-parametric methods like random-forest,
SVM, boosting, bagging, sophisticated loss functions (read maximizing revenue with respect to
minimizing cost, profit!)."

This seems like an attempt to bash on traditional statistical methods simply because most
statistical models require assumptions. While some machine learning tools like random-forest and
support vector machines may not require similar assumptions, the trade-off is a lack of
interpret-ability. I agree that these tools are helpful *provided that your goal is prediction*.
However, if there is any skill that statisticians can hold over data scientists (if any difference
really exists), it's their ability to explain real-world phenomena in a simplistic manner. If you
call yourself a statistician and you restrict yourself to non-parametric methods, then *you're
doing it all wrong*.

This statement also implies that statisticians are reduced to regression assumptions that are
taught in introductory courses. There are a number of ways to work around non-linearity and/or
non-constant variance using a parametric approach. There also grotesque number of ways to perform
model selection. Again, how you actually deal with these issues should depend on your goals! If
you're interested in prediction, why aren't you doing model selection via cross-validation (which
is agnostic to the choice of model)? In that case...look ma, no p values! Furthermore, a loss
function (no matter how "sophisticated") should not be coined a non-parametric method. Rather, it's
a criteria for evaluating the performance of (possibly parametric) model.

I've probably lost most of you my now, which may be why "Statisticians Lost Their Business Mojo".
Let's be honest, the statistician's tendency to be careful, critical, and thorough when
communicating their work generally doesn't translate well in the business world. As a result,
people tend to put an artificial box around the capabilities of the statistician.

Besides the mainstream misunderstanding of statisticians, I think "Statisticians Lost Their
Business Mojo" because of their slow response to the increase in computational capability. I think
too many (applied) statisticians neglect their programming skills because they think that someone
or something will do that work for them. But in many businesses nowadays, people need to have a
well-rounded skill set in order to be employable; which is probably why the data scientist has more
"business mojo" nowadays compared to the statistician.
