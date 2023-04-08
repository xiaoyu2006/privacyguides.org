---
title: "Browser Fingerprinting"
icon: material/fingerprint
description: Browser fingerprinting is a method of tracking users across sites regardless of their network.
---

**Fingerprinting** refers to a service collecting metadata about whatever connects to it, for the purposes of identifying a user. In this overview we are largely going to cover **browser fingerprinting**, specifically how websites try to uniquely identify your web browser outside the standard identifiers most people think of, like your IP address or user agent.

It is important to remember that your "browser fingerprint" is not a single thing, it is a collection of all the different metrics websites can use to track you. Many websites or fingerprinting scripts will take all those metrics and hash them into a single identifying string with a fingerprinting algorithm, but these algorithms and the metrics they use to create that fingerprint can vary wildly between different trackers. In other words, just because one fingerprinting test says your browser's fingerprint is non-unique, or randomized, or any certain thing; it doesn't necessarily mean that it will be for every other fingerprinting test or tracker out there.

Many non-experts will claim that using Firefox or enabling its fingerprinting resistance preferences will make you *more* unique, give you *less* privacy, and make you "stand out in the crowd." However, if you do nothing at all your browser will already be uniquely identifiable. Thus, the "crowd" of Google Chrome or Safari users these people will claim exists in fact does not, because you can't blend in to a crowd filled with completely unique browsers. A [study](https://www.ndss-symposium.org/ndss2017/ndss-2017-programme/cross-browser-fingerprinting-os-and-hardware-level-features/) published in 2017 demonstrated an approach that could uniquely identify 99.24% of users, without even taking into account their IP address. ==Becoming "more unique" is impossible, there is no such thing.==

## Common Metrics

## Types of Tracking Scripts

In general, we can classify tracking software into two groups: **naive** and **advanced**. Naive trackers can be fooled by standard anti-fingerprinting techniques like Firefox's "resist fingerprinting" or Brave's fingerprint randomization features, because they acc

The good news is that most fingerprinting you will encounter on the internet is naive.

## Anti-Fingerprinting Approaches

Broadly speaking, there are two ways that browsers try to deal with fingerprinting: **Randomization** and **blocking**. There are advantages and disadvantages to both approaches, and generally they cover distinct threat models.

[Brave](../desktop-browsers.md#brave) takes the **randomization** approach to fingerprinting
