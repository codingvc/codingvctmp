---
layout: post
date: 2015-06-29 08:00:00
title: "Bubbles and Unicorns"
---
![Unicorns]({{ site.url }}public/img/unicorns-and-bubbles.png)

<span style="font-size: 0.7em">(Image sources: <a href="http://zutheskunk.deviantart.com/art/MLP-Resource-Twilight-Sparkle-001-245173904" target="_blank">1</a>, <a href="https://pixabay.com/en/circle-ball-blue-bubble-3d-sphere-576797/" target="_blank">2</a>)</span>

Recently, there has been a lot of talk about a possible bubble in startup valuations. The question I want to explore is: "How are VC investment returns affected by bubbles?" That is, if it's a bubble, should VCs (and by extension, startups that need VC funding) close up shop for a few years and wait until market conditions change?

### Assertion #1: VC returns are governed by power laws

Most VC funds have somewhere between 15 and 50 portfolio companies. It turns out that almost all of a fund's returns will come from its best 1-3 investments. Here's a chart of outcomes for a typical individual investment:

![Angel investing returns]({{ site.url }}public/img/employee-options-angel-returns.png)

(Source: <a href="http://www.angelcapitalassociation.org/data/Documents/Resources/AngelGroupResarch/1d%20-%20Resources%20-%20Research/ACEF%20Angel%20Performance%20Project%2004.28.09.pdf" target="_blank">Returns to Angel Investors in Groups</a>)

Assigning some sample numbers, this chart suggestions that:

* 52% of investments might each return 0.2X (i.e. only 20% of the initial investment)
* 35% of investments might each return 1.5X
* 8% of investments might each return 6.5x
* 2% of investments might each return 15x
* 3% of investments might each return 40x

This distribution results in an expected multiple of 2.65X for the overall fund (pretty close to the 2.6X mentioned in the upper-right of the chart).

The noteworthy bit is that for a typical portfolio, 5% of the investments will be responsible for more than half of the total returns, and 13% of the investments will be responsible for more than 3/4 of the returns. This is what people mean when they say that VC returns follow the power law: the bulk of the returns are to be found in the outliers, not in the most common outcomes. If a fund invests in Twitter or Nest early on, the fund will be hugely successful; if none of the investments becomes a $1b+ company, then the fund will be mediocre at best. Trying to eke out an extra 1.5X or 6.5X exit is relatively meaningless when a 40x exit could return the entire fund. That's why investors and founders swing for the fences.

### Assertion #2: Investing in a power law distribution is only worthwhile if you might find an outlier.
A typical VC fund makes investments for 3-4 years, then holds onto those investments until every company in the portfolio either goes public, gets acquired, or fails. If outlier companies (i.e. the Twitters and the Nests) predictably occur in some years and not others, then it would be prudent to only invest in the good years. For example, if it turned out that 95% of all $5b+ companies were started during a recession, then making venture capital investments during economic booms would be unwise.

### Assertion #3: Great companies are founded every single year
I spent some time trying to dig up the most successful companies founded in each year since 1997 (the year that the Dot-com bubble began according to Wikipedia). The most notable companies that I found are listed below.

(Note: the list is not meant to be exhaustive.)

<style>
table#unicorns {border: 1px solid black; border-collapse: collapse;}
table#unicorns tr, table#unicorns th, table#unicorns td {border: 1px solid gray;}
table#unicorns td {padding: 5px;}
table#unicorns td.valuation {text-align: right}
</style>

<table id="unicorns">
    <tr>
        <th>Year</th>

        <th>Company</th>

        <th>Valuation**</th>
    </tr>

    <tr>
        <td rowspan="2">1997</td>

        <td>Priceline</td>

        <td class="valuation">$59b</td>
    </tr>

    <tr>
        <td>Netflix</td>

        <td class="valuation">$40b</td>
    </tr>

    <tr>
        <td rowspan="2">1998</td>

        <td>Google</td>

        <td class="valuation">$370b</td>
    </tr>

    <tr>
        <td>VMWare</td>

        <td class="valuation">$37b</td>
    </tr>

    <tr>
        <td rowspan="2">1999</td>

        <td>Salesforce</td>

        <td class="valuation">$47b</td>
    </tr>

    <tr>
        <td>Jawbone</td>

        <td class="valuation">$3.3b</td>
    </tr>

    <tr>
        <td rowspan="2">2000</td>

        <td>TripAdvisor</td>

        <td class="valuation">$13b</td>
    </tr>

    <tr>
        <td>Pandora</td>

        <td class="valuation">$3.4b</td>
    </tr>

    <tr>
        <td rowspan="3">2001</td>

        <td>Guidewire</td>

        <td class="valuation">$3.9b</td>
    </tr>

    <tr>
        <td>SuccessFactors</td>

        <td class="valuation">$3.4b</td>
    </tr>

    <tr>
        <td>Bloom Energy</td>

        <td class="valuation">$3b</td>
    </tr>

    <tr>
        <td rowspan="3">2002</td>

        <td>LinkedIn</td>

        <td class="valuation">$27b</td>
    </tr>

    <tr>
        <td>SpaceX</td>

        <td class="valuation">$12b</td>
    </tr>

    <tr>
        <td>GoPro</td>

        <td class="valuation">$7b</td>
    </tr>

    <tr>
        <td rowspan="3">2003</td>

        <td>Tesla</td>

        <td class="valuation">$34b</td>
    </tr>

    <tr>
        <td>Splunk</td>

        <td class="valuation">$9b</td>
    </tr>

    <tr>
        <td>Tableau</td>

        <td class="valuation">$8b</td>
    </tr>

    <tr>
        <td rowspan="2">2004</td>

        <td>Facebook</td>

        <td class="valuation">$247b</td>
    </tr>

    <tr>
        <td>Palantir</td>

        <td class="valuation">$20b</td>
    </tr>

    <tr>
        <td rowspan="2">2005</td>

        <td>Workday</td>

        <td class="valuation">$15b</td>
    </tr>

    <tr>
        <td>Palo Alto Networks</td>

        <td class="valuation">$15b</td>
    </tr>

    <tr>
        <td rowspan="2">2006</td>

        <td>Twitter</td>

        <td class="valuation">$23b</td>
    </tr>

    <tr>
        <td>Lending Club</td>

        <td class="valuation">$5.7b</td>
    </tr>

    <tr>
        <td rowspan="2">2007</td>

        <td>Dropbox</td>

        <td class="valuation">$10b</td>
    </tr>

    <tr>
        <td>Fitbit</td>

        <td class="valuation">$7b</td>
    </tr>

    <tr>
        <td rowspan="2">2008</td>

        <td>Airbnb</td>

        <td class="valuation">$25b</td>
    </tr>

    <tr>
        <td>Cloudera</td>

        <td class="valuation">$4.1b</td>
    </tr>

    <tr>
        <td rowspan="3">2009</td>

        <td>Uber</td>

        <td class="valuation">$41b</td>
    </tr>

    <tr>
        <td>WhatsApp</td>

        <td class="valuation">$19b</td>
    </tr>

    <tr>
        <td>Square</td>

        <td class="valuation">$6b</td>
    </tr>

    <tr>
        <td rowspan="3">2010</td>

        <td>Pinterest</td>

        <td class="valuation">$11b</td>
    </tr>

    <tr>
        <td>WeWork</td>

        <td class="valuation">$10b</td>
    </tr>

    <tr>
        <td>Nest</td>

        <td class="valuation">$3.2b</td>
    </tr>

    <tr>
        <td rowspan="2">2011</td>

        <td>Wish</td>

        <td class="valuation">$3b</td>
    </tr>

    <tr>
        <td>SoFi</td>

        <td class="valuation">$1.3b</td>
    </tr>

    <tr>
        <td rowspan="1">2012</td>

        <td>Instacart</td>

        <td class="valuation">$2b</td>
    </tr>

    <tr>
        <td rowspan="1">2013</td>

        <td>Zenefits</td>

        <td class="valuation">$4.5b</td>
    </tr>
</table>

### Observations and conclusions
The years when bubbles were bursting (2000-2002, 2008) were quite strong. So were the Dot-com bubble years (1997-1999) and the year before the real estate bubble popped (2007). Great companies are created every year. There's no clear pattern of which years produce at least one $10b+ company and which years do not. Actually, the pattern is that almost every year produces a $10b+ company!

Because VC returns follow a power law, it doesn't matter if there's a bubble or not, it only matters that there are at least one or two _huge_ companies created each year. Examples from the last two decades show that great companies are formed consistently, year after year, which means that even if we are near the peak of a bubble, founders should keep building companies and investors should keep investing in those companies.  
<br>
<br>
<span style="font-size: 0.7em">** Valuations are: 1) market caps for publicly traded companies, 2) reported valuations for privately held companies, and 3) acquisition prices for acquired companies. All numbers are as of June 2015.</span>