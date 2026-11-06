# Experiment Guardrail Metrics

Guardrail metrics are measures a team watches to make sure an experiment does not improve one result at an unacceptable cost elsewhere. They belong in the test plan before anyone sees the outcome.

## The checkout test that won more orders and less money

Consider a hypothetical retailer testing free express shipping at checkout. The company randomly assigns 5,000 eligible visitors to each version.

- Standard checkout: 200 purchases, a **4%** purchase rate.
- Free express shipping: 235 purchases, a **4.7%** purchase rate.

The shipping offer brings in 35 more orders. A conversion report would call that encouraging.

But the business earns an average contribution of $28 per order with standard shipping and $21 with the offer, after relevant variable costs.

- Standard: **200 × $28 = $5,600** contribution.
- Offer: **235 × $21 = $4,935** contribution.

The version with more orders produces **$665 less contribution** from the same number of visitors.

These results are illustrative. A real test would need an uncertainty analysis before concluding that either version is better.

## Write down what cannot get worse

Before launch, the team could choose completed purchases per eligible visitor as its primary outcome and contribution per visitor as a guardrail. It might also monitor refunds and payment failures.

A different experiment needs different guardrails. An onboarding change might track support contacts and seven-day [activation](https://startup-growth.github.io/growth-marketing-glossary/terms/activation-rate/). A price test could track cancellations and net revenue, not just initial purchases.

If a metric matters enough to reverse a decision, decide how to measure it and what regression is unacceptable before the result arrives.

## A green dashboard is not a safety certificate

When an experiment shows no detectable change in refunds or cancellations, that does not prove those outcomes were unaffected. The sample may be small or the harm may appear months later.

[A/B testing](https://startup-growth.github.io/growth-marketing-glossary/terms/a-b-testing/) helps estimate what changed. [Growth experimentation](https://startup-growth.github.io/growth-marketing-glossary/terms/growth-experimentation/) keeps the hypothesis and decision on record. [CRO](https://startup-growth.github.io/growth-marketing-glossary/terms/conversion-rate-optimization-cro/) helps determine whether an improved page metric is worth anything to the business.

The point of guardrails is to avoid shipping a local win that creates a larger problem.

**References:** [Statsig's experiment guidance](https://docs.statsig.com/experiments/overview) and [sample ratio mismatch checks](https://docs.statsig.com/experiments/monitoring/srm).
