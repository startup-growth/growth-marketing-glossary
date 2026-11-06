# Funnel Analysis

Funnel analysis follows people through a sequence of events to see where a journey breaks down. A signup funnel or checkout funnel is more than a chart of totals. Its event order, time window and customer segments determine what the numbers mean.

## The checkout problem hidden in the overall total

A hypothetical online store notices that completed purchases have fallen. The team splits checkout activity by device over the same period:

- Mobile: 800 people begin checkout, 600 reach payment and 240 buy.
- Desktop: 400 begin checkout, 360 reach payment and 288 buy.

Mobile checkout completion is **240 ÷ 800 = 30%**. Desktop completion is **288 ÷ 400 = 72%**.

The striking difference comes after the payment step. On mobile, 240 of 600 people who reach payment finish buying, or **40%**. On desktop, 288 of 360 finish, or **80%**.

The team has a specific place to investigate. It should not start by redesigning the homepage or buying different traffic.

## Find out what happened at payment

Open the mobile checkout, try paying with different methods, and inspect payment failures and validation errors. Perhaps a third-party wallet button is broken on certain phones. Perhaps customers are rejecting an unexpected shipping charge. Those problems require different fixes.

The funnel only shows where people stopped. It does not tell you which explanation is true.

Check the instrumentation before trusting the comparison. Does “reached payment” fire when the page loads or only after the person submits valid billing details? Can someone trigger it twice? Are purchases tracked after the payment processor redirects back to the site?

## Keep the sequence honest

Give people a consistent time window to finish. A customer who starts checkout at 11:58 p.m. and pays after midnight should not vanish because the report resets at the calendar boundary.

[The growth funnel](https://startup-growth.github.io/growth-marketing-glossary/terms/growth-funnel/) explains the stages leading to a business outcome. Funnel analysis examines actual event sequences and losses within those stages. Compare new users at the same age with [cohort analysis](https://startup-growth.github.io/growth-marketing-glossary/terms/cohort-analysis/), then test a proposed fix through [experimentation](https://startup-growth.github.io/growth-marketing-glossary/terms/growth-experimentation/).

**Further reading:** [Amplitude on funnel analysis](https://amplitude.com/blog/funnel-analysis).
