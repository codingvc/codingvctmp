---
layout: post
title: "The Value of Data, Part 2: Building Valuable Datasets"
date: 2015-03-05 2:45:00
tags:
- "Value of Data"
- "Business Models"
---
Data is incredibly valuable. It helps create superior products, it forms a barrier to entry, and it can be directly monetized. This post is the second in a 3-part series about making data a core part of a startup's business plan.

### 3-Part Series
<a href="{{site.url}}the-value-of-data-part-1-using-data-as-a-competitive-advantage" target="_blank">**Part 1**</a>: An explanation of why data is becoming increasingly valuable + a catalog of ways in which data creates competitive advantages.  
**Part 2**: How to accumulate data + pitfalls to be aware of. [this post]  
<a href="{{site.url}}the-value-of-data-part-3-data-business-models" target="_blank">**Part 3**</a>:  A catalog of business models where data plays a key role.

In this post, I'm going to talk about tips and strategies for building valuable datasets.

### Attributes of a Valuable Dataset

What should you strive for as you accumulate data? Here are the key attributes of valuable datasets:

1. An ideal dataset is hard for others to build from scratch.
2. An ideal dataset consists of clean, accurate, up-to-date data.
3. An ideal dataset has useful applications. For example, a database of restaurant menus would be quite valuable while a database of shoe sizes would be much less valuable.
4. An ideal dataset grows in value as more people or machines contribute to it. That is, the data has positive network effects.

### Data Sources

Ok, you read the <a href="{{site.url}}the-value-of-data-part-1-using-data-as-a-competitive-advantage" target="_blank">first post</a> in this series and you're convinced that data is great and that you want more of it. But how do you get it? Here are some proven approaches:

* **Direct collection**. Sensors, web forms, surveys, interviews, etc. are all great ways to collect data directly.
* **Crowdsourcing**. Companies like Glassdoor, Yelp, and Waze get data through user contributions. Crowdsourcing is a subset of direct collection, but deserves its own bullet point because users are often unaware that they're helping a company build a data asset. For example, Yelp users write reviews because they want to express their opinions, but those reviews also help build up Yelp's dataset.
* **Paid crowdsourcing**. You can pay employees (frequently these are outsourced employees) or <a href="https://www.mturk.com/mturk/welcome" target="_blank">Mechanical Turk workers</a> to collect data that might be hard to gather without human help.
* **<a href="http://www.techopedia.com/definition/30319/data-exhaust" target="_blank">Data exhaust</a> from tool usage**. A technique that's closely related to crowdsourcing is making use of data exhaust. While crowdsourcing is often a core part of a business model (Yelp only works if people write reviews), "data exhaust" is data that's a byproduct of normal tool usage. For example, Amazon's main purpose is to sell products, but it collects a lot of behavioral data while users shop. What do users search for? Which results do they look at? What do they end up buying? All of that data helps Amazon build internal models of price elasticity, an understanding of which pairs of products are purchased together, and personalized recommendations for each user.  
<br>
Note that almost any tool will have valuable data exhaust. A shopping site accumulates data on searches and purchases. A tool for pharmacists will have great data for predicting sales figures for drug companies. An accounting app for legal departments will have data on how much different legal jobs typically cost. All of this data can be used to make better products for users. Sometimes this data can be directly sold to 3rd parties, too.  
<br>
When in doubt about whether it's worth saving some piece of data, go ahead and save it. You can always delete it later if it doesn't prove useful, but you'd be surprised: a lot of data ends up being valuable if you just get enough of it.

* **Tying many existing datasets together**. Companies like <a href="http://www.factual.com/" target="_blank">Factual</a>, <a href="http://vurb.com/" target="_blank">Vurb</a>, and <a href="http://www.datafox.co/" target="_blank">DataFox</a> all combine multiple data sources in a single place. In fact, Google Search can be thought of as a giant data hub, since Google collects data (content) from many sources (websites) and make it accessible through a unified search interface. This model of data accumulation often involves heavy web crawling, data cleaning, and entity resolution. While the other data collection methods listed above involve the creation of raw data, this approach is about figuring out the connections between existing data sources.

### Tips for Accumulating Data
* **Collect as much data as you can**. Almost any piece of data has value if you're creative, and you can always delete data in the future if you decide it's not valuable enough.
* **Starting collecting data as early as possible**. Data analysis can be postponed until your company is more mature, but data collection cannot be postponed. You can't go back in time to retrieve unsaved data.
* **Prefer raw data to derived data**. Raw data (e.g. every user's rating for a book) is more valuable than processed data (e.g. a book's average rating). The main problem with processed data is that there's no way to un-process it. For example, if you only track average ratings, then you won't be able to figure out how to tweak those ratings when you add the ability to mark some users as spammy. Software bugs can also wreak havoc on processed data. For example, if you never saved individual user ratings and then introduced a bug that miscalculates average ratings, all of your rating data would become worthless. For these reasons, store raw data whenever that's not cost prohibitive.
* **Connect your data with external datasets** The more independent data sources you have access to, the better your insights will be. For example, if you know Bob's email address then you know how to contact him. If you can link the email to Bob's Facebook and LinkedIn profiles, then you'll have a better understanding of his personal and professional interests. If you can get OAuth access to the email account, you'll know what products Bob buys and who he talks to the most. If you tie Bob's location history to business listings then you'll know if he's a gym rat or an art lover or a homebody. You can connect your data to other proprietary datasets (for example, you might purchase business listings from <a href="http://www.factual.com/" target="_blank">Factual</a> or social networking profiles from <a href="http://www.clearbit.com/" target="_blank">Clearbit</a>) or to public datasets (e.g. weather data or US Census data).

### Caveats and Pitfalls

While building up a huge dataset can be great, there are things that can reduce the value of your data. Here are some questions to ask yourself:

* **How severe is the law of diminishing returns for your data?** For some datasets, like car prices, having 10x more data points is probably 3x or 4x more valuable. Each car has many possible configurations, and the more data points you have, the more accurately you can predict a fair price for a specific configuration. For other datasets, like car fuel efficiency, 10x more data might only be 1.01x more valuable. Having 100 data points will let you estimate a Prius's MPG pretty accurately, and increasing that to 1,000 or 10,000 data points will only help a tiny bit. The most valuable datasets will be the ones that don't suffer from quickly diminishing marginal returns.
* **Are there other, simpler ways to accumulate your data?** If you're a credit card company, you might think having online transaction data for lots of consumers is valuable. It is. But you don't have to be a credit card company to get that data: you can be an accounting tool like <a href="http://www.mint.com/" target="_blank">Mint</a>, or a coupon tool like <a href="http://www.joinhoney.com/" target="_blank">Honey</a>, or an email analyzer like <a href="https://unroll.me/" target="_blank">Unroll.me</a>. The harder your dataset is to replicate, the more valuable it will be.
* **How clean/accurate is your data?** Sometimes the usefulness of a dataset is limited by its messiness. For example, a list of book prices is great if each price corresponds to an ISBN number, but less useful if each price corresponds to a book title. (If you see two different prices, is it because one price is for a hardback and one is for a paperback? Or because there are two books with the same title?)
* **How fresh is your data?** If your data says that Google's stock price hit $400 just as astronomers discovered two new moons orbiting the planet Pluto, then that's useful -- if it's 2005. Unfortunately, Google is now at $1100 (split adjusted) and Pluto is no longer considered a planet. As data becomes less fresh, it becomes less and less useful.

### Conclusion

So far, I've covered ways of accumulating valuable data, and how that data can be used as a competitive advantage. In next week's post, I'm going to discuss specific business models that have data at their core.  
<br>
*Thanks to <a href="https://twitter.com/sbyrnes" target="_blank">Sean Byrnes</a>, <a href="https://twitter.com/chadbyers" target="_blank">Chad Byers</a>, <a href="https://twitter.com/eva_ho" target="_blank">Eva Ho</a>, <a href="https://twitter.com/wenwen" target="_blank">Wen-Wen Lam</a>, and <a href="https://twitter.com/shivon" target="_blank">Shivon Zilis</a> for feedback on this post.*