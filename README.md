# Applied Statistics – Problem Set

This repository contains my work for the Applied Statistics assignment. All problems were completed in a Jupyter notebook using Python's standard library (`math`, `itertools`, `random`), NumPy, SciPy, and Matplotlib. Each section includes code, explanations, and simulation results.

## Problem 1 – Extended Lady Tasting Tea Experiment
This problem extended the original 8-cup Lady Tasting Tea setup to a 12-cup version (8 tea-first, 4 milk-first).

Steps included:
- Calculated the exact probability of guessing all cups correctly using combinations.
- Simulated repeated random guesses to estimate the same probability.
- Compared analytical and simulated results.
- Compared the 12-cup probability with the original 8-cup version.
- Discussed what the lower probability implies and whether the usual p-value threshold should change.

## Problem 2 – Sampling Distribution of the Standard Deviation
This problem examined the difference between population SD (ddof=0) and sample SD (ddof=1).

Steps included:
- Generated 100,000 samples of size 10 from a standard normal distribution.
- Calculated both population and sample SD for each sample.
- Plotted both SD distributions on the same axes.
- Explained why sample SD values tend to be slightly higher.
- Discussed how the difference shrinks when sample size increases.

## Problem 3 – Type II Error in t-Tests
This problem looked at how Type II error behaves for different effect sizes.

Steps included:
- Tested mean differences from 0 to 1 in steps of 0.1.
- Ran 1,000 independent t-tests for each difference.
- Recorded how often the null hypothesis was rejected.
- Converted results to Type II error rates.
- Plotted Type II error vs. effect size and explained the trend.

The results show high Type II error when the true mean difference is zero, decreasing quickly as the difference grows, and approaching zero for large effect sizes.

## Problem 4 – ANOVA vs Multiple t-Tests

This problem compared ANOVA with multiple t-tests when analyzing more than two groups.

Steps included:
- Generated three independent samples from normal distributions with means 0, 0.5, and 1.
- Performed a one-way ANOVA to test if all three means are equal.
- Conducted three independent two-sample t-tests for each pair of samples.
- Compared the statistical conclusions from both approaches.
- Explained why ANOVA is preferred over multiple t-tests.

The results show that ANOVA correctly detects overall group differences while controlling Type I error, whereas multiple t-tests can lead to inconsistent conclusions and inflated error rates.