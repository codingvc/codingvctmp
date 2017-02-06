---
layout: post
date: 2014-09-08 17:16:00
title: "Analyzing AngelList Job Postings, Part 1: Basic Stats"
tags:
- "Data Analysis"
- "AngelList"
---
<style>
  tr, th, td {
    text-align:left;
    border-bottom: 1px dotted gray;
  }
  th {
    border-top: 1px dotted gray;
  }  
  td, th {
      width: 50%;
  }
  table {
      margin-bottom:1em;
      border-collape: collapse;
      width: 100%;
  }
</style>
Last month, I used AngelList data to analyze <a href="{{site.url}}which-technologies-do-startups-use-an-exploration-of-angellist-data" target="_blank">the technologies that startups use</a>. After getting positive feedback on my analysis, I decided to dig into more AngelList data -- this time looking at job postings.  There is a lot of job posting data available via API, and <a href="https://twitter.com/joshuaxls" target="_blank">Joshua Slayton</a> from AngelList was kind enough to send me some additional data that is not available via API.  

This series will consist of two separate blog posts:

Part 1: Basic stats about popular startup locations, job titles, vesting schedules, etc. [Full disclosure: this is the least interesting/actionable post in the series]

Part 2: <a href="{{site.url}}analyzing-angellist-job-postings-part-2-salary-and-equity-benchmarks" target="_blank">Salary and equity benchmarks. By role, company size, etc</a>.

### Preliminaries

I took a snapshot of all jobs on AngelList on August 31st, 2014. There were 12610 jobs posted at the time.

Please note that this is an analysis of companies found on AngelList, which creates some expected biases. For example, the data will be biased toward earlier stage startups, and away from startups in non-English-speaking countries.

### Job Locations

**Top 20 cities**
<table>
<tr><th>City</th><th># of open jobs</th></tr>

<tr><td>San Francisco</td><td>2766</td></tr>

<tr><td>New York City</td><td>1676</td></tr>

<tr><td>Los Angeles</td><td>485</td></tr>

<tr><td>London</td><td>444</td></tr>

<tr><td>Boston</td><td>309</td></tr>

<tr><td>Palo Alto</td><td>300</td></tr>

<tr><td>Bangalore</td><td>263</td></tr>

<tr><td>Washington, DC</td><td>230</td></tr>

<tr><td>Toronto</td><td>226</td></tr>

<tr><td>Chicago</td><td>218</td></tr>

<tr><td>Mountain View</td><td>216</td></tr>

<tr><td>Seattle</td><td>201</td></tr>

<tr><td>Silicon Valley</td><td>186</td></tr>

<tr><td>New Delhi</td><td>185</td></tr>

<tr><td>Austin</td><td>161</td></tr>

<tr><td>Mumbai</td><td>153</td></tr>

<tr><td>Berlin</td><td>130</td></tr>

<tr><td>Vancouver</td><td>120</td></tr>

<tr><td>Santa Monica</td><td>117</td></tr>

<tr><td>Singapore</td><td>107</td></tr>
</table>

Next, I removed all cities that had 3 or fewer jobs (about 5% of all jobs) and categorized the remaining cities into geographic areas.

**Jobs in each major geographic area**

<table>
<tr><th>Geographic Area</th><th># of open jobs</th></tr>

<tr><td>Silicon Valley</td><td>4130</td></tr>

<tr><td>US (minus Silicon Valley, NY, SoCal)</td><td>2282</td></tr>

<tr><td>New York</td><td>1723</td></tr>

<tr><td>India</td><td>839</td></tr>

<tr><td>Southern California</td><td>801</td></tr>

<tr><td>Continental Europe</td><td>649</td></tr>

<tr><td>Canada</td><td>503</td></tr>

<tr><td>UK</td><td>493</td></tr>

<tr><td>Asia</td><td>238</td></tr>

<tr><td>Central/South America</td><td>91</td></tr>

<tr><td>Australia</td><td>78</td></tr>

<tr><td>Israel</td><td>54</td></tr>

<tr><td>Russia</td><td>46</td></tr>

</table>

Notable observations: SF, LA, and NYC make up almost 50% of all jobs on AngelList. Within Silicon Valley, 2/3 of all jobs are in SF and 1/3 are in Mountain View/Palo Alto/etc.

### Openings per company

<table>
<tr><th># of openings at startup</th><th># of startups</th></tr>

<tr><td>1 opening</td><td>3123</td></tr>

<tr><td>2 openings</td><td>1238</td></tr>

<tr><td>3 openings</td><td>689</td></tr>

<tr><td>4 openings</td><td>349</td></tr>

<tr><td>5 openings</td><td>215</td></tr>

<tr><td>6 openings</td><td>115</td></tr>

<tr><td>7 openings</td><td>78</td></tr>

<tr><td>8 openings</td><td>47</td></tr>

<tr><td>9 openings</td><td>30</td></tr>

<tr><td>10 openings</td><td>26</td></tr>

<tr><td>11 openings</td><td>10</td></tr>

<tr><td>12 openings</td><td>5</td></tr>

<tr><td>13 openings</td><td>7</td></tr>

<tr><td>14 openings</td><td>3</td></tr>

<tr><td>15 openings</td><td>1</td></tr>

<tr><td>17 openings</td><td>3</td></tr>

<tr><td>19 openings</td><td>3</td></tr>

<tr><td>23 openings</td><td>1</td></tr>

<tr><td>25 openings</td><td>1</td></tr>
</table>

Notable observations: About 60% of openings are at companies that list &lt;=3 jobs, 35% are at companies that list 4-10 jobs, and the last 5% are at a handful of companies that have 11 or more open positions.

### Job Opening Types

<table>
<tr><th>Type</th><th># of open jobs</th></tr>

<tr><td>Full-time</td><td>9740</td></tr>

<tr><td>Cofounder</td><td>1080</td></tr>

<tr><td>Internship</td><td>997</td></tr>

<tr><td>Contract</td><td>936</td></tr>
</table>

### Equity Vesting

**Most common vesting periods**  

<table>
<tr><th>Vesting period</th><th># of open jobs</th></tr>

<tr><td>4 years</td><td>11096</td></tr>

<tr><td>3 years</td><td>526</td></tr>

<tr><td>0 years</td><td>355</td></tr>

<tr><td>2 years</td><td>269</td></tr>

<tr><td>5 years</td><td>182</td></tr>
</table>

**Most common vesting cliffs**

<table>
<tr><th>Vesting cliff</th><th># of open jobs</th></tr>
<tr><td>1.0 years</td><td>11875</td></tr>

<tr><td>0.0 years</td><td>403</td></tr>

<tr><td>0.5 years</td><td>135</td></tr>
</table>

Notable observations: <a href="http://startuplawyer.com/incorporation/what-is-four-years-with-a-one-year-cliff" target="_blank">4 year vesting with a 1 year cliff</a> is by far the most common equity vesting set-up.

### Job Functions

<table>
<tr><th>Role</th><th># of open jobs</th></tr>

<tr><td>Developer</td><td>6486</td></tr>

<tr><td>Marketing</td><td>1795</td></tr>

<tr><td>Designer</td><td>1656</td></tr>

<tr><td>Sales</td><td>1601</td></tr>

<tr><td>Mobile Developer</td><td>1434</td></tr>

<tr><td>Operations</td><td>818</td></tr>

<tr><td>Product Manager</td><td>810</td></tr>

<tr><td>Hardware Engineer</td><td>288</td></tr>

<tr><td>Finance</td><td>227</td></tr>

<tr><td>Office Manager</td><td>157</td></tr>

<tr><td>Human Resources</td><td>143</td></tr>

<tr><td>Attorney</td><td>39</td></tr>
</table>

(The counts in the second column add up to a little more than 12610 because some jobs were tagged with multiple roles.)

### In-demand Skills

**Skills mentioned in at least 500 job openings:**

<table>
<tr><th>Skill</th><th># of open jobs</th></tr>
<tr><td>Javascript</td><td>2372</td></tr>

<tr><td>Python</td><td>1341</td></tr>

<tr><td>Ruby on Rails</td><td>1211</td></tr>

<tr><td>HTML</td><td>1131</td></tr>

<tr><td>Sales and Marketing</td><td>1089</td></tr>

<tr><td>iOS Development</td><td>1069</td></tr>

<tr><td>jQuery</td><td>1016</td></tr>

<tr><td>CSS</td><td>1001</td></tr>

<tr><td>Java</td><td>991</td></tr>

<tr><td>HTML5 & CSS3</td><td>952</td></tr>

<tr><td>Android</td><td>852</td></tr>

<tr><td>User Experience Design</td><td>816</td></tr>

<tr><td>PHP</td><td>777</td></tr>

<tr><td>Business Development</td><td>769</td></tr>

<tr><td>MySQL</td><td>690</td></tr>

<tr><td>Node.js</td><td>644</td></tr>

<tr><td>Social Media Marketing</td><td>604</td></tr>

<tr><td>MongoDB</td><td>509</td></tr>

<tr><td>Amazon Web Services</td><td>503</td></tr>
</table>  

<br>
**Skills mentioned in 250-499 openings:** Angular.JS, Objective C, Sales, UI/UX Design, HTML/CSS/PHP/MYSQL, Product Development, Ruby, Mobile Application Design, Mobile Development, User Interface Design, SQL, Backbone.js, Django, PostgreSQL, Linux, Git, APIs, Sales Strategy and Management, Product Marketing, Mobile, Data Analysis, RESTful Services, and Social Media.

**Skills mentioned in 100-249 openings:** Big Data, Graphic Design, Hadoop, Adobe Photoshop, Web Design, Web Development, Redis, C++, Mobile Application Development, Photoshop, Product Management, Machine Learning, Software Engineering, SEO/SEM, iOS, REST APIs, Customer Service, noSQL, Twitter Bootstrap, Front-End Development, C, Databases, SaaS, AngularJS, JSON, Business Operations, C#, Growth Hacking, Marketing, Scala, Analytics & Reporting, Adobe Illustrator, Online Marketing, AJAX, Communication Skills, Project Management, E-Commerce, Customer Relationship Management, Full-Stack Web Development, Web Analytics, Sales/Marketing and Strategic Partnerships, Coffeescript, Business Strategy, Account Management, Community Management, Content Marketing, Writing, Backend Development, Amazon EC2, Advertising, .NET, Visual Design, Agile Software Develoment, Software Development, Google Analytics, Adobe Creative Suite, Heroku, and Algorithms.