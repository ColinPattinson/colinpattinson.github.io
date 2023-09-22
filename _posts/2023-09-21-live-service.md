---
layout: post
title:  "Managing a Live service"
date:   2023-09-21
excerpt: "Hints & tips about the live phase"
tag: [Kry]
comments: false
---
I’ve been asked to give a little talk about managing a live service. What follows is a list of thoughts, tips, tricks & activities that spring to mind that would help a product manager & team who are responsible for a service out in the wild. Needless to say it’s a slightly different mindset then being in [discovery](https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works), [alpha](https://www.gov.uk/service-manual/agile-delivery/how-the-alpha-phase-works) or even private [beta](https://www.gov.uk/service-manual/agile-delivery/how-the-beta-phase-works).

# What do I mean by a live service
Just for clarity’s sake. Broadly, I subscribe to the notion that a service is [“something that helps someone to do something”](https://good.services/blog/what-is-a-service). For example, this could be applying for a new passport or booking a GP appointment. Your organisation may have bigger goals and outcomes it is seeking but typically most people will be owning some segment of a broader problem/opportunity.

By ‘live’ I mean the service is mostly unrestricted to your target audience. Private beta you’ll likely be throttling users to learn & iterate and still scaling up to allow more people to use your service. ‘Live’ is what comes after. 

I absolutely am not envisioning that 'live' services that reach it this far are inherently a perfect service that fulfils every need of your user. Maybe you’ve not quite nailed product/market fit or some elements of the journey are somewhat wonky. This is absolutely fine & normal, while you may wind down the amount of people/investment you might have thrown at the problem initially there is typically still work to be done and not every issue addressed.

So… with that hopefully clarified. What do I think should be floating in your brain as you sit there with this live service on your hands.

## Does it do the thing it’s supposed to… well?
As stated previously the service will be fulfilling some sort of purpose. It might functionally be able to provide users with what they need but how well does it do it? 

By this point a team should have some form of monitoring on how its service is performing which is going to be key in assessing what might be worth investing more time into it to make it better. Actively you & the team will be routinely monitoring how the service is performing through some sort of dashboard, [Looker](https://cloud.google.com/looker) seems a popular choice I've found but also things like [DataDog](https://www.datadoghq.com/). It could be keeping track of anything from:
- user conversion rate metrics and if they are lower than industry standard
- is there a sudden decline in retention rate
- the speed of the service is slow with a 3+ second average page load speed
- the uptime of the service is problematic and users couldn’t access the service when they wanted to
- accessibility testing highlights issues for a subset of your users

All of these are valid things to investigate and act upon and in general are healthy signs the team is continually improving the service. These would need to be prioritised against other endeavours but give you a good source of future investments of time. I'd reccomend routinely looking diving into key metrics (say every month) and looking at the trend of the numbers over (3+ months). I've found a monthly meeting to address what I'm seeing in the numbers with the team can work very well as a ceremony to celebrate successes and catch issues. 

The team will likely have some broader OKR’s or KPI’s that the team should be monitoring too (e.g. profitability, uptake, etc) & while otheir part of the service may only contributes a smidgen to these metrics they should be followed to sniff out potential areas of improvement and are good to report on. If the companies goal is to get x% market share or reach profitability by z date then focusing people's attention to that mission reguarily can be worthwhile to keep organisational cohesion. 

Metrics aren’t everything! It is healthy to continue to amass qualitative evidence on the experience of your service. This will give you a deeper understanding of how users feel, what they do as they progress around the service & why they do it. It can highlight more areas that need addressing or spark new ideas about what is missing. Perhaps also there user groups the team hadn’t prioritised at first but feel interesting and unique compared to the other groups that the service primarily is working for. THus, further research might be warranted and further effort to know your users (potential or existing). 
There are loads of ways to get these insights from app store reviews, user satisfaction scores/comments, surveys, interviews, ethnographic research. All can be valuable. 

It’s more than likely the earliest version of your service might not “[solve the whole problem](https://www.gov.uk/service-manual/agile-delivery/how-the-live-phase-works#meeting-the-standard-to-move-into-live)” in the first place. Almost certainly extra effort is needed to make sure the service works intuitively across the wider experience. This could be preventing people from filling out the same form multiple times, what's the non-digital experience like, can you improve the backoffice tools that colleagues use for the service or making sure the service feels consistent no matter where you are within it. As the team finds more time to investigate things that it needed to de-prioritise to get the first version out, you'll still find a wealth of knotty problems. Some of these will have always existed and your service will likely create new ones itself so one again you should remain conscious to the entire service. 

When managing a live service you get the great opportunity to invest more time and effort into knowing your user, from their needs to their patterns of behaviour. Unlike earlier phases when you may have been making more decisions off assumptions, in ‘live’ you likely will have far more expertise than before but staying curious remains important as people change, so will your service need to change with them. 

Added onto this the organisation or your team most likely will have set a vision that was out of reach on purpose & either needs a refresh or might still have room to grow into depending on how big you dreamed. There are some great resources on hallmarks on what makes a [great service](https://good.services/15-principles-of-good-service-design) which might spawn new ideas on how to improve things. The key is to understand that just because you are 'live' doesn't mean you are done. 

## New endeavours
New goals often spring up even if the service is performing well enough. 
While managing a live service you should still be keeping your ear to the ground within the organisation for new directives that could influence the work you do & the service you are responsible for. For example, there could be a new drive to save money/make more profit over growth means you need to look at where you can cut some costs or try to make the service more efficient and cost effective. Or it could be a new partnership is on the horizon so a bunch of new features or [SLA’s](https://en.wikipedia.org/wiki/Service-level_agreement) might land on your plate. Often other teams might also be furiously creating something new too which might require swarming on an endeavour. 
The key is to not falling into a place of being overly reactive and only thinking about the service when something is wrong or urgent. The live service will still need to adapt over time. I’d suggest trying to stay ahead of the pack, especially if you wish to shape what your service becomes and be an active participant in how it evolves.

From previous experience, many new initiatives can start off quite hazy objectives/ideas and don't arrive fully formed. Especially if you catch them early enough. For these occasions I’ve found it helpful to try to use [opportunity trees](https://www.producttalk.org/opportunity-solution-tree/) & working with the team in some form of [ideation session](https://designsprintkit.withgoogle.com/methodology/phase3-sketch/crazy-8s) to figure out how your team & service could contribute to any new stated organisational goal. If you can figure out the outcome stakeholders/bosses are desiring up front then you'll have a greater opportunity to construct and experiment towards the best solution. These activities should help with understanding what contributions you could make and the metrics that you can focus on to fix and in general are well received from those above your head when you communicate how your team of experts would best approach the problem/opportunity. Better to be nice & early and pre-emptive. 

Needless to say. You should continue to stay curious and alert to how your service could change while also monitoring its performance. This in part requires you to continually have a good grasp of the landscape your service sits in.

## Staying relevant
Very much in keeping with the above, is factoring in that your solution’s ability to satiate a need will degrade over time. A users expectation and need will morph and while you may strike gold in your first iteration it’s more than likely you’ll need to evolve the longer you service is 'live'. 

As the landscape around the service shifts then the team shouldn't ignore how that could affect what is 'live'. I'd be cautious to jump on any hype train or bandwagon but clearly right now many people are fascinated and motivated about how tools like ChatGPT could affect day to day work and practices. If you are a teacher, marking submitted homework, the world has presented you a new wrinkle you didn't need to think of previously. Your service, the longer it is available, will not be immune to change. It could be technological advances but equally it could be shifts in people & practices. 

The other big source of judging relevancy would be competitors. Other organisations and teams will likely be tackling a similar problem somewhere and provide a great source of inspiration for change. It's wise to keep note of someone is eating up your market share & what they are doing differently or you keep your ears out for those trying to solve the problem in an interesting direction. If I'm being brutally honest I've never cracked a perfect method to keep track of competitors offerings. I setup a weekly space in my calendar and had a miro board of a competitor analysis template and a list of companies but didn't find it easy to do the task every single week. No matter how you find the time, in general if you can have a play (acutally use their service) and reflect on how it differs and what is interesting. Then communicate it back to the team then this is a good healthy behaviour to have. 

Lastly, in knowing your landscape & staying relevant then I'd say having a go at [Wardley mapping](https://learnwardleymapping.com/#learn-more) is a sound idea. Maybe a bit daunting to learn at first but effectively a way to map your service with all its component parts and try to predict what is unique about it. This helps to decide where you can invest most in or cut costs. After all most products and services are cobbled together with a much wider set of parts, it's rarely just a web page with some buttons on it.

## Contracts
This leads me nicely onto managing the service more broadly & sort of away from users and their experience. 

Likely you’ll have some contracts or arrangements in place to keep the service up and running. Over time you’ll need to keep track of these deals and try to assess their value against whatever else is on the market or building a solution yourself as a replacement. Switching suppliers can be a long winded process and present a lot of risks so worth keeping on track of what’s in the contract and especially knowing when it's due to end. 

You'll naturally end up being a source of institutional memory if you stay there long enough and this is important for things like contracts. It could be that someone else signed the deal, left the company and it's just been getting resigned (somewhat blindly) year on year. I've found useful that if I'm newer to the team & wasn't around during the contract signing days, then one great this is to try write up a summary of what's in the deal and publish it where lots of colleagues can see (e.g. a nice little thread on your teams slack channel). As boring as this may sound, it's easy to forget what you've signed up for and I've found plenty of perks we'd never used bruied in the contracts or been alarmed by how much extra we were paying when we didn't need to. 

## Making the team hum
With the service now in live you’ll likely have a core team which you can continue to dedicate time to making perform consistently. A lot of trust and expertise would of been built over time but it’s still great to continue doing retrospectives and finding ways the team can become as well oiled a machine as possible.

That also might lead to some team members wanting to spread their wings or try some side hustles they are passionate about. I’ve always been very pro in people to continue to learn & grow and letting people go off to invest time in another endeavour, for a time, is usually holistically good for all. You are endlessly chasing having a happy, productive team. People come and go, challenges pop up and disappate and nothing stays permanent so even in 'live' you need to not get lazy and just stay on autopilot forever. 

Thankfully, there are ways to track how well your team is doing. The team can measure team health in metrics such as:
- routine [team health surveys](https://www.teamretro.com/health-checks/team-health-check) at retrospectives
- Google’s [Elite DevOps metrics](https://cloud.google.com/blog/products/devops-sre/using-the-four-keys-to-measure-your-devops-performance)

All of these are just tools to sense if the team is happy, performing as consistently as before and hunt down opportunities to get better. They remain constant no matter what phase you are in.

## Incident management
Being in a live service means at some time, something will go wrong and you & the team will need to deal with it. Over time the team will get better at diagnosing issues but needless to say it can be somewhat stressful when one of the services you own stops working and people are breathing down your neck to get it back up again.

First advice is to try and nail down some sort of process for incidents early on in the team’s history. Firstly, it’s worth having someone ‘on-call’ so if an incident happens people know whom to contact and be responsible for triaging the issue and coming up with what to do next.

Setting up monitoring of your services to see if they are performing as expected and setting up notifications if things wobble so the team can act fast is also very useful. It’s much better to spot issues early then wait for people to get a bad experience and the organisation to get into a frenzy. 

Next up is a sensible way to diagnose issues when they arise. Simply, not every issue is created equally. Typically some version that means you can rank an issue between:
- urgent: drop everything and fix
- medium urgency: create a bug and fix within the sprint
- non-urgent: create a bug, prioritise later
- ignore: quielty understand that maybe it was a blip you couldn't influence and doing nothing is more valuable then wasting extra time spinning wheels on it

I would suggest starting with having a matrix that pits how many users are affected vs how big is the impact. For example something urgent would be every user is affected and nobody can pay for their items in their basket. Non-urgent on the other hand could be some devices (<5% of all users) can’t change their language settings in their app. I have found in most companies people can become very animated during incidents and emotions are high but it’s good to not be swept up within the storm and stay true to your process of deciding what really is worth all hands on deck and what is not. 

When the incident strikes it is great to keep people informed. This is also internally making sure that stakeholders are aware and feel confident the incident is being handled (having some #incident channel that people can follow is great) but also making sure users know what is happening. Firstly, it’s a much better experience to communicate that something is not working quite right for now to users of the service but also you don’t want to be spammed with reports of an incident from customer service departments or it splashed all over social media. That only amps up the drama.

The last core step is having a well oiled [post-mortem process](https://www.atlassian.com/incident-management/postmortem/templates). You want these to be entirely blameless and focused on finding ways these events don’t happen again/making the service more secure & stable. It’s once again, another ceremony that enforces a learning culture within the team and organisation. Side note: It’s easy to do these and forget about them, so a reminder that it’s worth prioritising improvements and not just doing the theatre of reflecting on what went wrong but never doing anything about it.

## Juggling other things and letting others take some of the burden
With most teams, there will come a point where the service is not the only or main priority. It might be placed in some form of upkeep mode. There will need to be prioritisation against the other services/products/projects you & the team are wrapped up in. Again, if it is performing well and you don't think there are lots of opportunities that would make a big impact then the decision to wind down effort becomes far easier. 

Connected to this, you might endeavour to also more neatly document your service and how it works so others can self-serve or help fix if needs be. As people who know the service inside out might wheel off into other work then ideally you'd leave a strong base of institutional knowledge somewhere. It could be in more formal documentation, week notes, monthly updates, video's or guides published and pinned in Slack. I'm more relaxed on the method but it's usually good if:
- someone can find links to the service's history
- understand how it works
- be able to get answers on how to tinker or improve it
- some justification on why things are the way they are

Largely this investment reaps rewards in the scenario that you have less people committed to the team, say something goes wrong and you are not around and people can go in fix it because they have all they need to do so. Likewise, someone in the future might want to tweak parts of the journey due to some new work and they might be able to do so with minimal aid because you've got just enough guidance for them to solve their own problems.

## Retirement 
At some point your service might be worth wrapping up. In general if the service no longer adds value then it might be worth shutting down. This would probably be well choreographed far in advance as something will have replaced it or metrics indicate it no longer performs or it is too costly to continue maintaining at all. A compelling arguement you will hear when something is on the cusp of retirement is the cost of time and headspace needed to keep something up and running. Usually it's a service barely used and on it's last legs and effectively its a question of opportunity cost. If we stopped looking after x, we could spend more time on y. Most of the times I've seen this occur it has required a lot of discussions with management about when this gets triggered. 

One noteworthy point related to retirement is communication to users. Ideally you want any remaining users to know that the service is being wrapped up and give advice on what to do next. The service doesn’t [need to just vanish](https://www.w3.org/Provider/Style/URI), you should try your best to redirect people to the best next destination.  
 
### Summary
Managing a live service is a wonderful phase to work in. You get time and space to refine your service and make users even happier while also doing things like lowering costs & making things run more efficiently. 

Broadly, you should remain curious about solving user needs, tracking is the service performing well, making sure it stays relevant, assessing all component parts to see what improvements can be made, making sure the team stays happy and productive & being able to handle things when they go wrong. 

The biggest differences to previous phases is: 
- making your monitoring of real world performance more key to decision making over limited evidence/intuition
- continue to find joy in making either smaller incremental tweaks to your service or investing time in more knotty wider service issues rather than big splashy releases
- taking more time to establish stable foundations to make sure the service can run smoothly rather than moving fast with compriomises
- thinking about it's long-term future and potential end then hustling to make it a reality
- getting it to a point that it doesn't really need you anymore and you don't become a focal point for the service to exist

I no longer remember who said this but I'll end on a quote I've always enjoyed...
> You learn most when it's live

I think this is true. Having something out there in the wild is a brilliant culmination of lots of hard work but is by no means the end of a journey, simply the start of a new one where you get to learn more and make even more things better.

#### EXTRA: Your own growth
After re-reading this blog post I'm adding in an extra section. IMO you want to have a role that you are passionate about and are continually learning something. It's entirely possible that you'll max out this feeling if you remain in the team for a very long stretch. Like any annoying product manager I love a good matrix and this one talks about a way to sense [if it's a good time to move on or not](https://sarah-weiler.medium.com/knowing-when-to-quit-introducing-the-quitting-quadrant-model-37ff083f12a2). Your team will be naturally thinking the same thing so if you do intend to stick around then plan ahead for team changes and succession plans.
