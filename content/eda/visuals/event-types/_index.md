---
weight: 3
description: Different Event types in Event-driven Architecture
title: Exploring different types of events
tags:
- eda-visuals
keywords:
- eda event types
type: "docs"
---
<!--more-->

When building EDA applications, it’s important to know the different types of events you can publish, each has their own trade-offs.


{{< image "/images/visuals/event-type/event-type.svg" "Event Types"  >}}


 ### <u>Event Carried State Transfer Events</u> 
* Enriched events (stateful)
* Higher risk of data being out of sync
* Consumers have the data
* Decreases architecture coupling
* Producer/consumer contracts more coupled
* Higher risks of breaking contracts

 ### <u>Notification Events</u> 
* Minimal information
* Less risk of data being out of sync
* Consumers often need to fetch data
* Increases architecture coupling (callback for info)
* Producer/Consumer contracts kept minimum
* Lower risk of breaking contracts

 ### <u>Delta Events</u> 
* Stores difference between old/new
* Examples seen in change data capture events
* Can reduce complex in consumers needing to figure out what has changed

 ### <u>Domain Events</u> 
* Events that raised in the same bounded context
* Some team reference these as internal events raised in bounded context
* Some team reference these as business “important” events.
* People also refer to “integration” events. These are events used for integrations.