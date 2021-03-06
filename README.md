# k8s-is-not-a-paas

[![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/)

Kubernetes is awesome for all sorts of reasons: convergence; idempotency; API extensibility; elegance; its declarative nature. It also **isn't a PaaS**.

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">The delta between Kubernetes and a developer friendly PaaS is where the next layer of value is and where things tend to get opinionated -- a requirement for reliable end to end workflows.</p>&mdash; Kelsey Hightower (@kelseyhightower) <a href="https://twitter.com/kelseyhightower/status/1099731286950727680?ref_src=twsrc%5Etfw">February 24, 2019</a></blockquote>

This repo contains an SVG diagram with a permissive license that aims to visualise this delta:

![Comparison of IaaS, PaaS and KaaS](/iaas-kubes-paas.svg?raw=true&sanitize=true)

* [SVG](/iaas-kubes-paas.svg?raw=true&sanitize=true)
* [PNG](/iaas-kubes-paas.png?raw=true)

## Intention

The diagram aims to illustrate the difference in functionality between PaaSes like Cloud Foundry, and 'raw' Kubernetes. We have encountered many folks asking "should I use Cloud Foundry or Kubernetes", not realising that they are very different things.

The diagram does _not_ indicate that the functionality 'missing' from Kubernetes cannot be added; rather that these don't come preconfigured 'out of the box'. You will need to configure in-built primitives (e.g. RBAC), choose plugins (e.g. CNI), choose extensions (e.g. cluster DNS, ingresses, log aggregation), configure all of those, keep them all patched, and also test that new versions work nicely together.

## Usage Terms

Please feel free to use and remix. Please attribute and do not place more restrictive licenses on adaptations.

This diagram is licensed with Creative Commons By-ShareAlike International 4.0.

## Engineer's Caveat

The diagram was exported from Google Slides, so apologies for the awful SVG markup.
