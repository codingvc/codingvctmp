---
layout: post
title: "The Value of Data, Part 1: Using Data as a Competitive Advantage"
date: 2015-02-27 2:45:00
tags:
- "Value of Data"
- "Business Models"
---
Data is incredibly valuable. It helps create superior products, it forms a barrier to entry, and it can be directly monetized. This post is the first in a 3-part series about building companies that leverage the value of data.  

### 3-Part Series
**Part 1**: An explanation of why data is becoming increasingly valuable + a catalog of ways in which data creates competitive advantages. [this post]  
<a href="{{site.url}}the-value-of-data-part-2-building-valuable-datasets" target="_blank">**Part 2**</a>: How to accumulate data + pitfalls to be aware of.  
<a href="{{site.url}}the-value-of-data-part-3-data-business-models" target="_blank">**Part 3**</a>: A catalog of business models where data plays a key role.

In this post, I'm going to talk about how the increasing commoditization of software and hardware makes data more valuable, and how data can be used to create competitive <a href="http://www.investopedia.com/terms/e/economicmoat.asp" target="_blank">moats</a>.

### Hardware and Software Commoditization
During my decade of working as a developer I saw some major changes in the software industry:

LinkedIn in 2003-2005:

* _Software_: core pieces of the software stack (web servers, DB connectors, etc.) were free and open source. Almost everything else had to be built from scratch. I remember paying a lot of money for Oracle licenses because MySQL wasn't very mature at the time.
* _Hardware_: our servers were installed at a nearby <a href="http://en.wikipedia.org/wiki/Colocation_centre" target="_blank">colo</a>. If there was a problem with one of the machines, our IT guy, Ian, had to drive to the colo to physically diagnose the issue.

Factual in 2009-2012:

* _Software_: while the core software stack was still free and open source, there were now numerous libraries and frameworks available for things like web caching, HTML parsing, and machine learning algorithms.  
* _Hardware_: just like at LinkedIn, we started out with servers in a colo. However, by the time I left in 2012, a lot of our software was running in Amazon's cloud.

Today:

* _Software_: the amount of free, hiqh quality, off-the-shelf software has continued to grow at a staggering pace. You can download plenty of amazing code for free, and pay for SaaS tools when free solutions are insufficient. For less than the annual cost of a developer, you can incorporate technologies like cutting edge <a href="http://wise.io" target="_blank">machine learning as a service</a>, <a href="http://www.alchemyapi.com/" target="_blank">natural language processing as a service</a>, and <a href="https://cloud.google.com/translate/docs" target="_blank">language translation as a service</a> into your product.
* _Hardware_: containerization via tools like <a href="https://www.docker.com/" target="_blank">Docker</a> means that your software can be deployed to almost any cloud with a few clicks, then monitored with increasingly <a href="https://www.scalyr.com/" target="_blank">sophisticated, yet easy-to-use DevOps tools</a>. It's easier than ever to be a developer and never worry about physically setting up machines. In 2009, you might have gotten funny looks if you were deploying to the cloud; today, you might get funny looks if you're not. 

On the software side, developers have gone from writing low-level libraries to using pre-built libraries to using sophisticated, feature-rich APIs. On the hardware side, we've gone from buying machines and storing them a few miles from the office to deploying everything to the cloud.

The trend is clear: both software and hardware infrastructure are becoming more and more commoditized. So what's left if you're trying to build a company with sustainable competitive advantages? **Data**.

### Data Moats
Large, meaningful datasets are incredibly hard to build, which is part of what makes them so valuable. A recent trend is for tech companies to open-source non-core software because it's good for the community and also good marketing. For example, Netflix has publicly released many of its <a href="http://netflix.github.io/#repo" target="_blank">infrastructure and monitoring tools</a>.

However, while companies will publish some of their code, it's very unusual for them to release their data. That's because while it's possible to replicate software with a strong engineering team, it's very hard to replicate meaningful datasets without large user bases (or very complex web crawling/scraping pipelines). This is an ideal competitive moat: a company can't copy your product without the corresponding dataset, but that dataset can only be built via an existing heavily used product -- a catch-22!

Of course, the scarcity of good datasets is just part of their value. The remaining value lies in the hard-to-copy applications that are enabled by large amounts of data. Here are some ways to apply data to create more defensible products:

* **Data helps you provide great content recommendations**. Examples: Google's search relevance, Netflix's movie recs, Amazon's product recs, Facebook's news feed, and OKCupid's personality matching. More data enables better recommendations, and once users become accustomed to great recommendations, they won't want to try competing services.
* **Data helps you provide more accurate ad targeting**. Examples: ads on Google, YouTube, Facebook, and Twitter. Ads are similar to recommendations, but ad targeting is often based on data from many sources instead of just one source. Better ad targeting leads to more revenue, which lets you outspend competitors in areas like product development and customer acquisition.
* **Data helps you optimize pricing and offer pricing transparency**. Examples: Amazon, eBay, almost every adtech company, and the airline industry. Companies that have a lot of historical transaction data can set prices to optimize profit (or revenue, or user happiness), and they can also make price trends more clear to their customers, thereby earning more trust (e.g. Kayak's flight price predictor).
* **Data helps you provide a definitive destination for some type of content**. Examples: Quora for Q&A, Yelp for restaurant reviews, Stack Overflow for tech questions, TripAdvisor for travel reviews, Glassdoor for salary comps, AppAnnie for mobile app stats. The more data and content these companies have, the more trusted they become (at the expense of their competitors). At this point, even if someone makes an amazing restaurant review app, it would be next to impossible to compete with Yelp because Yelp has so many rich reviews (and the new entrant has none).
* **Data helps you provide actionable insights**. Examples: Yelp highlights popular phrases from reviews (like which menu items are popular), <a href="https://www.framed.io/" target="_blank">Framed Data</a> helps predict which customers are going to churn and what factors make them likely to churn. The more data you have to analyze, the more accurate and useful your insights will be.
* **Data helps you make operations more efficient**. Examples: Amazon's inventory management, BuzzFeed's content curation, Uber's automatic driver dispatching, and <a href="https://www.flexport.com/" target="_blank">Flexport's</a> logistics streamlining. The more usage data you have, the better you can organize operations around predicted usage patterns.
* **Data helps you provide more accurate models and predictions**. Examples: <a href="https://siftscience.com/" target="_blank">Sift Science</a> (fraud detection), <a href="https://blockscore.com/" target="_blank">BlockScore</a> (ID verification), <a href="https://www.lendup.com/" target="_blank">LendUp</a> (credit scoring), <a href="http://www.climate.com/" target="_blank">Climate Corp</a> (crop insurance). The more data you have, the more accurate your models will be.
* **Data helps you improve categorization/tagging/sentiment analysis**. Examples: Facebook (facial recognition), <a href="https://www.atlaswearables.com/" target="_blank">Atlas Wearables</a> (exercise categorization). The more data you have, the easier it is to automatically categorize things like images or book plots or website content.
* **Data helps you improve language parsing/semantic analysis**. Examples: Siri, <a href="https://x.ai/" target="_blank">x.ai</a>, <a href="https://wit.ai/" target="_blank">wit.ai</a>, <a href="https://casetext.com/" target="_blank">Casetext</a>. The more training data you have about what people meant when they said or wrote something, the better you can predict what a given piece of text means.
* **Data helps you create better AIs**. Examples: self-driving cars, Wolfram Alpha. More training data makes it possible to train smarter AIs.

In each of these cases, bigger datasets created bigger competitive advantages. At some point, competitors can no longer catch up to you -- even if their products are superior -- because they don't have the data that you have.

This is by no means an exhaustive list of competitive advantages, and if you have suggestions for other ways that data helps make products more defensible, please let me know on <a href="https://twitter.com/lpolovets" target="_blank">Twitter</a>.  

Next week, I'll cover effective ways to accumulate data, as well as what to watch out for as you're building up your data assets.  
<br>
Additional resource: <a href="https://www.slideshare.net/pskomoroch/building-competitive-moats-with-data" target="_blank">Building Competitive Moats With Data</a> by <a href="https://twitter.com/peteskomoroch" target="_blank">Pete Skomoroch</a>  
<br>
*Thanks to <a href="https://twitter.com/sbyrnes" target="_blank">Sean Byrnes</a>, <a href="https://twitter.com/SethGB" target="_blank">Seth Berman</a>, and <a href="https://twitter.com/eva_ho" target="_blank">Eva Ho</a> for feedback on this post.*