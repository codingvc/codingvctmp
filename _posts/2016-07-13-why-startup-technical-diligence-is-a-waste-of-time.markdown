---
layout: post
title: "Why Startup Technical Diligence is a Waste of Time"
date: 2016-07-13 04:08:00
---
In late 2012, I made the transition from software engineering to seed stage investing. I started <a href="http://susaventures.com" target="_blank">Susa Ventures </a> with several friends, and I was going to be the person in charge of all technical diligence. Since practicing software engineers are relatively rare in the VC industry, I (naively) assumed that my background would give Susa a big competitive advantage when making investing decisions. For the most part, I was wrong.

## What should seed stage technical diligence actually measure?

My early attempts at doing technical deep dives turned out to be fruitless for a number of reasons:

* Early versions of a product are often prototypes that are intentionally meant to be rewritten or heavily refactored in the near future.

* Because getting a product in the hands of users is a top priority, even great engineers will intentionally take shortcuts and accumulate technical debt in order to launch sooner.

* The ability to scale with success is important, but designing products for high scalability from Day 1 is usually a mistake. (*"Premature optimization is the root of all evil." -- Donald Knuth*)

* "CTO" is an ambiguous title at small companies. A CTO might be a great coder who is a mediocre manager, or a great manager who is a mediocre coder, or simply a founding engineer who assumes the CTO title to make the founding team appear more well-rounded. Because CTOs often evolve in very different directions after a company hits 5-10 engineers, it's not clear what bar they should be held to. Is it better to have someone who's good at building prototypes quickly? Someone who is a slow prototyper but great at releasing robust software? Someone who may not be a great coder, but who is great at recruiting and managing engineers? It's hard to pigeonhole different types of CTOs into a standardized tech diligence process.

Because code is likely to be temporary and the CTO's role is likely to change quickly, it's not obvious what should be measured during technical due diligence.

(An aside: in addition to tech diligence having questionable value, many seed stage founders consider it overbearing and passively resist it. Given that engineering resources are scarce and that there are plenty of investors who write $100k+ checks after one or two short meetings, founders often prioritize "lighter-diligence investors" instead of submitting to an hour or two of technical grilling.)

## Tech rarely moves the needle
For >95% of startups, however, technical diligence is a waste of time for a more fundamental reason: in today's world of SaaS tools, APIs, and cloud infrastructure, most startup ideas don't have significant technical risk. That means technical resources are rarely the cause of success or the reason for failure.

A quick skim of CB Insights' <a href="https://www.cbinsights.com/blog/startup-death-data/" target="_blank">collection of 150+ startup post-mortems</a> reveals that only ~5% of post-mortems referenced a lack of technical ability/execution. Most startup failures were caused by building the wrong product, or lacking strong sales skills, or not having a viable business model. The presence or absence of amazing engineers was rarely a factor.
 
Another way to analyze the value of engineering is to look at highly-valued private companies: Uber, Airbnb, Snapchat, Pinterest, etc. These are certainly challenging products to work on today because most software is hard at a large enough scale. However, it's doubtful that any of these companies needed 10x engineers for their initial launches. 3x or 2x or maybe even 1x engineers would have been sufficient.

There are, of course, some companies with real technical risk: <a href="http://www.spacex.com/" target="_blank">SpaceX</a>, <a href="http://spectrum.ieee.org/transportation/advanced-cars/meet-zoox-the-robotaxi-startup-taking-on-google-and-uber" target="_blank">Zoox</a>, <a href="http://www.rigetti.com/" target="_blank">Rigetti Quantum Computing</a>, etc. But for a typical consumer app or SaaS tool, technical risk is low enough to be ignored.

## Does anything on the tech side matter?

During the early days of a startup, engineers spend most of their time iterating on the product and recruiting. These are the only things that matter.

On the product side, most engineers have specific areas of strength, and these areas should be well-suited to the product vision. If a product needs great UX, then someone on the team should be a UX designer; if a product will need to handle petabytes of data, then someone on the team should have experience with scalability and distributed systems; etc.

On the recruiting side, a technical founder needs to be someone who can do recruiting and someone whom other engineers want to work for. This is especially true in today's hiring market, which is extremely competitive. The best ideas won't go far if a company can't attract enough talent to launch a product.

Both non-technical cofounders and investors should should be testing a CTO's ability to hire and to build a particular product (either through direct coding or through managing other coders). Notably, these tests don't require having a technical background. Instead, they require the ability to read a resume, common sense, EQ, and a few reference checks.

### Takeaways

My underwhelming experience with due diligence has led me to two key takeaways:

1. If you're a seed investor and you're doing tech diligence on a company, you're most likely wasting your time and the founders' time. 
2. If you're a technical founder or part an all-technical founding team, be very careful not to overestimate the value of technical execution while underestimating the value of non-technical execution. Technical execution enables great software products to exist, but in my experience it doesn't significantly contribute to success or failure for most early-stage companies. The things that lead to success are generally non-technical: being good at understanding customers' needs, being able to design a product that addresses those needs, being good at hiring, being good at customer acquisition, and so on. A well-built product that doesn't solve a problem will always be inferior to an ugly, buggy product that addresses a burning need.

<hr>

If you're interested in a counterpoint to this post, check out <a href="http://medium.com/point-nine-news/a-technical-due-diligence-framework-for-early-stage-startups-c24d5408256e" target="_blank">A Technical Due Diligence Framework for Early Stage Startups</a> by <a href="https://twitter.com/DecodingVC" target="_blank">Rodrigo Martinez</a>.