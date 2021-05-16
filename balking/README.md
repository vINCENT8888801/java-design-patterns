---
layout: pattern
title: Balking
folder: balking
permalink: /patterns/balking/
categories: Concurrency
tags:
 - Decoupling
---

## Intent
Balking Pattern is used to prevent an object from executing certain code if it is an
incomplete or inappropriate state

## Explanation

Real world example

> Consider a washing machine. A washing machine that is currently washing clothes should not execute wash command when washing so it doesn't redo the whole washing process again.

In plain words

> It prevent an object from executing it's method during it's incomplete or inappropriate state by returning or throwing exception while doing nothing.

> The balking pattern is a software design pattern that only executes an action on an object when the object is in a particular state. For example, if an object reads ZIP files and a calling method invokes a get method on the object when the ZIP file is not open, the object would "balk" at the request.
 

**Programmatic Example**


## Class diagram
![alt text](./etc/balking.png "Balking")

## Applicability
Use the Balking pattern when

* you want to invoke an action on an object only when it is in a particular state
* objects are generally only in a state that is prone to balking temporarily
but for an unknown amount of time

## Related patterns
* Guarded Suspension Pattern
* Double Checked Locking Pattern
