---
title: Continuous visibility, no more dashboards
category: "monitoring"
cover: photo-1465070845512-2b2dbdc6df67.jpg
author: JB
---

The first panicked 3am call from a founding member of the company telling you that something is down and you have 10 minutes to fix it! ...is a great day!. It means your software means something. It has value. But after the dust settles and we all realise that we don’t know when the next critical failure is, how do we start gaining visibility on the health and fitness of our systems? are dashboards the answer?

This post aims to reflect my own teams journey on gaining visibility in our erupting swarm of microservices along with their emergant capabilities and why dashboards were often a siren to the rocks.


### What are dashboards

...!

### What is visbility

...!

![](./dash-rash-12334.png)

### A tale of accidentally important software


:honeybee: *"Microservices are amazing little creatures, instead of designing direct solutions to individual problems we compose our systems down to small powerful masters of domain goodness, each smart, aware and empowered by data sovereignty we watch the capabilities of the resulting platform emerge from the primordial soup of chaos"*

When our team chose to embrace microservices as our default mindset, we stopped working out how to deliver outputs and started to decompose domain specific problems into a platform which would by its nature deliver the **outcomes** desired. Whilst this was empowering to the platform, business capabilities and developers, as many *"micro-developer"* will know, it comes with a whole host of new problems opened up by the increased numbers of **seams** in the new system. 

This also enabled the business and developers to quickly pounce on new market opportunities by looking at the individual capabilities of each microservice and rapidly combining and composing their features to create *"mash-up"* products. Because our services were self documenting, used decoupled communication patterns and homogenous proctocols and security, there was no need for users of our services to let us know they were using it. Whilst *mash-ups* where often failures (which didn't matter as these were cheap to experiment and fail), some were successes, this could lead to sudden promotion of the importance of a service, silently becoming more important to the business's bottom line.

:honeybee: *"A consequence of Microservices is emergent capabilities. 
This decoupling from your customers means a service can go from unused to mission critical without any deliberate plan or warning"* 

Needless to say, we were not necessarily aware off our systems health, capabilities, capacity or creakyness. How fast was it going?, how fast could it go?, how fast does it need to go (SLA's)?, is it about to fail?, how long would it take us to recover it if it did fail (what was our MTTR)?

Our visibility stategy at this point was **"Customer Driven Visibility (CDV)"**, in other words, someone was watching the *"Bat Phone"* at all times and most would argue, once your customer has seen the issue, its too late, disaster recovery is post visibility.

```javascript
import visibility!... now please!
```

Whilst this post is less about how we gained visibility and more about why dashboards sometimes worked against us, lets briefly outline what I believe are the 5 levels of visibility in a system.

### Visibility level 0

We dont know what the hell our system is doing, all we know is customers are not complaining.

### Visibility level 1

We know if our hardware is overloaded and some people will get called if a server fails or a service stops

### Visibility level 2

We are emitting timings from our code which could indicate problems, these timings are hooked up to dashboards in the office so if anyone is around and looking, we may pevent an issue

### Visibility level 3

These timings will now cause phones to ring, auto-scaling to occur, things to happen

### Visibility level 4

Monitoring as part of our dev process. The team takes visibility seriously, they run "Game Days" to uncover thier MTTR. They deploy chaos testers into their environments. They know their SLA's, their SLI's and their SLO's.

### Visibility level 5

Using the knowledge from level 4 they employ a range of automated strategys to prove performance targets are being hit, systems are up and functional and report where bottlenecks are emerging down the line. They have lifted key e2e tests into production and redirected the test ouputs to monitring systems for real world production proving and health checking.

At this point, if your sitting in the pub and your CEO calls you telling you the system down you can confidently state that it isnt and she should check their internet connection.

### Dashboards are a trap

Now we know what