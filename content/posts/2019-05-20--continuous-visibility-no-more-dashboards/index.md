---
title: Continuous visibility, no more dashboards
category: "monitoring"
cover: photo-1465070845512-2b2dbdc6df67.jpg
author: JB
---

The first panicked 3am call from a founding member of the company telling you that something is down and you have 10 minutes to fix it! ...is a great day!. It means your software means something. It has value. But after the dust settles and we all realise that we don’t know when the next critical failure is, how do we start gaining visibility on the health and fitness of our systems? are dashboards the answer?

This post aims to reflect my own teams journey on gaining visibility in our erupting swarm of microservices along with the emergant capabilities it bred and why dashboards were often a siren to the rocks.

![](./dash-rash-12334.png)

### A tale of accidentally important software


:honeybee: *"Microservices are amazing little creatures, instead of designing direct solutions to individual problems we compose our systems down to small powerful masters of domain goodness, each smart, aware and empowered by data sovereignty we watch the capabilities of the resulting platform emerge from the primordial soup of chaos"*

When our team chose to embrace microservices as our default mindset, we stopped working out how to deliver outputs and started to decompose domain specific problems into a platform which would by its nature deliver the **outcomes** desired. Whist this was empowering to the platform, business capabilities and developers, as many *"micro-developer"* will know, it comes with a whole host of new problems often opened up by the increased numbers of **seams** opened up by the new system. 

This also enabled the business and developers to quickly pounce on new market opportunities by looking at the individual capabilities of each microservice and rapidly combining and composing their features to create *"mash-up"* products. Because our services were self documenting, used decoupled communication patterns and homogenous proctocols and security, there was no need for users of our services to let us know they were using it. Whils *mash-ups* where often failures (which didn't matter as these were cheap to experiment and fail), some were successes, this could lead to silent promotion of our services, suddenly and silently becoming more important to the business's bottom line.

:honeybee: *"A consequence of Microservices is emergent capabilities. 
This decoupling from your customers means a service can go from unused to mission critical without any deliberate plan or necessarily any warning"* 

```javascript
import visibility!.... like now please!
```

Needless to say, we were not necessarily aware off our systems health, capabilities, capacity or creakyness. How fast was it going?, how fast could it go?, how fast does it need to go (SLA's)?, is it about to fail?, how long would it take us to recover it if it did fail (what was our MTTR)?

Our visibility stategy at this point was **"Customer Driven Visibility (CDV)"**, in other words, someone was watching the *"Bat Phone"* at all times and most would argue, once your customer has seen the issue, its too late, disaster recovery is post visibility.

### Donec hendrerit laoreet risus eget adipiscing.


