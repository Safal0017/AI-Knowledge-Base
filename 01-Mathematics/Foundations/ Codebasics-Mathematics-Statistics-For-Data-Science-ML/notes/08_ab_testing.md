# A/B Testing

**Video:** [Simple explanation of A/B Testing](https://www.youtube.com/watch?v=eiIhTbFP0ls)

**Playlist:** [Mathematics, statistics for data science and machine learning](https://www.youtube.com/playlist?list=PLeo1K3hjS3uuKaU2nBDwr6zrSOTzNCs0l)

This note gives a short, practical explanation of A/B testing: how it helps compare two versions of a website, product, or model using data instead of intuition.

## What Problem Are We Solving?

When you change something in a product, you usually want to know whether the new version is actually better.

A/B testing compares two versions:

- Version A = current version
- Version B = new version

The goal is to see which one performs better on a chosen metric.

## Core Intuition

Think of A/B testing as a controlled experiment.

You show one group version A and another group version B, then measure the result.

| Version | Meaning |
|---|---|
| A | Existing design or model |
| B | New design or model |

If B performs better consistently, you may choose to replace A with B.

## Website Example

The video uses a simple website example.

Suppose a company has a contact button at the top right. A business manager thinks moving it to the center may generate more leads.

So the company creates two versions:

| Version | Button position |
|---|---|
| A | Top right |
| B | Middle of the page |

Then traffic is split between both versions for several days.

## Result Example

If after 10 days:

| Version | Sales leads |
|---|---:|
| A | 300 |
| B | 400 |

Then version B looks better because it generated more leads.

## Why It Is Not That Simple

The video makes an important point: you cannot jump to conclusions too quickly.

Two big concerns are:

- Sampling bias.
- Too few samples.

If the users seeing version B are not representative, the result may be misleading. And if the test runs for too little time, a random lucky or unlucky outcome can distort the conclusion.

## Common Mistakes

| Mistake | Why it is a problem |
|---|---|
| Non-random traffic split | Can create sampling bias |
| Too short test duration | Can lead to conclusions from random chance |
| Too few users | Results may not be reliable |
| Comparing without a fixed metric | Makes the test unclear |

The video mentions that statistical significance is needed to decide whether the difference is real or just due to randomness.

## Why Businesses Use A/B Testing

A/B testing is common in websites and product teams.

Examples from the video:

- Amazon layout changes.
- LinkedIn or Facebook page changes.
- Ad campaign experiments.
- Product recommendation model updates.

The idea is always the same: test a change on a smaller group first, then scale it if the result is better.

## ML Relevance

A/B testing is also useful in machine learning.

If a company builds a new recommendation model, it should not be deployed to everyone immediately.

Instead, part of the traffic can go to the new model and the rest can stay on the current model. Then the business can compare performance before making a full rollout.

## Key Takeaways

- A/B testing compares two versions using real user data.
- Version A is the current version, version B is the new version.
- Random traffic split is important to avoid bias.
- Enough samples and enough time are needed for trustworthy results.
- A/B testing is used in product design, ads, and ML model rollout.

## Revision Cheat Sheet

- **A/B test** = compare two versions.
- **A** = current version.
- **B** = new version.
- **Goal** = decide which version performs better.
- **Important** = random split, enough samples, significance.

## 30-Second Revision

A/B testing is a method for comparing two versions of a website, product, or model. You split traffic between version A and version B, measure a metric like leads or clicks, and decide which version performs better. Randomness and sample size matter a lot.

## 2-Minute Revision

If a company wants to change a layout or deploy a new model, it should not rely only on intuition. A/B testing gives both versions a fair comparison by splitting users between them and measuring outcomes. If the traffic is not random or the test is too small, the result may be misleading. That is why significance and careful experiment design matter.

## Engineering Perspective

In product and ML systems, A/B testing is a practical decision-making tool. It helps teams validate changes safely before full rollout, which reduces risk and makes product decisions more data-driven.
