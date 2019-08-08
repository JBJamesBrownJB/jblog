---
title: Continuous visibility, no more dashboards
category: "monitoring"
cover: DashRash.png
author: JB
---

##My software fails! …and so does yours!

In my experience working with agile software teams practising CI and CD, we were still far away from dealing with outages elegantly. It wasn’t until a few of our systems, through successful business manoeuvres were elevated to increasing levels of criticality that we began to put more thought into monitoring, reliability, observability and outage planning into our day to day.

Just like the tools, practices, culture and processes that makes CI and CD work, continuous visibility (CV) is to harness practices such as chaos engineering, monitoring and observability into our dev process in an attempt to reduce nasty surprises on our way.

###One of the tools we utilised to help us was dashboards.

We were already recording a wealth of insights about our systems such as timings, logs, tracing and hardware profiles to centralized stores and we started to mount overhead monitors in our office to present various collections of this data to the development teams. It was a simple and effective boost to visibility…and also makes the office look all modern and techy. But as with everything, if you build it, they may not come. No silver bullets in this world and often left neglected the value of our dashboards degraded.

The lightning talk I delivered at muCon 2019 focuses on how we can keep value in our overhead dashboards as well as my teams journey on gaining visibility in a critical new system we were challenged to build.


### muCon Conference, London, 2019

[![Conference video not found](notclear.PNG)](https://player.vimeo.com/video/339167478 "Continuous Visivility, no more dashboards!")

<br />

-------

<br />
There was an interesting question from the audience after this talk which wasn’t captured in the video (partly down to me trying to evade questions ). The question was:

_“Can you talk about some of the tools you used for aiding visibility in your team”_
    
This question actually caught me by surprise, and whilst they were absolutely correct and maybe I should have spoken about some of the tools we used such as Nagios, CheckMK, OPSGenie, graylog, graphite, grafana. It struck me that the successful visibility we had on this project was not down to the tools we used but much more about the culture of visibility we adopted and the mindset we had. Embracing outages were more important than embracing tools. However, I’m not sure we would have been able to do it without the tools listed above.

Just like tools, dashboards don’t bring visibility alone, they are just another way to empower the culture that breeds visibility.

![](dash-rash-12334.png)