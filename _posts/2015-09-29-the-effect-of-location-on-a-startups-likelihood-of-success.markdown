---
layout: post
date: 2015-09-29 09:00:00
title: "The Effect of Location on a Startup's Likelihood of Success"
tags:
- "Data Analysis"
- "AngelList"
---
One of my friends is about to start a company, and he asked me if location matters. He lives in Mountain View and doesn't want to move north to SF, but he's not sure if staying south impedes his startup's chances of success.

Not having a good answer to the question, I decided to look at some data. Fortunately, <a href="http://angel.co/" target="_blank">AngelList</a> contains a fairly comprehensive list of startups around the world, as well as a Signal score for each startup. This score represents AngelList's estimate of a startup's quality based on the people involved (the founders, investors, advisors, et cetera). It's not a perfect metric for a startup's level of success, but it's not bad.

To answer my friend's question, I analyzed the composition of low vs. medium vs. high Signal startups for different metro areas and cities. What I found is that there are significant differences in startup qualities across different tech hubs, but that any city within a hub is about as good as any other.

## Caveats
This is not a very scientific analysis. Some of the flaws include: the Signal scores that AngelList provides are a black box; the list of startups on AngelList is not 100% comprehensive; some of the locations of startups might be wrong or out-of-date; I'm not a statistician; etc etc. The goal of this post is not to give a quantitative answer to where a startup should be based to maximize success, but rather to provide some qualitative thoughts with some light data behind them. It's not perfect, but it's better than nothing.

## Interpreting the charts
AngelList's Signal scores are between 0 and 10. In each of the charts below, the green elements represent the fractions of startups with high Signal scores (between 7 and 10), the orange elements represent startups with medium scores (between 2 and 7), and the red elements represent startups with low scores (between 0 and 2).

The right-most bar on each each is always the same -- it's the breakdown of high/medium/low scores across _all_ startups on AngelList. It's a reference point for comparing the cities and metros covered by each chart.

## Startup Quality by Metro Area
![Quality composition by metro]({{ site.url }}public/img/signal_metros.png)

If you look at the global averages on the right, only 1% of startups in the world have high Signal scores, 36% have medium scores, and 63% have low scores.

In contrast, most startup hubs consist of 5-15% high-scoring startups, 60-75% medium-scoring, and 20-25% low-scoring.

As you might expect, startup hubs are much more likely produce high-scoring startups. This makes sense, since a lot of top talent specifically moves to those hubs, and a lot of investors live in those hubs (and prefer to invest locally).

SF and Silicon Valley lead the pack in terms of high-scoring companies. In fact, 40% of all of the high-scoring companies in the world are in SF or SV.

## Startup Quality within Metros

### Silicon Valley

![Quality composition by metro]({{ site.url }}public/img/signal_sv_cities.png)

The two most interesting observations are:

1. Anywhere in the heart of Silicon Valley (the first four bars from the left) has approximately the same distribution of startup qualities.
2. As you move away from the core cities, average startup quality goes down. The decrease is more dramatic going south (Cupertino/San Jose) than going north (San Mateo/Burlingame). I suspect that when going north, you get away from Silicon Valley but end up approaching another strong hub (SF); when going south, you're just leaving the tech scene.

### East Bay

![Quality composition by metro]({{ site.url }}public/img/signal_east_bay_cities.png)

If you leave SF and go to the East Bay, the average quality decreases substantially. The percentage of startups with high Signal scores drops from 15-20% (in SF/Silicon Valley) to 5-10%.

There's a small tech hub in Oakland, and once you start going further out, like Fremont, the distribution of startup quality is probably closer to the global distribution than to the distribution in SF.
 
(Note, sample sizes for the East Bay were not very large.)

### Los Angeles

![Quality composition by metro]({{ site.url }}public/img/signal_LA_cities.png)

Los Angeles shows a similar pattern: Santa Monica (the tech epicenter of LA) has the strongest startups, then the distribution gets weaker as one travels further away.

### Washington DC

![Quality composition by metro]({{ site.url }}public/img/signal_dc_cities.png)

Washington DC and Baltimore are two nearby tech hubs with similar quality distributions. Cities between the hubs, like Rockville, Maryland, have a lower quality distribution.

### Seattle

![Quality composition by metro]({{ site.url }}public/img/signal_seattle_cities.png)

The last example is Seattle. While Seattle has many more startups than surrounding suburbs, the pattern of decreasing average quality with increasing distance is not as strong. This is probably because cities like Redmond and Kirkland house the offices of tech giants like Microsoft and Google.

## Summary
Taking the data and charts into account, as well AngelList's Signal score being an indicator of the quality of people involved in a company, three patterns emerge:

1. There are large differences in average startup quality among the top startup hubs, and even larger differences between startup hubs and the rest of the world.
2. Within a hub, it doesn't really matter what city you're in, as long as you're near the center of the hub.
3. As you get further and further away from a hub's center, average startup quality declines.

These observations make intuitive sense, too. Within a hub, there's a lot of talent and a lot investment dollars, and people are willing to commute 10 or 15 minutes for a good job or interesting investment opportunity. Being a couple of miles from the center is not a big deal. As you move further from these centers, there are fewer people willing to commute that far, fewer local investors, and more people who are actually commuting into hubs for more interesting opportunities. All of these factors make it harder to assemble a great team and to build a great company.

Finally, not being at the epicenter of a tech hub doesn't mean your company won't be amazing. It will just make it a little harder to attract top cofounders, top talent, and top investors. 
<br>
<br>
<br>
If you enjoyed this AngelList-based analysis, you might like the following articles:

- <a href="http://codingvc.com/which-technologies-do-startups-use-an-exploration-of-angellist-data" target="_blank">Which Technologies Do Startups Use? An Exploration of AngelList Data</a>
- <a href="http://codingvc.com/analyzing-angellist-job-postings-part-1-basic-stats" target="_blank">Analyzing AngelList Job Postings, Part 1: Basic Stats</a>
- <a href="http://codingvc.com/analyzing-angellist-job-postings-part-2-salary-and-equity-benchmarks" target="_blank">Analyzing AngelList Job Postings, Part 2: Salary and Equity Benchmarks</a>