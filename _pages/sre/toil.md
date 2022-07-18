---
title: Toil
permalink: /sre/toil/
layout: single
sidebar:
  nav: "sre"
toc: true
toc_label: "Helpers"
toc_icon: "cogs"
---

## What is Toil
Any important task e.g. deployments, cache refresh etc. which is manual, repetitive, automatable, scales linearly as system grows.

## Examples of Toil
- Manual or semi-manual software release
- Manual release approvals
- Manual scaling to respond to growing traffic
- Checking system health
- Manual user creation
- Manual cache refresh
- Manually adding or removing server from the loadbalancer configuration

## Examples of What is not Toil
- Meetings
- Coding
- Brainstorming, planning and agile sessions

## Why toil is bad
- Hinders the speed of progress
- Inconsistent or poor quality
- Career stagnation
- Attrition due to job non-satisfaction
- Never ending manual tasks
- Employee burnout

## What can be done to reduce Toil
- Dedicated engineering time to work on toil
- Developing an external automation like scripts to deploy a service
- Developing an internal automation like as part of a service
- SRE works 50% enginerring tasks like automating toil and rest 50% on manual operation tasks. Anything above 50% manual ops is redirected to product team.

