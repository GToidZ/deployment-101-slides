---
layout: section
---

# Concepts

---

# Development Environment
What is development environment?

A **dev**elopment environment is a dedicated space for developers to write, modify, test and sandbox their concepts or code.

In this environment the process of software development happens, it allows developers to
make changes or test new implementations, without affecting their end users.

This environment is supposedly for developers only and shouldn't be used by external users.

---

# Production Environment
What is production environment?

A **prod**uction environment is where the final version or working copy of software is deployed
and made available to end-users.

It is a live environment that needs to be stable, secure and highly available to ensure positive user experience.

Any changes to the environment must be carefully planned, tested and deployed in here to minimize disruptions that can affect users.

---

# Differences of Dev and Prod
||**Development**|**Production**|
|---|---|---|
|**Target Users**|Developers, Testers|End-users|
|**Purpose**|For developing new features and testing|For deploying a usable application|
|**Characteristics**|Unstable, Can have bugs (for devs to fix)|Stable, Minimal errors, Crash-proof|

However, deployment is not just a term that can be used with only Production environments.<br>
Even Development environments can apply the same principles.

---

# Types of Hosting
Choose how to host your application before deploying.

There are multiple ways you can host your application, and each have varying costs. We can most likely find three different groups of hosting methods:
* **Dedicated hosting**
    * ✅ You have your own physical server with all the resources available.
    * ✅ You are in control of environment and tooling available.
    * ❌ You are required to configure everything from scratch (even the hardware).
    * ❌ Costs a lot, the target customers are mostly enterprises.

Example use cases: Streaming servers, Big data, Video game servers, high traffic servers (i.e. Google, Facebook, Youtube)

---

# Types of Hosting
Choose how to host your application before deploying.

* **Shared hosting**
    * ✅ Almost no need to configure anything, works-out-of-box.
    * ✅ Small fees and cheap.
    * ⚠️ You might not be able to find hosting providers for your specifications.
    * ❌ You cannot choose environment nor tooling, most likely provided as-is.
    * ❌ You share resources with others, your instance can be powered off.

Example use cases: Web hosting, Email hosting, WordPress

---

# Types of Hosting
Choose how to host your application before deploying.

* **Cloud hosting**
    * ✅ Modular and customizable services, choose what you want to use.
    * ✅ Spin up instances or tooling based on what you need.
    * ✅ Cloud is always scalable.
    * ⚠️ Pricing model is on-demand. Pay for what you use.
    * ❌ Many services needed to be managed due to natural modularity of cloud services.
    * ❌ No standardized cloud strategy, tools and ecosystems create a steep learning curve.

Example use cases: Web applications, Software as a service, Serverless computing

*We'll likely tackle this approach!*

---

# Domain Names
Give your application a flair.

In Internet, a domain name is a string that identifies a network domain or an IP address. All servers on Internet
always have one or more IP addresses. To aid users in finding the correct server route, a domain name helps a lot.

Domain names always require money to even get started. *("free" never meant free)*

So, your final project isn't required to have a customized domain name.

---
layout: center
---

# 12-Factor App
[Reference slide](https://docs.google.com/presentation/d/1nO6cQBjoavqjNY3p7tnP-Gu9el231g_y/edit?usp=sharing&ouid=112038110271235589258&rtpof=true&sd=true)