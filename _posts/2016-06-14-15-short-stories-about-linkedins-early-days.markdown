---
layout: post
title: "15 Short Stories About LinkedIn's Early Days"
date: 2016-06-14 05:24:00
---
I was lucky enough to be one of LinkedIn's earliest employees in 2003. I joined the company when it was just over a dozen people and was the 2nd non-founding engineer hire.

![LinkedIn's team at 2 million members]({{ site.url }}public/img/2million.jpg)
<center>_Team photo from 2005, when we reached 2,000,000 users_</center>

Yesterday, I woke up to the news that Microsoft is acquiring LinkedIn for $26b in cash. It was a surreal story to read because when I left Microsoft to join LinkedIn in 2003, I never imagined that one day that tiny startup would be acquired for almost 7% of Microsoft's market cap.

The acquisition announcement got me reminiscing about LinkedIn's early days, so I thought I'd share some of my favorite memories from my two years at the company (2003-2005).

Obligatory caveat: I'm not affiliated with LinkedIn in any way at this point. I don't own any LinkedIn stock. Some of the small details might be a little off since the events described happened over a decade ago.

# Money

## 1. Series A

I wasn't involved in LinkedIn's fundraising, but felt firsthand just how long the Series A took. I received an unofficial employment offer in December 2002, during my senior year of college. The offer was conditional on LinkedIn raising their Series A, which was expected to take a few weeks. A few weeks turned into a month, and then several months, and I ended up having to accept an expiring job offer from Microsoft.

I started at Microsoft in July of 2003, and I ended up on a miserable project: legacy maintenance for a 15-year-old product. I was deciding whether to switch jobs when I got a call from someone at LinkedIn in October 2003. They had finally raised their Series A -- _10 months after my initial interview_ -- and wanted to know if any of my college classmates were looking for work. I was unhappy at Microsoft, so I volunteered myself. I started at LinkedIn two weeks later. (If you're interested, the full story of how I got my job at LinkedIn can be found <a href="https://www.quora.com/How-did-you-get-your-job-at-LinkedIn-product/answer/Leo-Polovets?share=1" target="_blank">here</a>.)

To this day, I'm surprised that it took LinkedIn so long to raise their first institutional round despite having had a very strong CEO and a live, growing product in the market.

## 2. Office Space
We were frugal in the early days, so we moved offices every year to get a good deal. One year we had an office in East Palo Alto that was cheap, but very remotely located. The only decent restaurant nearby was a cafe at the Palo Alto Airport, so LinkedIn's engineering team walked over and ate lunch at an airport almost daily for an entire year. 

## 3. Initial monetization strategy

From the beginning, users could get introductions to other LinkedIn members who were in their 2nd, 3rd, or 4th degree networks. The original monetization plan was to wait until we had a few hundred connection requests per day, and then we'd try charging something like $5 for each request. However, as the number of daily requests reached and surpassed that target, we kept delaying monetization because we didn't want to add friction to site usage. In the end, we never used the per-request model. Instead, LinkedIn rolled out paid job postings, ads, and premium memberships in 2004-2005 and became one of the few internet companies that has several significant revenue streams.

## 4. Challenges with selling job postings

When we launched job listings in ~2005, they ended up being surprisingly hard to sell. The problem was that LinkedIn only had 1m or 2m users worldwide, so there wasn't enough applicant density for most jobs. "Oh, you're looking for a software engineer in Portland? Well, LinkedIn has 2 engineers in the Portland area and 7 more in the rest of Oregon. Do you want to pay for a job listing to target those 9 people??" At one point, the sales team offered generous job listing packages to some large tech companies because we didn't want our job directory to look empty. (e.g. $1000 for 50 job postings.)

# Product features

## 5. A/B testing
LinkedIn was ahead of its time when it came to being data-driven. I remember having to implement A/B testing for some feature back in ~2004. I had never heard of A/B testing, so I asked Josh Elman* to explain it to me. His explanation piqued my interest even further, so I tried to look up A/B testing on Wikipedia. However, A/B testing wasn't yet mainstream enough to have a Wikipedia entry, and it wouldn't be until 2007.

&nbsp;* <a href="https://www.linkedin.com/in/joshe" target="_blank">Josh</a> was the first product management hire at Linkedin. He eventually became a partner at Greylock, but not before being an early employee at LinkedIn, Facebook, _and_ Twitter.

## 6. A/B testing invitation messages
Speaking of A/B testing, one of the ongoing debates in the early years was how to message the product to new users. Social networking was a very new concept in the early 2000s, and most people's first exposure to LinkedIn was an invitation email from an existing member. The key question was: what should that invitation say? We tried a number of alternatives:

- A paragraph explaining social networking and another paragraph explaining LinkedIn.
- A few paragraphs on the benefits of joining LinkedIn.
- A few paragraphs explaining that a LinkedIn invitation was special because it meant that the inviter trusted and respected the invitee and wanted to stay in touch professionally. 
- A tiny blurb along the lines of "I'd like to add you to LinkedIn network."

Surprisingly, despite most people being unfamiliar with social networking and LinkedIn, the last alternative handily beat all of the others. It was a good lesson in looking at data instead of trusting your gut when it comes to understanding users.

## 7. Engineer optimization vs. PM optimization
Whenever you tried to view another user's profile, LinkedIn would check how many degrees separated you from that user. We'd map out your entire 4-degree network, and if the user was in it we'd show you how you two were connected. If they were not in your network, we'd tell you that you didn't have permission to view their profile. The problem was that some highly-connected LinkedIn members had very large networks, and so there would be a long lag whenever they tried to view profiles. These lookups also hogged more and more of our servers' resources.

I eventually came up with an algorithm that made these lookups up to 200x faster. I was _so_ proud of that algorithm. A few weeks later, the product team decided that people who were 4-degrees away were too distant, and that the site should limit browsing to 3-degrees or less. My optimization immediately became superfluous. At the time I was bummed, but it was absolutely the right product decision, and a great lesson about optimizing at the right level.

## 8. Product vision
On the product side, Reid Hoffman had an incredible knack for seeing into the future. I remember one company pep talk in 2004 or 2005 where Reid talked about his goal of LinkedIn becoming Resume 2.0. He believed that one day, people would send each other LinkedIn profile links instead of resumes. It seemed like a crazy prediction at the time, and yet here we are.

## 9. Product detail
When I started at the company in late 2003, I wanted to make a good impression on everyone. It was the pre-smartphone era, so I carried around a small Olympus voice recorder and saved every interesting product idea I could think of. After a few weeks, I approached <a href="https://www.linkedin.com/in/ablue" target="_blank">Allen Blue</a>, who was one of LinkedIn's cofounders and its VP of Product, and asked him if he'd humor me and my list of ideas sometime. He kindly agreed, and a few days later I proceeded to go through 50 or 60 feature proposals with him.

That meeting turned out to be an unforgettable experience because Allen had previously considered _literally_ every idea that I proposed, and he patiently explained which ideas were unlikely to work, which ones were planned for the near term, and which ones might be incorporated in the longer term. I was very impressed with the level of thinking and thoroughness that Allen had applied to the product roadmap. In fact, now that I'm a VC I've turned this into a due diligence test: sometimes I will suggest a few not-completely-obvious product ideas to a founder just to see if they've considered them before.

# Market size and M&A
## 10. How big can this get? -- Part 1
During my engineering interview in 2002, I had a chance to chat with Reid for half an hour. I asked him how big he thought LinkedIn could become, and he said he foresaw every white collar worker in the world being on the site, which could be 250m-300m people. I tried not to laugh out loud. Not only did social networking not exist yet, but even Yahoo!, which was probably the biggest website in the world at the time, didn't have that many users. 300m members seemed ludicrously optimistic, and yet turned out to be another example of Reid's prescience. Today, LinkedIn has over 400m members. (As an aside, it's interesting to watch Yahoo get offers for a fraction of LinkedIn's acquisition price -- yet another thing that I never would have believed in 2002.)

## 11. How big can this get? -- Part 2
In 2007 or 2008, early employees had a chance to sell some of their vested stock back to the company. I remember consulting with some of my alumni friends and deciding as a group that the company still had 3x or 5x upside. That upside eventually turned out to be closer to 100x.
 
When the company IPO'ed in 2011, many early employees -- including myself -- sold their stock as quickly as possible, fearing that the company's valuation was unsustainably rich. The stock price ended up appreciating an additional 3x-4x in the following years.

All of this taught me a sobering lesson: even if one of your investments goes up by 100x, there's a good chance you'll end up with 5x or 12x or 34x instead of 100x, because it's very hard to anticipate whether the investment has hit a peak or whether it's about to grow even more. At some point, fear about the potential downside begins to outweigh greed for the potential upside.

## 12. Will Monster acquire LinkedIn?

In the early days, I remember reading a news article where some Monster.com exec (maybe even the CEO) was asked if Monster might acquire LinkedIn someday. Monster was the big player in the online recruiting market at that time, and the exec's response was that LinkedIn wasn't worth acquiring at the time, but that if it did prove out its value it would probably be too expensive for Monster to buy. That turned out to be an insightful prediction, as today LinkedIn is approximately 100x the size of Monster.

# Technical details

## 13. The first recommendation server
LinkedIn was built before cloud computing was a thing. Many of the early recommendation services started as experiments that were running off of a desktop under the desk of the sole data scientist. When the experiments eventually turned into full-fledged features, that lonely desktop continued to generate most of the recommendations that were uploaded to production. The fragility of that set-up was simultaneously funny and terrifying.

## 14. Living on the edge
We stored the graph of all member connections in RAM so that we could very quickly determine whether any two members were in each other's networks. The problem was that we were always approaching the limits of how much RAM was available. We had servers with 8GB of RAM, and the graph database took up 5GB... then 6GB... then 7GB... and then we'd get very nervous. Just in the nick of time, 16GB servers came out and we were saved for a few months. Then the graph started to approach 16GB, we got nervous again, and were again saved by a higher capacity server model. I still remember rewriting some core Java data structures like BitSets and HashSets -- structures that programmers should never have to rewrite -- in order to get get an extra 5-10% memory savings.

## 15. Super-connectors
When LinkedIn launched, every person's profile would show how many connections they had. For some reason, a small group of users decided to compete for who had the most connections. A few even updated their profile headlines to say things like, "Bob Smith, #4 most connected user with 18,000 connections." This put a surprising amount of strain on our servers because some parts of the site had to do a tiny computation for every connection that a user had, and 18,000 connections multiplied by even a few milliseconds meant that pages would take minutes to load.

On the engineering side, we started creating fake "super-connector" profiles internally so that we could performance test every page on our site with a lot of data. On the product side, we stopped showing the exact number of connections people had and instead showed "500+" as soon as a user exceeded five hundred connections. That minor UI tweak decreased the incentive for higher connection counts, and it remains on the site to this day.

People say that "what gets measured gets improved," but super-connectors taught me that "what gets measured publicly gets gamed."

<br>
<hr>
<br>
The more I work with companies, the more I see how easy it is to be blinded by their eventual success. Once a company is huge, people often forget that there was a time when it was dinky or struggling or even on the verge of failure. I hope these stories give a little bit of a sense of what LinkedIn was like when it was fifteen people instead of ten thousand. 