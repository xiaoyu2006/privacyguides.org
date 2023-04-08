---
title: "Browser Fingerprinting"
icon: material/fingerprint
description: Browser fingerprinting is a method of tracking users across sites regardless of their network.
---

**Fingerprinting** refers to a service collecting metadata about whatever connects to it, for the purposes of identifying a user. In this overview we are largely going to cover **browser fingerprinting**, specifically how websites try to uniquely identify your web browser outside the standard identifiers most people think of, like your IP address or user agent.

!!! abstract "TL;DR"

    The **only** reliable way to thwart all fingerprinting scripts and be anonymous is to use [Tor Browser](../tor.md). Other browsers can only confidently fool certain tracking scripts, and will **never** be unidentifiable despite any claims otherwise. However, the anti-fingerprinting approaches used by other browsers and described here can still be useful in protecting your privacy.

Many people think their browser fingerprint is a single thing, like your actual fingerprints, a string of characters like `XP2urbkhQIaHyMQYXYv4` that uniquely identifies their browser, and if they can get theirs to match everyone else's they are safe. However, browser fingerprinting actually refers to the broad collection of all the different metrics which websites can use to track you. Many websites or fingerprinting scripts *will* take all those metrics and hash them into a single identifying string with a fingerprinting algorithm, but the algorithms and the metrics they use to create that fingerprint can vary wildly between different trackers. In other words, just because one fingerprinting test says your browser's fingerprint is non-unique, or randomized, or any certain thing; doesn't necessarily mean that it will be for every other fingerprinting test or tracker out there, because every method of fingerprinting your browser is different.

Many non-experts will claim that using Firefox or enabling its fingerprinting resistance preferences will make you *more* unique, give you *less* privacy, and make you "stand out in the crowd." However, if you do nothing at all your browser will already be uniquely identifiable. Thus, the "crowd" of Google Chrome or Safari users these people will claim exists in fact does not, because you can't blend in to a crowd filled with completely unique browsers. A [study](https://www.ndss-symposium.org/ndss2017/ndss-2017-programme/cross-browser-fingerprinting-os-and-hardware-level-features/) published in 2017 demonstrated an approach that could uniquely identify 99.24% of users, without even taking into account their IP address. ==When you are already completely unique, becoming "more unique" is impossible.== In reality, these fingerprint resistance features are generally not meant to make your browser unidentifiable at all, they merely block tracker scripts from collecting certain metrics, which in turn *can* make your browser unidentifiable to certain—but not all—tracking scripts which rely on those metrics.

## Common Metrics

## Types of Tracking Scripts

In general, we can classify tracking software into two groups: **naive** and **advanced**. Naive trackers can be fooled by standard anti-fingerprinting techniques like Firefox's "resist fingerprinting" or Brave's fingerprint randomization features, because they acc

On the other hand, advanced fingerprinting scripts can detect randomized values (this is always possible) with varying levels of sophistication. The only way to defeat advanced scripts is by blending in with a crowd of other identical looking browsers, which is no easy feat as we've already covered. We'll delve into this more in the next section.

The good news is that most fingerprinting you will encounter on the internet is naive.

## Anti-Fingerprinting Approaches

Broadly speaking, there are two ways that browsers try to deal with fingerprinting: **Randomization** and **blocking**. There are advantages and disadvantages to both approaches, and generally they cover distinct threat models, but both approaches ultimately try and accomplish the same thing: Protecting the real value of each metric.

[Brave](../desktop-browsers.md#brave) takes the **randomization** approach to fingerprinting protection by

## Sources

The [Arkenfox user.js documentation](https://github.com/arkenfox/user.js/wiki) is a very detailed resource about fingerprinting and Firefox's anti-fingerprinting protections, and the data there was used as the basis for most of this article.
