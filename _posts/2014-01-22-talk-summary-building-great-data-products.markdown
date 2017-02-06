---
layout: post
date: 2014-01-22 05:00:00
title: "Talk Summary: Building Great Data Products"
tags:
- "Notes"
- "Talk Notes"
---

Yesterday I went to a great talk by <a href="https://twitter.com/dpatil" target="_blank">DJ Patil</a> called "Building Great Data Products." DJ has an impressive background in building data-centric products: he was head of LinkedIn's data products for several years, then Data Scientist in Residence at <a href="http://www.greylock.com/" target="_blank">Greylock</a>, and is now the VP of Product at <a href="https://www.relateiq.com/" target="_blank">RelateIQ</a>, a CRM tool whose homepage reads, "The Beginning of Data Science in Decision Making." He also co-coined the term _Data Scientist_.

DJ discussed some of the lessons he learned while building products at LinkedIn and RelateIQ, and the following is a summary of my notes from the talk:

- **Don't try to be too clever**. Simple, straightforward approaches beat cleverness 9 times out of 10.
- **Start with something simple, then make it more complex if necessary**. Don't start with something complex and then simplify.
- **The hardest part of data science is getting good, clean data**. Cleaning data is often 80% of the work.
- **Try to get clean data from the front end (i.e. the user) instead of cleaning it on the backend**. For example, if you're trying to figure out what company someone works for, it's easier to guide them with auto-complete or "did you mean &#95;&#95;&#95;&#95;?" suggestions, rather than accepting whatever they type and trying to understand it later. You'd be surprised at <a href="https://web.archive.org/web/20080731042402/http://www.google.com/jobs/britney.html" target="_blank">the number of ways</a> in which people can input the same thing if you don't give them any guidance.
- **Use humans in general and <a href="https://www.mturk.com/mturk/" target="_blank">Mechanical Turk</a> specifically for early versions of your product**, then try to automate and streamline as desired.
- **Build easy products first.** For example, start with collaborative filtering before diving into fully personalized recommendations.
- **Showing users their own data via charts, blog posts, etc. is a great way to engage them.**
- **When showing data, think about 1) what you want the viewer to take away, 2) what actions you want them to take, 3) and how you want them to feel.** UX is very important. Don't overload people with too much information or creep them out with inappropriate details.
- **Set user expectations low**. If you set high expectations and screw up, it's very hard to regain a user's trust. For example, if you tell someone, "We know you will love XYZ!" and they don't like XYZ, they'll be skeptical of your future recommendations -- or even ignore them. If you reframe as, "Are you interested in XYZ? No? Okay, sorry!" then users will be more forgiving.
- Unfortunately, **the best way to test data products is in production**. It's the only way to find out if your recommendations are effective and to learn about all of the warts and corner cases that lead to embarrassing mistakes. For example, how do you tell if your product suggestions are good? Show them to users and measure the effect that they have on spending/engagement/whatever you're hoping to improve.
- Simple beats clever 9 times out of 10, but **you need to be able to recognize when to build something sophisticated**.
- **Try to augment humans and make them more efficient instead of trying to replace them**. People generally dislike feeling unnecessary or replaceable.
- **Minimize the friction in your product. **If you're asking users to answer questions or input data, make that as easy and painless as possible -- otherwise users won't do it. Nobody reads manuals and instructions anymore. Strive to make products that are as intuitive as the iPad or Angry Birds.
- **Rule of thumb: every time you ask for data, your conversion funnel takes a 10% hit.** Try to keep all questions lightweight and easy to answer so that you can minimize the damage.

DJ's talk was great and I can vouch for many of these lessons personally based on my work at Google and <a href="http://www.factual.com/" target="_blank">Factual</a>. I think the most valuable lesson that I've learned over the last decade is one that came up repeatedly during the talk: simple approaches are often surprisingly effective. For example, I remember one task where I had a sparse dataset and had to fill out as much of the missing data as possible. Instead of using fancy algorithms and sophisticated machine learning, I tried the following heuristic: for every pair of columns, if a value, X, in one column was associated with a value, Y, in another column almost all of the time, then every time the first column value was X and the second column value was missing, I'd set the second column value to Y. It was a very naive approach, and yet it managed to fill in a large chunk of my dataset. I've now used this heuristic for data about books, movies, places of interest, and other datasets, and it often makes more clever strategies unnecessary or not worth the time.

Another important lesson that I've learned is that it's a great idea to work with small samples of data and use a single machine for as long as possible. Hadoop and distributed systems are nice when you're running in production on terabytes of data, but they greatly diminish your development speed and ability to experiment. You'll probably make progress much more rapidly if you just load a 500MB slice of data into RAM and experiment on your laptop.

After DJ's talk, I started thinking about the many blog posts that I've seen that focus on technologies that are commonly used for working with data: Hadoop, scipy, regular expressions, etc. I'd love to see more blog posts (and books) about higher level strategies and tactics for building data products. Posts that offer suggestions like "work with small samples"; "leverage Mechanical Turk"; and "start with the simplest approaches." I might turn a few of these topics into future blog posts, but I'm sure there are many lessons that I haven't learned yet. If you know of any great resources for creating data products, please let me know on <a href="https://twitter.com/lpolovets" target="_blank">Twitter</a>!