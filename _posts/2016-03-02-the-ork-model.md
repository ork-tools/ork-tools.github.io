---
layout: post
title: the ork model
---

**ork** suggests and provides tooling for a reasonably simple model:

### *Domain clients* send *commands* and *notifications* to the *core logic*
Commands represent a directive to perform some defined action in the system, such as *"Charge customer THX1138 $1,324.00."*
Notifications represent some external event that the system is interested in, such as *"The recurring charge for subscription 8675309 was declined."*
In the **ork** model, commands and notifications are referred to, collectively, as *messages*.

There is nothing new about this, but what should be noted is that the mechanism is not specified.
RESTish-like APIs are the golden hammer of the day, but REST assured that something else will be in fashion
within a few years.

### The core logic validates the messages and plans the *logical results* and *real actions* that should occur in response to the messages


### The core logic commits one or more *events* to record the *logical results* of the messages

### The planned real actions are executed

### Projectors watching the *event stream* update views to reflect the new state of the system

