# Intro to Border Gateway Protocol (BGP) Overview Guide

**Description/Overview:** Border Gateway Protocol (BGP) is the internet's common, standardized exterior gateway routing protocol. Routers rely on it to relay accessibility and routing information with various networks/autonomous systems (ASes), enabling traffic to discover optimal paths between source and target networks. Furthermore, when BGP is used to route for a single autonomous system, it serves as an interior border gateway protocol.

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

**BGP attributes are also grouped into four categories:**

* *Well-Known Mandatory (e.g., AS_PATH, NEXT_HOP, ORIGIN):* These attributes have to be recognized by every BGP implementation and need to be included in all BGP update messages.
* *Well-Known Discretionary (e.g., Weight, LOCAL_PREF):* These attributes are recognized by all BGP routers and included in processing, yet are not necessarily included in all update messages.  
* *Optional Transitive:* While it is not a certainty that routers will recognize these attributes, they will be passed along to other BGP routers for sure. Even if a router is not configured to support a transitive attribute, it will still forward it.  
* *Optional Non-Transitive:* It is not a certainity that routers will recognize these attributes. If they do not, then they will also not forward the attribute information to other BGP routers.

<hr />

## 6. <a name="supplemental">Supplemental Resources</a>

* *[Official National Telecommunications and Information Administration Webpage on BGP Security](https://www.ntia.gov/programs-and-initiatives/border-gateway-protocol)*
* *[Official Microsoft Webpage on BGP Support in Microsoft Azure](https://learn.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-bgp-overview)*
* *[Official AWS Webpage on BGP Integration](https://docs.aws.amazon.com/directconnect/latest/UserGuide/routing-and-bgp.html)*
