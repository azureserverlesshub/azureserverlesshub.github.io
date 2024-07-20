---
weight: 1
description: What are the events in event driven architecture?
title: What are events?
tags:
- eda-visuals
keywords:
- eda events
type: "docs"
---
<!--more-->

Events may seem simple, raise something and react somewhere, but as you dive deeper into event-driven architecture and start building solutions you soon realise that there is much more to events that you initially thought.

{{< image "/images/visuals/what-are-events/what-are-events.svg" "Events in Event Driven Architecture"  >}}


Understanding the core concepts, event types and exploring integration patterns with events can really help you understand events at a deeper level, which can help you when building event-driven solutions.

### <u>Immutable Facts</u>

* Events are immutable facts. Things that have happened that cannot be undone or changed.

* Events are great a representing real-life scenarios. Events happen all the time, everywhere. The time you played that song, took the bin out, ordered something online, cooked food, at most situations events are happening.

 ### <u>Event Types</u>
* When you start, you may just be publishing any kind of event without much thought. This works initially but can lead you to problems with inconsistent events, poor event design, migration and much more.

* Events come in many different sizes and patterns, many developers building event-driven solutions use various different event types based on their use case.

* Examples of these are notification events (keeping contracts simple), event-carried state transfer (putting more information into the events), domain events(events representing your domain), delta events (events that give the difference between old and new), and many more…

Understanding these event types can help, and there are more resources below to dive deeper.

### <u>Integration Patterns</u>
Integration patterns give us ways in which we can interact, consume and manipulate information before consumers get it.

* __Anti-corruption layer (ACL)__ is a popular pattern that engineers use to map consumed events into events/models that the consuming domain understands. For example consuming an OrderPlaced event within the Payment domain, the payment domain may want to map this event into a structure/schema that the payment domain understands.

* __Enrichment__ allows events to be enriched with information before downstream consumers consume them. This pattern allows producers to raise simple events, and consumers get information they may require even if it is not on the original event.

* __Conformist__ pattern is when consumers conform to events as they are. No enrichment, no mapping, nothing. They take the event and consume it. This can be great for domains that life close together, but be careful not to conform to implementation details exposed in events.

[Enterprise Integration Patterns](https://www.enterpriseintegrationpatterns.com/) is a great resource to dive deeper into messaging integration patterns. Worth reading and re-reading. 