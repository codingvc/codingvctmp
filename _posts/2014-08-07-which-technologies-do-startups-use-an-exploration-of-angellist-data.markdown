---
layout: post
date: 2014-08-07 06:54:00
title: "Which Technologies Do Startups Use? An Exploration of AngelList Data"
tags:
- "Data Analysis"
- "AngelList"
---

There's a lot of hype surrounding new programming languages, databases, and the like. I've always been curious about which technologies are actually in use, and whether great startups use different technologies than not-so-great startups.

Fortunately, AngelList offers some self-reported data about technology usage. For example, you can see that <a href="https://angel.co/robinhood" target="_blank">Robinhood</a> uses Python, Django, and iOS while <a href="https://angel.co/secret" target="_blank">Secret</a> uses Java, Go, Python, JavaScript, HTML5, CSS, iOS, and Android.

Additionally, AngelList calculates a Signal score for each startup. While it's not 100% clear what this represents, it seems to be some combination of company quality and popularity. For example, <a href="https://angel.co/transportation" target="_blank">these</a> are all of the startups in the Transportation sector, sorted by their Signal scores.

In the interest of openness, there are lots of caveats for this dataset:

- It's not clear if AngelList Signal is actually correlated with company quality (although it seems to be).
- Many companies don't report the technologies that they use.
- The lists of technologies that are self-reported are not necessarily exhaustive.
- etc.

Limitations aside, I calculated the number of startups with low, medium, and high Signal scores using each of ~75 different technologies, and this post summarizes the results. Whenever I refer to okay/good/great companies, the intended interpretation is companies with low/medium/high AngelList Signal scores.

(Note: you can click on each chart to see a higher resolution version.)

## Interpreting the Charts

In each chart, blue represents 'okay' startups, red represents 'good' startups, and orange represents 'great' startups. Within each color, the bars show relative frequencies of technology mentions. For example, let's say we're looking at technologies A and B. If 'okay' companies use B 3x as often as A, 'good' companies use A and B equally often, and 'great' companies use A twice as often as B, then the chart would look like this:

<center>
<a href="{{ site.url }}public/img/angellist-tech-example.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-example.png" alt="Example"></a>
</center>

(Note: the ratios of the lengths of blue/orange/red bars are 1:3, 1:1, and 2:1.)

## Programming Languages  

<center>
<a href="{{ site.url }}public/img/angellist-tech-prog-lang.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-prog-lang.png" alt="Programming Languages"></a>
</center>

Observations:

- For great companies, the most popular languages are Javascript, Ruby, Python, and Java.
- For okay companies, the most popular languages are Javascript, Ruby, PHP, and Java.
- The likelihood that PHP is being used is strongly anti-correlated with company quality.
- The better the company, the more likely it is to be using modern and/or functional programming languages (i.e. Go, Scala, Haskell, Erlang, Clojure).

## Front-end Tech

<center>
<a href="{{ site.url }}public/img/angellist-tech-front-end.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-front-end.png" alt="Front-end Tech"></a>
</center>

This chart shows a combination of web frameworks (Rails, Django), Javascript Libraries, and HTML/CSS.  

Observations:

- Ruby on Rails is super popular.
- HTML5 is dominating HTML.
- CSS is still dominating CSS3.
- The better the company, the less likely it is to use Bootstrap. 

## Databases/Storage/Caching

<center>
<a href="{{ site.url }}public/img/angellist-tech-db.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-db.png" alt="DBs"></a>
</center>

Observations:

- MySQL, Mongo, and Postgres dominate the database side.
- Redis is much more popular than memcached.
- The better the company, the less likely it is to build on top of Microsoft's products (SQL Server).

## Mobile

<center>
<a href="{{ site.url }}public/img/angellist-tech-android.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-android.png" alt="Mobile"></a>
</center>

Observations:

- Developing for iOS is slightly more popular than developing for Android
- The gap widens as company quality increases.
- Windows Mobile (which is not present in the chart) is 30x-50x less popular than iOS and Android among good/great companies.

## Infrastructure/Hosting

<center>
<a href="{{ site.url }}public/img/angellist-tech-infra.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-infra.png" alt="Infrastructure"></a>
</center>

Observations:

- AWS and Heroku dominate.
- The better the company, the more likely it is to use IaaS (e.g. AWS) instead of PaaS (e.g. Parse)
- The better the company, the less likely it is to build on top of Microsoft's products (Azure).

## DevOps Tools

<center>
<a href="{{ site.url }}public/img/angellist-tech-devops.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-devops.png" alt="DevOps"></a>
</center>

(Note: the sample size here was small because DevOps tools were rarely mentioned on AngelList profiles)

## Search

<center>
<a href="{{ site.url }}public/img/angellist-tech-search.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-search.png" alt="Search"></a>
</center>

Observations:

- Elasticsearch dominates this category.

## API Integrations

<center>
<a href="{{ site.url }}public/img/angellist-tech-api.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-api.png" alt="APIs"></a>
</center>

(Note: the sample size here was small because APIs were rarely mentioned on AngelList profiles -- especially for good/great companies.)

## Advanced Tech

<center>
<a href="{{ site.url }}public/img/angellist-tech-advanced.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-advanced.png" alt="Advanced Tech"></a>
</center>

Observations:

- I was surprised that there's no clear correlation between quality of company and usage of sophisticated technologies like machine learning or computer vision.

## Big Data Software

<center>
<a href="{{ site.url }}public/img/angellist-tech-big-data.png" target="_blank"><img src="{{ site.url }}public/img/angellist-tech-big-data.png" alt="Big Data"></a>
</center>

(Note: small sample size)