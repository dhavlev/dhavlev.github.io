---
title: What is SRE?
permalink: /sre/what-is-sre/
layout: single
sidebar:
  nav: "sre"
toc: true
toc_label: "Helpers"
toc_icon: "cogs"    
---

## Site Reliability Engineering (SRE)
It is a discipline that incorporates software engineering aspects to the infrastructure and operations problems. The term SRE was coined by Google and it in practice since 2003 at Google.

## Goals of SRE
- Create an ultra-scalable and highly reliable distributed software system. 
- SRE spends 50% of their time on operations-related activities like on-call and manual intervention and the rest 50% on development like new features, scaling or automation. 
- Monitoring, alerting and automation are central to SRE. 

## What is DevOps
`RAILM`
- Reduce organisational silos
- Accept failure as normal
- Implement gradual changes
- Leverage tooling and automation
- Measure everything

## SRE Principles
#### Operations is a software problem

Focus is on designing and building rather than operating and maintaining. Estimates suggest that anywhere between 40% and 90% of the total cost of ownership is incurred after launch.

#### Service levels objective
SLO is an availability target for a service or product. SLO needs consequences if violated.

#### Toil
Any manual operational task is bad. If a task can be automated then it should be automated.

#### Automation
Automate what is manual with an engineering approach. Don't automate bad process, fix the process first.

#### Reduce the cost of failure
Promote progressive rollouts/canary deployments. Shift left in every aspect of SDLC-related task to discover issues in the early phased of a cycle. Improve MTTRecover and Repair. Rollout small changes vs big changes.

#### Shared ownership
No boundaries between application development and production support. SREs are instrumental in sharing skills and production experience with the development teams to shift left.