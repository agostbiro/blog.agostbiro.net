---
title: "A Forkable Company"
date: "2020-01-29"
description: "A forkable company’s code is not only open source, but also makes it easy to replicate its services. This post explains how that works."
---

> By letting it go, it all gets done.
> 
> <cite>Tao Te Ching</cite>

Network effects lead to natural monopolies in many internet markets. This is problematic, because monopolies are not subject to market-based incentives for good behavior. Open source projects solve a similar problem by forking: if a faction does not agree with the project’s leadership, they can duplicate the project and continue in a different direction.

I believe the time is right today to bring the principle of forking to software startups. Software startups are forkable given four conditions:

1. All code is open source.
1. The operation of the software stack is commodified and specified in code.
1. No API or data lock in.
1. No fixed costs and no regulatory approval required to run the business.

Open source software is old news, but two other recent developments made forking companies viable: infrastructure as code and the serverless stack. Infrastructure as code lets developers declaratively specify what services they want to consume and then provision those services automatically while the serverless stack brings commodified operations to cloud services. Commodified operations mean that software companies can source their operational needs from the market (as opposed to hiring people to do it). Combined with infrastructure as code, the serverless stack lets a company operate their services securely and with high availability, but without having employees who operate those services. Externally this means that if a company open sources their serverless architecture, anybody can duplicate their services and provide the same level of security and availability at scale.

But why isn’t it enough if the code itself is open source? Because the forkability claim is worthless if it’s not easily verifiable. A company should be only considered forkable if an experienced programmer can replicate its services in an hour and operate them at the same level of availability and security at scale.

A forkable company operates under constant threat of obliteration. Piss enough people off today and a new competitor has taken your business by tomorrow. So why would you start a forkable company? Well, besides good karma, it’s also good strategy. Creating a forkable company in a new market for customers that care about such things[^1] forces your competition to operate as forkable companies as well. This means that the internet monopolist’s standard playbook of raising a lot of money to outspend the competition until they can consolidate the market is checked: After all, who would invest in a forkable company? They are not defensible by definition.

Your margins are now everybody’s opportunity, so get used to tight margins. But that’s ok, because you don’t have to raise any money to run a successful forkable business. The overhead of contributing to your company’s codebase is minimal which means you can hire programmers on a commit-by-commit basis as your cash flow allows. Got a new bug report? Put a bounty on it and receive offers in hours. Wondering how to scale support? Your CRM is Github and Stack Overflow, all indexed for search. Instead of chatbots, you are building a community now that gives you instant feedback on new features. This is the power of a forkable company.

[^1]: It’s often enough for a small percentage of users to care a lot in a networked market. See [Mapping Crytpo: The Minority Rule](https://blog.agostbiro.net/2019/06/mapping-crypto-minority-rule/) on how this could play out in personal payments.

---

_[Dokknet](https://dokknet.com) which provides a documentation paywall for open source projects is a forkable company. You can read more about Dokknet in [A New Open Source Business Model](https://blog.agostbiro.net/2020/01/a-new-open-source-business-model/) or just go ahead and fork it on [Github.](https://github.com/dokknet/dokknet/blob/master/forking.md)_

