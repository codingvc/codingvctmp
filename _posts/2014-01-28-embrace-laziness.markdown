---
layout: post
date: 2014-01-28 05:00:00
title: "Embrace Laziness"
---

> "The dictionary is the only place that success comes before work. Work is the key to success, and hard work can help you accomplish anything."  
> <br>- Vince Lombardi

<div></div>
<br>
> "The problem with entrepreneurship is we are often working really hard producing high quality products that no-one wants."  
> <br>- Eric Ries

  

Hard work is necessary for a company to succeed, but it's not sufficient. The obvious, frustrating problem with hard work is that it can be misdirected. If you work hard on something that has no value, you're left frustrated, burnt out, and unsuccessful.  

Over the past decade, many companies have embraced the "minimum viable product" (MVP) philosophy. The basic idea behind MVPs is that startups have very limited time and resources, so they need to discover what customers want as quickly as possible. As a result, entrepreneurs should build the most basic features required to start getting feedback from customers, then use that feedback to guide subsequent development. This minimalist approach is very useful for product development, but it can also be applied to areas like <a href="{{site.url}}minimum-viable-everything" target="_blank">hiring and marketing</a>.

While MVPs encourage you to be lazy with adding features so that you can discover what you should be working on, it's often wise to be lazy even if you already know what you should work on. When I was at LinkedIn 10 years ago, one of our core challenges was how to determine whether two people were connected to each other. I had an insight about how to do this efficiently and ended up rewriting the existing algorithm so that it was almost 200x faster. Shortly thereafter, the product team decided to limit users' networks to 3 degrees instead of 4 degrees, and my speed-up was no longer necessary because the old algorithm was fast enough for 3 degrees. I had spent a lot of time thinking about how to improve performance with technology, but that turned out to be a waste of time because limiting network sizes was a much simpler, lazier approach.

As it turned out, transitioning to 3 degrees was also the superior solution because we found that users felt comfortable contacting people who were three degrees away, but not those who were four degrees away. In my personal experience, simple solutions often turn out to be the best solutions. A fun example of this is LinkedIn's invitation message template. LinkedIn used A/B testing heavily even in its early days, and the company ran numerous experiments with invitation messages (this was circa 2004). Back then, social networking was a brand new thing that most people didn't understand, so LinkedIn spent a lot of time fussing around with how to message and explain its value to people who were invited to the network by existing members. We tweaked and tuned a variety of single-page essays about the company, the value of social networking, and the benefits of connecting with colleagues. In the end, the template that had the highest invite acceptance rate was something like, "Hi, please join my LinkedIn network." To this day, if you try to invite someone through LinkedIn's website, the default text is very short.

Two more great opportunities for being lazy are when you're creating a product that your customers have never had access to before, or when you're not sure about the scope of a problem. If you start with something simple, your solution might end up being 'good enough' for a long time. Last year, I met a founder whose situation exemplified this point. Jeff (not his real name) led a startup that provided administrative tools for conference managers. Jeff told me that his customers' existing tools didn't offer any data about conference attendees, so he planned to hire a developer to write reporting software with fancy charts and dashboards. Eventually, Jeff realized that just offering a very basic analytics product was enough for his customers because, while bare-bones, it was so much better than what they were used to. The basic version took several weeks of an engineer's time and obviated the need to hire an additional employee.

The calculus of laziness is simple: if you can produce a basic solution in 5 hours or an advanced solution in 200 hours, and if the basic solution will be good enough 20% of the time, then always try the basic solution first. Even if the 5 hours is completely wasted 80% of the time, you'll still come out ahead in the long run. (20% * 5 hours + 80% * 205 hours = 165 hours per task, which is much better than if you always tried the 200-hour approach first.)  

Next time you're faced with a problem, forget being clever. Figure out the simplest thing you can try and then try it. If you need to track sales leads, start with an Excel spreadsheet instead of spending weeks test driving CRM software. If you need to fill in missing data in a dataset, try Bayes' Rule or Google Predict instead of training your own neural network. If your customers need dashboards, build something basic yourself (or use <a href="https://keen.io/" target="_blank">keen.io</a>) before hiring a Director of Analytics. You may eventually find that you need to buy CRM software or implement a neural network or hire an analytics expert, but there's a good chance that you won't.

In short, embrace laziness.  

<center>
![Sleeping Kitten]({{ site.url }}public/img/embrace-laziness-kitten.jpg)
Photo credit: http://www.flickr.com/photos/mistyanddavid
</center>