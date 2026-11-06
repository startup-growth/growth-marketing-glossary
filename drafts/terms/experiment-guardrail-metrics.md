# Experiment Guardrail Metrics

Guardrail metrics are measures an experiment should not materially damage while trying to improve its main outcome. They protect against a change that wins on one dashboard number while making the customer experience or economics worse elsewhere.

## What happens when clicks increase but useful signups fall?

Imagine a hypothetical signup experiment. A redesigned button raises click-through rate from 12% to 15%.

Qualified signups, however, decline from 4% to 3% of eligible visitors. More people click, but fewer suitable customers complete the journey.

This does not establish a real treatment effect. The figures are illustrative. A genuine experiment needs an appropriate design, enough observations, and uncertainty estimates.

It does show why qualified signups, not button clicks alone, should inform the shipping decision.

## Which metrics should be guardrails?

| Role | Example for a signup test | Question |
| --- | --- | --- |
| Goal metric | Qualified signups per eligible visitor | Did the change achieve its purpose? |
| Guardrail | Form error rate | Did reliability worsen? |
| Guardrail | Early refunds or cancellations | Did the change attract worse-fit customers? |

Choose guardrails that could plausibly be affected by the change. A pricing test might monitor refunds and cancellations; a checkout test might monitor failed payments.

State the maximum acceptable regression before seeing the result. If the experiment is too small to detect a meaningful decline, the guardrail cannot offer much protection.

## Does a passing guardrail prove the change is safe?

No. An undetected decline is not necessarily an absent decline. Small samples can miss important harm, and long-term effects may appear after the experiment closes.

Use [A/B testing](https://startup-growth.github.io/growth-marketing-glossary/terms/a-b-testing/) to estimate the effect of a variation. [Growth experimentation](https://startup-growth.github.io/growth-marketing-glossary/terms/growth-experimentation/) provides the decision process, while [CRO](https://startup-growth.github.io/growth-marketing-glossary/terms/conversion-rate-optimization-cro/) keeps the focus on business outcomes rather than cosmetic engagement.

**Further reading:** [Statsig on guardrail metrics](https://statsig.com/blog/what-are-guardrail-metrics-in-ab-tests).
