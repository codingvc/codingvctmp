---
layout: post
date: 2014-05-16 00:55:00
title: "An Algorithm for Seed Round Valuations"
tags:
- "Valuation"
- "Runway"
---

Your nascent startup is progressing well, and you've decided you want to raise $X at a <a href="{{site.url}}startup-valuations" target="_blank">pre-money valuation</a> of $Y. How do you figure out what X and Y should be? 

In this post, I'm going to outline a potential algorithm for calculating X and Y. Note that valuations are part science, part art, so this algorithm is meant to serve as a good starting point, not as a set of unbreakable rules.

### Step 1: How much do you need?

Come up with a list of all expenses you expect to have over the next 18 months: salaries for existing employees as well as new ones, office space, infrastructure, light marketing/PR, legal/accounting costs, etc. Assume that in the worst case, your monthly revenue, if you already have some, will be stagnant. Add a 10%-20% cushion to provide breathing room. The total of all of these costs is $X -- the number you should be raising.

Why is 18 months the magic duration? It takes up to 6 months to raise a Series A, so raising 18 months of runway right now will give you about a year to put yourself into a good position for raising your next round. 15 months of runway is okay -- that gives you 9 months to make substantial progress. Anything less than 15 months is risky because you might not have enough time to find product-market fit. (Redpoint's Tomasz Tunguz has an <a href="http://tomtunguz.com/seed-followon-rates/" target="_blank">informative post</a> about how much you need to raise to maximize your changes of getting to a Series A.)

### Step 2: What is your target valuation?

Guess the maximum (pre-money) valuation, $Y, that you think you could raise at within ~2 months.

Based on what I've seen in the last few months in Silicon Valley, here are some pre-money valuation benchmarks for companies:

- Pre-product or alpha version of product: $3m-$6.5m. (Occasionally, exceptionally strong teams might raise at $8m-$10m with just an idea.)
- Beta version, a few pilot customers, $1k-$20k in monthly revenue: $6m-$9m.
- Fairly mature product, sales is still high-touch and case-by-case, $25k-$100k in monthly revenue: $7m-$14m.
- Fairly mature product, starting to have repeatable sales process, $100k+ in monthly revenues $15m+. (This is Series A territory.)

(It should be noted that most founders that I talk to are building B2B SaaS products.)

What puts someone at the higher end of each range? Great revenue/growth numbers, strong founding teams, or some sort of unfair advantage (key industry connections, an important patent, etc.)  

You might be wondering about the two month time limit. Obviously you want to get a good valuation, so why limit yourself to the valuation you could raise at within 2 months? Because time is precious. At the seed stage, a company typically has 2-5 people. Fundraising will take up close to 100% of the CEO's time, and burning 4 or 6 man-months is too high a cost when your company is tiny. Startup outcomes are fairly binary (you have a big success or you fail), and whether you own 35% of the company or 33% of the company when it exits won't make a huge difference. Better to own 33% of something successful than to spend a few extra months negotiating for an extra few percent but dooming your company to failure because the product isn't getting any attention. Actually, this is also good advice for investors: if you think a valuation is 50% too high, it's worth negotiating; if you think it's 8% or 12% too high, it's better to just invest than to go into prolonged negotiations that hurt both parties.

### Step 3: Perform a sanity check

Now that you've calculated X, the amount you need to raise, and Y, the valuation you can raise at, how do you tell if X and Y are sensible? Here are a few rules of thumb:

1. If Y is much more than 4X, try to come up with a more aggressive roadmap, since you could probably raise more money with an acceptable amount of dilution. (Y Combinator companies are the exception here -- they often set Y to 7X-8X, perhaps because Y Combinator is already taking a 7% stake.)
2. If Y is between 4X and 6X, start fundraising!
3. If Y is less than 4X, that's too much dilution. It rarely makes sense to give up more than 20% of your company during your seed round -- unless X is very high and will buy you a lot of time.

What do you do if you're facing too much dilution? First, you can try to reduce $X by coming up with a more conservative growth plan (e.g. one that requires fewer hires -- and results in slower growth). Second, you might be able to get away with raising a very small amount now, and then trying to get to a place where you can raise the rest of $X in 6-9 months. For example, if your valuation is too low to raise $1m, you could raise $250k now to hire 1-2 extra people, then try to build enough value to raise $750k at a higher valuation in 6 months. If you don't like either of these options, you can take the dilution penalty as a last resort.

### Caveats

- Just like a very low valuation is bad for your company, a very high one can also hurt your future prospects. The higher your seed valuation, the higher expectations will be for your Series A. If your seed round is at $5m, you might raise your Series A at $16m. If your seed round is at $14m, you might need to be at $30m for your Series A. It's a lot harder to justify a $30m valuation after a year of work.

- Don't raise at multiple valuations in rapid succession in order to pressure investors to decide quickly. Some founders set up complex schemes like "if you invest now, the valuation is $4m; in two weeks, it goes up to $5m; in four weeks, it goes up to $7m." Funds don't like this because it's hard for the them to justify higher valuations to their LPs (i.e. their own investors). As a fund partner, it's unpleasant to go to an LPs and explain that you paid a higher price than another fund just because you found out about a startup a few days after someone else. Most funds will choose to avoid this issue altogether by not investing in your company. Only increase your valuation if you've made meaningful progress.

- Carefully weigh your dilution vs. your time. A startup's two most limited resources are time and money. If you spend a month or two on fundraising, your picked a good valuation. If you needed 6 months, you set your price too high. If you need 1 week, you set your price too low. Don't try to keep an extra 2% of your company if it destroys four months of founder time -- that's not worth it in the first year or two of your startup.

- Frequently, the lead investor in your round will negotiate terms with you. The lead investor frequently helps set the valuation, but it's good to have a number in mind so that you're prepared for the negotiation.

### Common terms investors ask for  

**Pro rata **-- this is the right to invest in your future rounds to maintain a fixed equity stake. A good explanation can be found <a href="http://nystartuphub.com/the-pro-rata-participation-right/" target="_blank">here</a>. Major investors, seed funds, and VCs will always want this right. Angel investors will sometimes want this right.  

**MFN** -- this is the right to get the same terms as the most favored investor in the round. Without an MFN clause, a company can sell equity to one investor at a $6m valuation and to another investor at an $8m valuation. With an MFN clause, every investor would automatically be upgraded to the best terms ($6m, in this case). In my opinion, this is a reasonable request. Investors want to make sure they get the same deal as everyone else, and this term guarantees that. You might still have some flexibility with advisory shares, common stock, or warrants if you really want to give someone a better deal, but everyone will at least be at the same valuation on paper.   

**Board Seats** -- larger investors often want a seat on your board. Some people think it's <a href="http://allthingsd.com/20130927/the-value-of-a-board-at-the-seed-stage/" target="_blank">wise</a> to add board members during a seed round, others <a href="http://steveblank.com/2013/07/09/dont-give-away-your-board-seats/" target="_blank">disagree</a>.

### Additional resources

- <a href="{{site.url}}how-do-investors-value-pre-revenue-companies" target="_blank">How investors value pre-revenue companies</a>
- <a href="http://seanonstartups.co/2014/05/16/what-investors-see-when-they-look-at-you/" target="_blank">What investors see when they look at you</a>

Thank you to <a href="https://twitter.com/CAustinB" target="_blank">Chad Byers</a>, <a href="https://angel.co/dsanka" target="_blank">Dheeraj Sanka</a>, and <a href="http://seanonstartups.co/" target="_blank">Sean Byrnes</a> for giving me feedback on this post.