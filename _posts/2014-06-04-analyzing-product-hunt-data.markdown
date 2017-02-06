---
layout: post
date: 2014-06-04 01:56:00
title: "Analyzing Product Hunt Data"
tags:
- "Data Analysis"
---

During the last few months, I've become a big fan of <a href="http://www.producthunt.com/" target="_blank">Product Hunt</a>, a site that showcases newly released products. Now that Product Hunt's been around for a little while and is getting decent traffic, I thought it might be fun to look at recent submissions to see which products and product descriptions get the most attention. I downloaded the last ~6 months of submissions and spent several hours exploring the data. This post summarizes some of my findings. If you don't want to read the whole thing, the most interesting section is probably "Miscellaneous Observations."

### Basic Stats

- 3285 products were listed on Product Hunt between early December, 2013, and early June, 2014.
- The average number of votes was 16.8. The median was 10. The standard deviation was 20.0.
- A single product has received over 200 votes (<a href="http://www.producthunt.co/posts/notifyr" target="_blank">http://www.producthunt.co/posts/notifyr</a>)
- 3 products have received over 150 votes (<a href="http://www.producthunt.co/posts/stamplay" target="_blank">http://www.producthunt.co/posts/stamplay</a> and <a href="http://www.producthunt.co/posts/product-hunt-search-2" target="_blank">http://www.producthunt.co/posts/product-hunt-search-2</a> and <a href="http://www.producthunt.com/posts/sunrise-2" target="_blank">http://www.producthunt.com/posts/sunrise-2</a>)
- 219 products had 50+ votes. (About 7% of all submissions)
- 715 products had 4 votes or less. (About 22% of all submissions)

Here's a plot of of the vote distribution (each bar represents a single product):
<center>
![Sleeping Kitten]({{ site.url }}public/img/ph-vote-distribution.png)
</center>

### Common Words in Product Names

When looking at words in product names, I noticed 3 main themes.

**Theme #1: Trendy naming conventions**

- **IO** (PredictionIO, Loader.io, Customer.io, Trak.io, ...)
- **iOS** (Mention for iOS, iOS 8, Medium for iOS, ...)
- **Me** (Unwind Me, Vinyl Me, Please, StartupJob.me, ...)
- **2.0** (Jekyll 2.0, Clarity 2.0, Quip 2.0, Crunchbase 2.0, ...)
- **One** (OneTab, One Month HTML, OneTask, One Month Rails, ...)
- **Up** (ThinkUp, CentUp, LendUp, UpCounsel, ...)
- **Box** (BatteryBox, Space Box, RocksBox, ...)
- **Hub** (UsabilityHub, HubYard, ZenHub, ...)
- **Hello** (HelloCar, HelloSign, Hello Ruby, ...)

**Theme #2: ****Software for startups and for product development**

- **Growth** (GrowthHackers, Learn to Growth Hack, Scraping for Growth, ...)
- **Startup** (StartupJob.me, Startups Anonymous, Startup Legitimizer, ...)
- **Design** (Hack Design, Design Triggers, Designer Chat, ...)
- **User** (User Onboarding, Peek by UserTesting, Random User Gen, UserApp, ...)
- **Hack** (Hack Hands, HackDesign, Sell Hack, ...)
- **Code** (CodeShare.io, Design+code, CodeCombat, ...)

**Theme #3: ****Common actions and broad product categories**

- **Mail** (MailCharts, Fake Mail Generator, Proton Mail, Mailbox 2.0, ...)
- **Read** (Beacon Reader, BeeLine Reader, ReadingPack, ...)
- **Share** (Routeshare, Share As Image, CodeShare.io, SupperShare, ...)
- **Work** (Workfrom, Workflowy, WorkingOn, ...)
- **Sketch** (Sketch Deck, Sketch, Sketch Mirror, ...)
- **Video** (Interactive Video, WeVideo, Video Quality Report, ...)
- **Sound** (SoundBetter, SoundCloud Wall, SoundFlake, ...
- **News** (Hacker Newsletter, thenews.im, newsle, Vice News, ...) 

### Most Upvoted Words in Product Names

The following are a few of the words most correlated with high vote counts:

- Anything related to **Product Hunt**:  Product Hunt Jobs,  Product Hunt Radio, Product Hunt Search, etc. (avg. votes=93, n=7)
- **Send**ing things: Sendwithus, DocSend, SendinBlue, Sendy, etc. (avg. votes=46, n=9)
- **Growth** hacking: Growth Hacker TV, Scraping for Growth, Learn to Growth Hack, GrowthHackers (avg. votes=40, n=4)
- **Read**ing: Slicereader, BeeLine Reader, Beacon Reader, FullContact Card Reader (avg. votes=37, n=4)

### Common Words in Product Descriptions

**Theme #1: Common English words**

- **For** ("Google Docs for Video Projects", "A/B Testing for Transactional Email", ...). N=709. The two most common usages were analogies like "Uber for XYZ", and target market/platform specifications like "XYZ for kids" or "XYZ for iOS"
- **Your** ("Finally an app to put your Facebook events on steroids", "A new way to interact with your phone", ...). N=661. Usually used to explain who/what the product is for.
- **Way** ("The easiest way to buy and sell used furniture", "The Easiest Way To Organize An Event", ...). N=107. Typically phrased like "The smartest/simplest/fastest/best/etc. way to XYZ"
- Other common words like **and**, **the**, **to**, **a**, and **with**.

**Theme #2: Adjectives**

- **New** ("Notify tech blogs about your new app", "A whole new swipe to unlock", ...). N=100
- **Simple** ("Shipping made simple", "A simple app to say yo to friends", ...). N=100
- **Free** ("Free tool and method for testing startup ideas", "Free video calling without the hassle", ...). N=73
- **Best** ("The best toy ever for kids!", "A new version of the best weather app!", ...). N=69
- **Beautiful** ("A beautiful new puzzle game for iOS from the makers of Dots", "Typeform makes asking questions easy, human and beautiful", ...) N=51
- **Better** ("Better communication, one page at a time", "Create better content", ...). N=51
- **Easy** ("An Easy Marketplace for Legal Services", "Free and easy online stores", ...). N=45

These are exactly the adjectives I would have expected at the top of the list. :)

### Most Upvoted Words and Phrases in Product Descriptions

- **Product Hunt** (avg. votes = 47.5, n=11)
- **For Developers** (avg. votes = 40.8, n=9)
- **Screenshots** (avg. votes = 39.1, n=8) [This was a surprise to me.]
- **Entrepreneur **(avg. votes = 35.6, n=9)
- **For Startup(s)** (avg. votes = 35.2, n=8)
- **Tinder** (avg. votes = 32.8, n=9). [Tinder for jobs, content, travel, etc.]
- **Documents** (avg. votes = 31.7, n=11)
- **Your App** (avg. votes = 31.7, n=16)
- **With Your Friend(s)** (avg. votes = 31.2, n=8)
- **The Easiest** (avg. votes = 31.2, n=21)
- **In Seconds** (avg. votes = 30.5, n=12)
- **Automate** (avg. votes = 28.4, n=20)  

The two big themes here seem to be _simplicity_ ("in seconds", "the easiest", "Tinder") and _products for developers and startups_ ("for developers", "for startups", "entrepreneur", "your app"). The latter is not surprising since there is a lot of overlap between the startup community and the Product Hunt community.

### Miscellaneous Observations

Some conclusions based on frequently occurring terms in product descriptions:

- "best" is in fact better than "better" (avg. of 19.4 votes vs. 16.3 votes)
- "easiest" is in fact easier than "easy" (25.9 vs 18.0 votes)
- "apps" are nice, but "iOS" apps are awesome (17.8 vs 23.7 votes)
- Users love seeing a better "way" of doing something they already do (avg. of 20.7 votes)
- People like products that are "new" and "free", and they like "more" of them (19.4, 22.2, and 20.4 votes, respectively)
- "Share" and "create"? Meh. (14.2 and 15.7 votes, respectively)
- People value their "friends" and other "people" that they can "chat" with, not just products that proclaim to be "social" (21.8, 18.3, 19.5, and 13.3, respectively)
- Products for your "phone" are much better than "mobile" versions of products (15.7 vs. 10.4 votes)
- "Email"? 23.4 votes. "Video"? 19.4. "Photos"? 13.3.
- A useful "tool" is better than a generic "platform". (21.0 vs. 13.2 votes)
- A "marketplace" is better liked than a "service" (17.8 vs 10.9 votes)
- Users like the "personal" touch (23.7 votes)

(Most of these conclusions have at least several dozen samples for each term.)

### Caveats

This analysis is meant to be more fun than rigorous. The sample size is not huge and I'm not a statistician. I checked my code for obvious bugs, but it might not be perfect. YMMV. IANAL.

### So What?  

This was fun to do with a dataset of 3000 products, but what really excites me is the dataset that Product Hunt will have in a year or two. So many things could be done with a database of tens of thousands of products tied to popularity data and user comments. Are some people great at finding popular products before everyone else? They might make for great VCs. Is "Uber for X" a gimmick, or a product category that everyone values? What are the most compelling adjectives for describing a product? A lot of these questions could be answered with enough data, and I'm looking forward to seeing what the data shows.