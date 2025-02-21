---
title: Custom load balancing rules
pcx-content-type: concept
weight: 18
meta:
  title: Custom rules
---

# Custom rules

Use load balancing rules to customize the behavior of your load balancer. For example, create a rule that selects an origin pool based on the URI path of an HTTP request.

## More details

You can [create Load Balancing rules](/load-balancing/additional-options/load-balancing-rules/create-rules/) whenever you create or edit a load balancer in **Traffic** > **Load Balancing**.

As with [firewall rules](/firewall/cf-firewall-rules/), each Load Balancing rule is a combination of two elements: an [expression](/load-balancing/additional-options/load-balancing-rules/expressions/) and an [action](/load-balancing/additional-options/load-balancing-rules/actions/). Expressions define the criteria for an HTTP request to trigger an action. The action tells Cloudflare how to handle the request.

When building expressions for Load Balancing rules, refer to [Supported fields and operators](/load-balancing/additional-options/load-balancing-rules/reference/) for definitions and usage.

## Availability

By default, non-Enterprise customers have **one** Load Balancing rule **per domain**. For more rules, upgrade to [Enterprise](https://www.cloudflare.com/enterprise/).

## Limitations

At the moment, you cannot use load balancing rules with [Cloudflare Spectrum](/spectrum/about/load-balancer/).
