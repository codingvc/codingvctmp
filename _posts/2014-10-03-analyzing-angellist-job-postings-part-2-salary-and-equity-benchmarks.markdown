---
layout: post
title: "Analyzing AngelList Job Postings, Part 2: Salary and Equity Benchmarks"
date: 2014-10-03 12:37:00
tags:
- "Data Analysis"
- "AngelList"
---

A few weeks ago, I did <a href="{{site.url}}analyzing-angellist-job-postings-part-1-basic-stats" target="_blank">a basic analysis of AngelList job postings</a>. That analysis looked at attributes like job locations, vesting schedules, and commonly requested skills.

In this post, I'll look at salary and equity numbers based on startup size. In my experience, founders frequently give out equity grants that are too generous or too stingy. The dangers of stinginess are that candidates will choose to work somewhere else and that you will waste a lot of time interviewing people who definitely won't take your offer. The danger of generosity is that, especially for the first few hires, you are giving away much more equity than you need to. That equity could be used to give stronger offers to multiple candidates later on, to raise more money from investors, or to retain more decision-making power for founders.

### Background

Every job posting on <a href="https://angel.co/jobs" target="_blank">AngelList</a> has a salary range and an equity range. For example, at the time of this writing, <a href="https://angel.co/casetext/jobs" target="_blank">Casetext</a> is hiring a full-stack software engineer and offering $90k - $125k in salary and 0.3% - 1.5% in equity.

Two notes on these ranges: first, the more senior and well-qualified you are, the closer your offer will be to the top of the company's salary/equity ranges. Second, a lot of companies will let you trade equity for salary. That is, if a company is offering 1% - 2% equity and $100k - $130k salary, a specific candidate might get to choose between $100k and 1.75% or $125k and 1.2%.

### Methodology

I used <a href="https://angel.co/api" target="_blank">AngelList's API</a> to find all full-time jobs in Silicon Valley that were posted in the last 2 months and offered salaries of at least $20k. I then checked LinkedIn and manually counted the number of employees at each company. (This was exactly as fun as it sounds.) To keep the manual work manageable, I limited the companies I was looking at to those with an AngelList Signal score of 6 or more, which cut the number of companies in half. All of these filters resulted in a list of jobs at over 300 startups. Finally, I grouped startups by the number of employees they had, then graphed the equity and salary offers for different company sizes.

### Caveats

My methodology is far from perfect, and there are lots of areas where fuzziness was introduced. For example, not everyone is on LinkedIn, so employee counts based on LinkedIn data won't be perfectly accurate. The following data is meant to provide ballpark ranges for salary and equity offers. Please don't treat it as gospel.  

### Summary of Results

_Note: These are benchmarks based on a medium-sized sample; they're not hard-and-fast rules. **The benchmarks are for engineering jobs in Silicon Valley. **(Non-engineering jobs are discussed at the end of this post.)_  

Assuming that a startup has two founders, here are some ballpark numbers for _engineering_ job offers:  

**Salary**:

- For employee #1:
    - 20th percentile salary range is $70k - $100k
    - 50th percentile salary range is $80k - $120k
    - 80th percentile salary range is $82k - $135k

- For employees #2 through #13, salaries rise for higher paying jobs:
    - 20th percentile salary range is $75k - $100k
    - 50th percentile salary range is $85k - $125k
    - 80th percentile salary range is $100k - $150k

- For employees #14 through #35, salaries rise for lower paying jobs :
    - 20th percentile salary range is $78k - $120k
    - 50th percentile salary range is $90k - $134k
    - 80th percentile salary range is $102k - $150k  

Lower salary ranges tend to be for more junior or more specialized roles (e.g. front-end engineer). Higher salary ranges tend to be for more senior roles, or for full-stack engineers. That is, a Junior Front-End Engineer is more likely to get an offer in the 20th percentile, while a Senior Full-Stack Engineer is more likely to get an offer in the 80th percentile.

**Equity**:

- Hire #1: 2% - 3% of equity
- Hires #2 through #5: 1% - 2%
- Hires #6 and #7: 0.5% - 1%
- Hires #8 through #14: 0.4% - 0.8%
- Hires #15 through #19: 0.3% - 0.7%
- Hires #21 through #27: 0.25% - 0.6%
- Hires #28 through #34: 0.25% - 0.5%

These ranges indicate the _maximum_ equity amounts offered by companies. These amounts are typically reserved for ideal candidates, or candidates who are very senior. If you're just out of college or not a perfect fit for a company, you will probably get a little (or a lot) less. A good way to frame these numbers is to add "up to" before each range. For example, a typical 6th hire will get _up to_ 0.5%-1%.

Given the recent attention to burn rates, one interesting observation here is that the first ten employees of a company will own about 12% of the company, and will cost, on average, about $100k/month for salary alone. Companies that are able to raise $1.5m+ seed rounds are fortunate because they can usually get about 18 months of runway as their team grows from a few founders to 10-15 people.

### Salaries for Engineers  

After employee #1, salaries for employees were relatively close together, with one noticeable jump occurring around the 13th or 14th hire. I suspect this is around the size of a company raising a Series A, and as soon as an A round is closed, the company increases salaries a little bit.

Here are graphs of min/max engineering salaries:

<center>
<a href="{{ site.url }}public/img/angellist-salary-eng-min.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-eng-min.png" alt="Min Eng Salaries"></a>
</center>

<center>
<a href="{{ site.url }}public/img/angellist-salary-eng-max.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-eng-max.png" alt="Max Eng Salaries"></a>
</center>

The way to interpret these graphs is that the horizontal axis is the salary's percentile among all other salaries. For example, if a company is offering a salary range of $90k - $140k for an engineer who will be the 8th employee, then we can see that $90k and $140k are each at the 60th-70th percentile on their respective graphs, so the salary offer is pretty good (better than 2/3 of startups).

### Equity for Engineers

The following graphs are histograms for max equity stakes of different job offers. Each bar represents a single startup's offer. For example, the first graph shows that for hire #1, 6 startups offered up to 2% equity, 4 startups offered up to 3%, and 3 startups offered up to 5%.

<center>
<a href="{{ site.url }}public/img/angellist-salary-equity-1.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-equity-1.png" alt="Equity Employee #1"></a>
</center>

<center>
<a href="{{ site.url }}public/img/angellist-salary-equity-2-5.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-equity-2-5.png" alt="Equity Employees #2 - #5"></a>
</center>

<center>
<a href="{{ site.url }}public/img/angellist-salary-equity-6-11.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-equity-6-11.png" alt="Equity Employees #6 - #11"></a>
</center>

<center>
<a href="{{ site.url }}public/img/angellist-salary-equity-12-21.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-equity-12-21.png" alt="Equity Employees #12 - #21"></a>
</center>

<center>
<a href="{{ site.url }}public/img/angellist-salary-equity-22-35.png" target="_blank"><img src="{{ site.url }}public/img/angellist-salary-equity-22-35.png" alt="Equity Employees #22 - #35"></a>
</center>

I expected to see a consistent drop for each additional employee, but was surprised to find that offers remained consistently high for many employees at a time. For example, the equity for Hire #5 is often similar to the equity for Hire #2. This feels like a market inefficiency, as Hire #5 is taking on much less risk than Hire #2.  

### What about latecomer VPs, Directors, etc?

The dataset only had 7 data points for VPs and Directors of Engineering who came in when a company already had 10+ people. In those cases, their equity stakes were at the top of the ranges for their employee numbers (e.g. 1.5% for a VP who was employee #13), and their salary ranges were consistently around $120k - $180k.

### What about non-Engineers?

The sample size of non-engineering jobs at early stage companies is too small to analyze rigorously. That said, here are some high-level observations:

**Sales jobs**

VPs tend to get 1%-2%. Directors tend to get 0.5% - 1.0%. Salary ranges for directors are often $80k - $140k.  

Non-director role salaries were very inconsistent, ranging from $40k - 60k to $80k - $120k (for the same job titles). Presumably there's also a commission structure, but that's not captured by AngelList.

Equity stakes for non-director roles were generally 1% or less. For the first 10 hires, equity was typically 0.3% - 0.5%, then dropped off to 0.1% - 0.2% for subsequent hires.

**Marketing jobs**

VPs: not enough data

Directors at &lt; 15-person companies: $80k-$120k, 0.5% - 1.0%

Directors at &gt;= 15 person companies: $120k-$180k, 0.25% - 0.5%

**UI/UX/Designer jobs**  

Median salary range was around $80k-$130k.

Designers among the first four hires get up to 1-2% equity, occasionally only 0.5%. Designers among next 5 hires get up to 0.5% - 1.0%. 0.2% - 0.5% for employees #10-30.

I'd like to reiterate that there wasn't enough data to deeply analyze non-engineering jobs. There were sales reps who joined early and only got 0.05% stakes, as well as marketers who joined late and got 1% stakes.   

### What about outside of Silicon Valley?

I chose to focus on Silicon Valley because the dataset was more manageable. For other locales like NYC or Houston, a hack that might work is to look at a dozen random, high-quality companies and see how their offers compare to Silicon Valley's. Seeing where those offers fall can help calibrate expectations.

### That's a lot of data. Now what?

There are four common problems with startup job offers:

1. **The founder's offer is too generous.** In this case, the employee will be happy in the short term, but the company suffers in the long term. If the founder gives away 10% more than they should to the first 10 employees, then that's 10% less that's available for fundraising and future equity grants -- and that might break the company.
2. **The founder's offer is too stingy.** In this case, the entire interview process is usually a waste of time for both parties. Furthermore, even if an employee takes the offer, it's harder to retain them because they'll either resent the founder once they realize they're being paid below market, or they'll just move to a company that pays better.
3. **The employee's expectations are too high.** In this case, the interview process is likely a waste of time, and the employee is likely to pass on multiple good job opportunities before realizing they have unrealistic expectations.
4. **The employee's expectations are too low.** If a founder exploits this, it hurts long-term retention and builds long-term resentment among employees.

The goal of this analysis is to increase transparency, which can help mitigate these four issues. The benchmarks are just rough guidelines, but they can be helpful if the employee expects to receive 2% while the founder thinks 0.2% is fair, or vice versa.  

As a parting thought, I'd like to reiterate that these are not rules, they are starting points. There are plenty of reasons to have higher equity grants (e.g. a specific employee can change the entire direction of a company) and plenty of reasons for lower grants (e.g. there are significant non-financial perks, like working with an amazing founder or working on a particularly meaningful project).

<i>Thanks to <a href="http://numeratechoir.com/" target="_blank">Mike Greenfield</a> and <a href="http://ml.posthaven.com/" target="_blank">Cheng-Tao Chu</a> for feedback on earlier drafts of this post.</i>