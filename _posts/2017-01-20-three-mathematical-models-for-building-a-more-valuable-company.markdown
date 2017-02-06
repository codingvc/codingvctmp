---
layout: post
title: "Three Mathematical Models for Building a More Valuable Company"
date: 2017-01-20 05:10:00
tags:
- "De-risking"
---
> "All models are wrong, but some are useful."
> 
> \- George E. P. Box

It's very hard, maybe impossible, to create a mathematical model that describes how to build a successful company. Still, there's value in trying to come up with different models and thinking about their implications. This post describe three possible models for calculating a startup's value and the lessons that each model offers.

## Model #1: A Product of Risk Multipliers
In <a href="https://codingvc.com/how-to-de-risk-a-startup/" target="_blank">How to De-Risk A Startup</a>, I described nine major risks that most startups face, as well as how investors might evaluate each of those risks:

1. **Product/Market Fit Risk** (is your product something that people want?)
2. **Product Quality Risk** (can you build a great product?)
3. **Team Risk** (do you have a great team for achieving your vision?)
4. **Recruiting Risk** (are you able to grow your team effectively with strong talent?)
5. **Sales Risk** (can you and your team sell your product effectively?)
6. **Market Risk** (is your target market large enough to support a huge company?)
7. **Funding Risk** (do you have enough capital to hit milestones that will either let you raise more capital on better terms, or get you to a place where you no longer need to raise capital?)
8. **Short-Term Competition Risk** (are you differentiated enough from existing competitors?)
9. **Long-Term Competition Risk** (will you be able to fend off strong, well-funded competitors in the long-run?)

For each of these categories, we can assign a 'risk multiplier' between 0.0 and 1.0. The more risk there is in a category, the lower the multiplier and the lower the expected value of a company. For example, a company where the team is inexperienced might have a Team Risk Multiplier of 0.2, while an experienced team would have a Team Risk Multiplier of 0.8.

Combining these multipliers, the expected value of a startup might be something like:
<br>
<br>
<img src="{{ site.url }}public/img/risk_formula1.png" style="margin-left:2em;">

(The **∝** sign means 'is proportional to.' This formula is not an equality because it ignores factors like the role of luck, the revenue multiples that companies trade at for a given sector, etc.)

According to this model, the expected value of a company is largely determined by its biggest weaknesses.

## Model #1: Implications

### 1) Startups are like triathlons

The model above suggests that a company's top priority should be reducing its biggest risks. For example, if your startup's risk multipliers are 0.75, 0.75, 0.75, 0.75, 0.75, 0.75, and 0.05, then you should focus on the 0.05. Moving a risk multiplier from 0.75 to 0.90 improves your startup's expected value by 20%, but moving a risk multiplier from 0.05 to 0.25 improves your startup's expected value by 400%.

Under this model, startups are like triathlons. Triathlons consist of three events: a swim, a bike ride, and a run. To be a world-class triathlete, you have be good at all three sports. If you're an amazing runner and cyclist but don't know how to swim, then swimming is the only thing you should be practicing. It won't matter if you can bike or run 10% faster if you can't finish the first portion of the race.

### 2) You have to get most things right
The corollary to the previous implication is that you have to get most things right to build a huge company. If you're going after a $10b market, and you have 10 risk multipliers each of which is currently 0.3, then the expected value of your company will be close to $0. Bringing each risk multiplier up to 0.5 gets you to an expected value of $10m. But your company won't actually get into the $1b+ territory until your risk multipliers are in the 0.8 or 0.9 range and you've de-risked almost every aspect of your business.

### 3) Most investors look for easy reasons to say 'no'
This model hints at why investors often say 'no' to companies quickly without doing much diligence. If the value of one or two of your risk multipliers is very close to 0, then many investors will pass because the 0's drown out everything else. For example, if your funding risk multiplier is 0.01 (maybe you need to raise $50m upfront to implement your business plan, which is nearly impossible), then it hardly matters if other risk multipliers are 0.2s or 0.5s or 0.9s.

### 4) Market size is a critical factor
It doesn't matter how high or low your risk multipliers are, if you're going after a $10m market then you're not going to end up with a billion-dollar company.

### 5) Early stage startup valuations are based on potential
This model explains how two founders can raise money at a $5m valuation on the day their company is founded. While a late stage company's valuation is based on revenue and growth rate, an early stage company's valuation is based on its potential best-case long-term valuation multiplied by the best-case scenario's likelihood. So while the two founders haven't built anything before incorporating, the combination of their idea, skills, and target market might suggest they have a 1% shot of building a $3b company over 10 years. That means the company has an expected value of $30m, and that justifies a $5m valuation today.

## Model #2: A product of categorized risk multipliers

A small tweak to the first model is to group the risks into categories and to treat each category a little differently. The nine risks mentioned at the beginning of this post can be divided into three groups:

1. Your company's current state (product/market fit, product quality, etc.)
2. Your company's ability to execute and to rapidly improve its current state (the strength of your team, your ability to recruit, whether the company culture suppresses talent or amplifies it, etc.)
3. The competitiveness in your target market (short-term + long-term competition risk)

Here's a (somewhat arbitrary) alternative model that reflects how these groupings might determine a startup's value:
<br>
<br>
<img src="{{ site.url }}public/img/risk_formula2.png" style="margin-left:2em;">

Why is execution ability given more weight than a company's current state? Because a company's current state is significantly easier to change than its execution ability. A strong team can quickly iterate on an okay product and make it great, but a weak team will have a hard time even if they start with an initially better product -- and they'll also have a hard time making the team stronger through recruiting because strong players don't like joining teams full of weak players.

In mathematical terms, it's better to have a CurrentState of 0.3 and a team that can improve that by 0.04 every month, than to have a CurrentState of 0.5 and a team that can improve that by 0.01 every month. The model reflects this.

## Model #2: Implications

### 1) You should pursue a monopoly, a large market, or both.
The best way to maximize the rightmost term in this model is to find a market where MarketSize is large or CompetitionFactor is small. Ideally both. If you're pursuing a small or mid sized market with a lot of competition then your chances of building a huge company are slim to none. On the other hand, heavy competition makes it very hard to stand out to customers, even if your company has a superior product and team. 

### 2) People are hugely important in the early days of a company
At inception, a company's CurrentState is close to 0 while its ExecutionAbility might be much higher than 0. The better the team and the faster it can execute, the faster the company's current state will improve. As a result, the quality of a founding team is a very large factor in determining a startup's seed stage valuation. This is why seasoned execs and successful serial founders often command higher seed valuations than first-time founders.

### 3) There's more than one way to increase expected value
There are four ways to make your company more valuable:

1. *Level up your current state*: improve product/market fit, improve the product quality, build up your revenues, etc.
2. *Level up your ability to execute*: hire great people, design a culture that makes people more productive, offer training, build up automation, etc.
3. *Look for adjacent markets that increase market size*: other customers who would buy the same software as your existing customers, other software that your existing customers would buy, etc.
4. *Improve your differentiation*: the better you can differentiate yourself the lower your CompetitorFactor drops. For example, the car industry is very competitive and there are many car manufacturers vying for market share. However, Telsa has managed to differentiate itself so much that it has very little direct competition while still having a chance to capture a large chunk of the entire auto market. Companies that reach this level of differentiation have a lot more potential value and can effectively operate like monopolies.

## Model #3: Achieving success one milestone at a time
<img src="{{ site.url }}public/img/risk_formula3.png" style="margin-left:2em;">

In this model, the key focus is on reaching a progression of major company milestones. These milestones might be things like building an MVP, achieving product/market fit, hitting your first $1m in revenue, or finding a scalable customer acquisition channel. Each milestone increases the value of the company, and each depends on previous milestones -- that is, you can't find product/market fit without building a product, and you can't find a scalable marketing channel until you have product/market fit.

## Model #3: Implications

### 1) Most of your focus should be on the next milestone
If you just reached Milestone #3, you should start focusing on Milestone #4, not Milestone #7. For example, if you just built an MVP, don't worry about hiring the CFO that you'll need if you go public some day, focus on finding a good user acquisition channel instead.

### 2) Lay the groundwork for future milestones
Under this model, your company's value won't increase when you skip milestones. However, if you know your next few goals and know what's needed to achieve them, you can set yourself up for success by laying some groundwork ahead of time. For example, if your current goal is to hit $500k in annual revenue and the next goal is to hire a VP of Sales, then on the one hand most of your focus should be on revenue growth, but on the other hand finding a good VP takes time, so starting to do interviews now is a good idea.

## The value of models
This post presented a few (somewhat arbitrary) mental models for valuing startups. None of these models is ideal**, but each of them has interesting implications for how to maximize the long-term value of a company. While no early stage investor or founder should be explicitly calculating a startup's value using these formulas, the implications are still relevant: you should mostly focus on near term milestones and not things you won't need for several years, you should beef up your company's biggest weaknesses, you should prioritize building a strong team because that has a large impact on everything else in the company, and so on.

There are many unknowns in the early days of building a company, and considering different models of success can be a useful exercise for forcing you to be more explicit about the weights you assign to different objectives and near-term tasks.

<br><br>
*Thank you to <a href="https://twitter.com/sbyrnes" target="_blank">Sean Byrnes</a> and <a href="http://twitter.com/thogge" target="_blank">Tyler Hogge</a> for giving me feedback on this post.* 

<br><br><br>
** Just for fun, here are three examples of these models' weaknesses:

1. The first model assumes all risks are independent, even though they're not (e.g. stronger product-market fit often implies a better product, and a better product reduces sales risk by being easier to sell).
2. In the second model, dividing market size by the number of competitors is unlikely to be correct. A $10b market with 10 competitors will result in one company owning most of the market and everyone else struggling to catch up; it's not likely to result in 10 companies worth $1b each. For example, consider Uber vs. Lyft vs. everyone else.
3. In the third model, there are many milestones that can be achieved in parallel or that do not depend on each other. For example, you can build a sales team and explore marketing channels at the same time, and making progress on either goal will increase your company's valuation.