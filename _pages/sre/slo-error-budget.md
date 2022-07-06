---
title: SLO & Error Budget
permalink: /sre/slo-error-budget/
layout: single
sidebar:
  nav: "sre"
toc: true
toc_label: "Helpers"
toc_icon: "cogs"
---

## Service level objectives (SLOs)
- Google has linked customer happiness with the measures of SLOs.
- Behavious of a service or product will dictate if customers were served better and were happy while an interaction with services.
- SLO is a goal which states how well a service should perform or operate or behave when deployed.
- Setting up an SLO is a most foundational activity of an SRE practice.
- A service can have one or more SLOs attached to it. Availability is the most widely used SLO.
- An SLO can be set against the application's latency and availability measurements.
- 100% SLO is impractical and will stagnate or stifle the ability to rollout a new feature or maintenance of a system or service.
- Missed SLO should have consequenace.

## Error budget
- Error budget defines a threshold for a service to error in terms of latency, availibility etc.
- With 99.9% availability SLO, out of 1M web requests in a particular month, 1000 web requests are allowed to fail. Thus, 0.01% becomes the Error Budget for that service.
- Another example of an SLO and Error Budget could be a number of tickets must complete automatically and number of tickets required a manual intervention respectively. For example, out of 1000 tickets with 75% SLO, 750 tickets should close automatically leaving 250 tickets to be completed manually with the Error Budget of 25%.
- Error budget can be utilised for experimentation and launching new features, system maintenance. Small changes are risk-free and avoid the risk of burning the Error Budget rapidly.
- Error Budget should be revisited regularly and adujested in agreement with product, support team and business.

## Examples of SLO & Error Budget
- Service Availability SLO of 99.9% in a particular month

| Request | SLO    | Error Budget |
| ------- | ------ | ------------ |
| 1000000 | 999000 | 1000         |

Only 1000 request in a month can return an error response.

- User Login SLO of 99.99% in particular month

| Login attempts | SLO    | Error Budget |
| -------------- | ------ | ------------ |
| 50000          | 49,995 | 5            |

Only 5 login requests can be unsuccessful even when users have provided valid credentials.

## Policies for non-adherant SLO targets

| Dimension      | SLO                                                                     | Policy                                             |
| -------------- | ----------------------------------------------------------------------- | -------------------------------------------------- |
| Volume/traffic | Does service handles right volume of data or traffic?                   | Address scalability issues                         |
| Availability   | Is service available when needed by the user?                           | Address downtime issues                            |
| Latency        | Does service respond with the accurate response within the agreed time? | Address performace issues                          |
| Errors         | Does service respond with positive http response codes?                 | Rectify issues with infrastructure or dependencies |
| Tickets        | Are support tickets getting completed on time?                          | Automate more manual processes                     |

## Consequences of Missed SLOs
- Lost revenue
- Drop in employee productivity as they will have to spend more time in fixing the systems
- Lost customers
- Lost reputation and credibility