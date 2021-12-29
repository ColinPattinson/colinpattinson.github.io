---
layout: post
title:  "Tracking Sustainability of Menu Pages"
date:   2021-12-29
excerpt: "Check-up of Nando's menu pages and their sustainability credentials"
tag: [Nandos]
comments: false
---
Once upon a time a few of us [revamped the online menus for Nando’s](https://medium.com/nandos-product-and-engineering/weve-recently-launched-a-new-menu-available-on-beta-nandos-co-uk-377f2ee762bc). We prioritised performance as a key metric and made some real progress. 

As a bit of an update, I’ve been experimenting with a tool. This time to track the sustainability of our pages. Here is my report on how we are doing…

# Context
Some things to know before we jump in;
- I have some skin in the game [for caring about this topic even before Nando’s days](https://colinpattinson.github.io/tags/#Climate). Did some stuff around making the NHS tech more sustainable with smart colleagues
- one of Nando’s internal [measures of success is essentially to make Nando’s more sustainable](https://www.nandos.co.uk/carbonneutral). Lots is being done and honestly, it’s super commendable. Absolutely leading the pack in the industry and lots of effort put in from colleagues. 

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Totally neutral, totally Nando’s. 🌎🌶<br><br>We are carbon neutral across our scope 1, 2 and 3 emissions, the first step on the way to our ultimate goal of becoming Net Zero by 2030. <br><br>We have made a good start on the journey to cut our own emissions and are also taking (1/4) <a href="https://t.co/piEXjQI62J">pic.twitter.com/piEXjQI62J</a></p>&mdash; Nando&#39;s (@NandosUK) <a href="https://twitter.com/NandosUK/status/1455531082053558276?ref_src=twsrc%5Etfw">November 2, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

- Performance of pages is 100% tied in with making them more sustainable (e.g. less page weight, means less to transfer) so I was hoping that we’d score alright given previous efforts (see above).
- menus have a fair amount going on… namely images of food can clog up performance. We did our best to make the pages/inc images as performant as possible
- I saw this tool on twitter. I fully appreciate that how things are measured and how accurate they are is in contention. I do not dare wade into that. I will take this solely as a proxy.

## Tool used.
I used the free version of [EcoPing](https://ecoping.earth/). It was very easy to set up. I did not pay for any extras. Straight up free version. You could in theory stick any site down if you wanted to measure a competitor. It appears to use [Lighthouse as a means to measure certain stats](https://developers.google.com/web/tools/lighthouse). 

I am conscious that continuously measuring the site's performance is in effect adding to our carbon footprint too. Not sure I can get around that. I suspect EcoPing is less of a hog than… say… Google Analytics. 

# What did we find?
Mostly good news…

## EcoScore
A score given out of 100. First test we scored an 86 but the average over the past week has shot up to 94. The tool tells me... 
> Over 90 is the goal! 

So check. For [comparison](https://ecoping.earth/indexes/popular-websites), Amazon (similarly an ecommerce site) scored a 72 when I wrote this.

## CO2 Grams
According to EcoPing…
> the average website creates 1.76 grams per page view

Our menu page clocked in at 0.29 grams. Which is canny.

Out of interest I looked at a comparison. [Humans apparently](https://www.sciencefocus.com/planet-earth/how-much-does-human-breathing-contribute-to-climate-change/)…
> In one day, the average person breathes out around 500 litres of the greenhouse gas CO2 – which amounts to around 1kg in mass. 

So, let's see…  if we had a million page views then we equate to about 29 days of one person breathing in and out.

## Transfer Size
After digging around this is sorta total page weight (“compressed size of all resources on the page”). We flirt most with missing a target here. The goal is under 1.96MB and we hit 1.89MB. Interestingly a big chunk is not images but our font.

Google homepage is a nice and lean [182 KB but something like the Guardian is a chunky 2.56 MB](https://ecoping.earth/indexes/popular-websites). 

##  Load time
We know this also affects everything from user experience to SEO so something we knew to improve. Thankfully it remains very healthy. Target is under 3 seconds and we scored 2.00 seconds on the dot on average.

Reddit apparently clocks in at [5.7 seconds load time according to EcoPing](https://ecoping.earth/indexes/popular-websites). BBC with a decent 1.6 seconds.

## Total CO2
Projected total CO2 per year would be 34.8kg based on 10,000 monthly visitors.

## Trees
To account for those total emissions we’d need to plant apparently 1.58 trees this year. I have visual evidence of colleagues planting trees this year so we might have already topped the 1.58 figure by now.

## Hosting
The reports also try figure out how low-carbon your hosting is. They say…
> see how "green" your web hosting is. Each report is integrated with live grid data so, we can see where in the world your resources come from and what the energy production is like in those areas.

As I type we are getting a 76% low carbon score. The worst culprits to drag the average down are third-parties. Mostly analytics related.

## Comparisons
The service has [a few ways to compare](https://ecoping.earth/indexes). I was mostly looking at the most popular list for this mini experiment.

# Suggested actions to improve
Overall the page scored pretty well according to EcoPing. We’d invested time in making it performant so that is a relief. It does however give some suggestions (that look generic to lighthouse suggestions to my eyes).

They include;
- Reduce unused JavaScript (a classic)
- Sort out the font

 I shall enquire about fonts.

# Overall Review
For a little check-up, the tool is pretty good. Easy to use and clear. Would recommend as long as comfortable with it being solely a proxy measure. 
