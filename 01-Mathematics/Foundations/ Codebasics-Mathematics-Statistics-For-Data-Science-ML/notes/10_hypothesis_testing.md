# Hypothesis Testing

**Video:** [What is Hypothesis Testing ? Math, Statistics for data science, machine learning](https://www.youtube.com/watch?v=fb8BSFr0isg)

**Playlist:** [Mathematics, statistics for data science and machine learning](https://www.youtube.com/playlist?list=PLeo1K3hjS3uuKaU2nBDwr6zrSOTzNCs0l)

This note explains hypothesis testing as a way to decide whether an observed result is likely due to real effect or just random chance.

## What Problem Are We Solving?

When we see a difference between two things, we do not immediately know whether the difference is meaningful.

For example:

- Drug B seems faster than Drug A.
- A new model seems better than the old model.
- Working from home may seem more productive than office work.

Hypothesis testing helps us check whether the observed difference is strong enough to believe.

## Core Intuition

The video uses a pharma example.

A company has an existing headache drug, Drug A. A new drug, Drug B, is claimed to work faster.

Instead of giving it to everyone immediately, the company first tests it on a sample of volunteers.

That is the whole idea:

**Test on a sample first, then decide whether the result is convincing enough.**

## Why We Need It

A small sample can be misleading.

If only 10 people are tested, and Drug B looks faster, that could be due to chance.

Even with 1000 people, the sample may still be biased if the groups are not representative.

So hypothesis testing is used to reduce the effect of randomness.

## Sample Size And Variation

The video highlights two big concerns:

| Concern | Why it matters |
|---|---|
| Sample size | Small samples are noisy and may mislead us |
| Sample variation | If groups are not diverse, the result may not generalize |

For example, if the Drug B group has mostly young people and the Drug A group has mostly older people, the result may reflect age differences rather than drug performance.

## Coin Flip Example

The video also uses coin flipping.

If you flip a coin only a few times, you may see several heads in a row and think the coin is biased.

But that may just be randomness.

This is the key lesson: **random patterns can look meaningful even when they are not.**

## The Purpose Of Hypothesis Testing

Hypothesis testing helps us answer this question:

**Is the observed result likely caused by a real effect, or could it reasonably happen by chance?**

That is why it is used in science, business, and machine learning.

## Null And Alternative Hypothesis

| Term | Meaning |
|---|---|
| Null hypothesis | The default assumption, usually the current or established state |
| Alternative hypothesis | The claim you want to prove |

The video stresses that we usually start by assuming the null hypothesis is true.

Then we try to reject it.

## Drug Example

| Hypothesis | Statement |
|---|---|
| Null hypothesis | Drug B is not more effective than Drug A |
| Alternative hypothesis | Drug B is more effective than Drug A |

The null hypothesis represents the established fact, while the alternative is the new claim.

## Why Start With The Null?

The video uses a courtroom analogy.

A person is assumed innocent until proven guilty.

Similarly, in hypothesis testing, we assume the existing belief is true until evidence suggests otherwise.

This is the same idea as playing devil’s advocate.

## Other Examples From The Video

| Situation | Null hypothesis | Alternative hypothesis |
|---|---|---|
| Sun vs earth model | Sun rotates around the earth | Sun does not rotate around the earth |
| Tennis ranking | Federer is the best player | Federer is not the best player, so someone else may be better |
| Office productivity | Employees are more productive in office | Employees can also be productive from home |
| Food and disease | Food has no relation with irritable bowel disease | Certain food may be related to irritable bowel disease |
| Amazon recommendation model | Model B is not better than model A | Model B is better than model A |

These examples all show the same structure: start with the established belief, then try to challenge it.

## Rejecting The Null

The goal of hypothesis testing is usually not to directly prove the alternative with absolute certainty.

Instead, we try to reject the null hypothesis.

If the null is rejected, the alternative becomes the more believable explanation.

## Common Testing Methods

The video briefly mentions several techniques used in hypothesis testing:

- Z-test
- T-test
- ANOVA
- Chi-square test

These are different tools for different data situations, but the overall logic remains the same.

## ML Relevance

Hypothesis testing is very useful in machine learning and experimentation.

Examples:

- Comparing two recommendation models
- Checking whether a new feature improves performance
- Testing whether a change in UI improves conversion
- Evaluating whether an observed improvement is statistically meaningful

## Key Takeaways

- Hypothesis testing helps separate real signal from randomness.
- The null hypothesis is the default or established belief.
- The alternative hypothesis is the claim you want to support.
- Small or biased samples can lead to wrong conclusions.
- Hypothesis testing is widely used in science, business, and ML.

## Revision Cheat Sheet

- **Null hypothesis** = default belief
- **Alternative hypothesis** = new claim
- **Goal** = reject null if evidence is strong enough
- **Problem** = randomness can create fake patterns
- **Need** = sample size, variation, and significance

## 30-Second Revision

Hypothesis testing is a method to check whether an observed result is likely real or just random chance. We begin with a null hypothesis, which is the default belief, and then test whether there is enough evidence to reject it. This is used in drug testing, experiments, and machine learning.

## 2-Minute Revision

A result can look convincing in a small sample but still be caused by randomness. Hypothesis testing helps us avoid that mistake. We start with the null hypothesis, which represents the current accepted belief, and the alternative hypothesis, which is the new claim. If the data provides enough evidence, we reject the null and accept that the alternative is more plausible. This logic is used in science, business experiments, and ML model evaluation.

## Engineering Perspective

In product and ML systems, hypothesis testing is the foundation of safe decision-making. It helps teams avoid shipping changes just because a small sample looked good. Instead, they use experiments and statistical evidence to make better rollout decisions.
