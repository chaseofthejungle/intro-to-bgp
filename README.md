# Intro to Border Gateway Protocol (BGP) Overview Guide

**TODO:** A brief introductory guide to Border Gateway Protocol.

#### Table of Contents

1. [Reasons to Use BGP](#reasons)
2. [BGP Limitations](#limits)
3. [BGP Types and How They Operate](#operate)
4. [BGP and Autonomous Systems](#autonomous)
5. [BGP Attributes](#attributes)
6. [Supplemental Resources](#supplemental)

<hr />

## 1. <a name="reasons">Reasons to Use BGP</a>

<hr />

## 2. <a name="limits">BGP Limitations</a>

<hr />

## 3. <a name="operate">BGP Types and How They Operate</a>

<hr />

## 4. <a name="autonomous">BGP and Autonomous Systems</a>

<hr />

## 5. <a name="attributes">BGP Attributes</a>

A core functionality of BGP routers is to determine the most optimal network traffic paths. They do so not just by considering traditional hop counts, but also using a variety of 'attributes', which are ranked by routing preference. These are assigned to all paths (with admins having granular-level configuration control over them), with the intention of assisting BGP routers in choosing the optimal paths when multiple path possibilities are present.

**Examples of BGP attributes include:**

* *Weight:* Informs configured routers which local paths are to have priority (note: this attribute is Cisco-proprietary).
* *ORIGIN:* Instructs routers to select routes based on how they were added to BGP (e.g., IGP, EGP, INCOMPLETE).
* *LOCAL_PREF:* Informs routers of the outbound/exit paths that should be chosen for routing.
* *AS_PATH:* Instructs routers to prioritize the shortest paths (the ones with the least amount of AS hops listed in the routes), which can help prevent routing loops.
* *NEXT_HOP:* Provides the IP address of the next (reachable) router that is to receive traffic.
  
<hr />

## 6. <a name="supplemental">Supplemental Resources</a>

* *[Official National Telecommunications and Information Administration Webpage on BGP Security](https://www.ntia.gov/programs-and-initiatives/border-gateway-protocol)*
* *[Official Microsoft Webpage on BGP Support in Microsoft Azure](https://learn.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-bgp-overview)*
* *[Official AWS Webpage on BGP Integration](https://docs.aws.amazon.com/directconnect/latest/UserGuide/routing-and-bgp.html)*
