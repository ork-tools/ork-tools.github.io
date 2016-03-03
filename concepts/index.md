---
layout: page
title: concept glossary
---

**bounded context** [see](http://martinfowler.com/bliki/BoundedContext.html)

: A self-contained and complete unit of a system model.

**core logic**

: the behaviors in the domain aggregates and process managers. Core logic is "pure" in that it has no
immediate side effects, but instead 

**kernel**

: a unit of domain code that can be trusted and shared among bounded contexts

**processor**

: provides orchestrations in the system [[core]].

  * They generally form the command API for the system core.
  * They define the [[business transaction]] boundaries. 
  * They often coordinate operations between multiple [[aggregates]].
  * 
