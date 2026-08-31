---
name: marketing-analytics
description: Diagnoses marketing performance, attribution, funnels, and conversion tracking using connected or supplied campaign and analytics data.
---

# Marketing Analytics

## Invoke when
Use for attribution questions, funnel analysis, campaign measurement, GA4/ads tracking, conversion discrepancies, source/medium analysis, or when performance conclusions depend on whether the data is trustworthy.

## Method
1. Define the business outcome and the conversion event representing it.
2. Verify measurement before optimizing media.
3. Map the funnel from impression/click through lead and final sale or booking where data exists.
4. Compare rates, not just totals, and preserve denominator context.
5. Segment only where the sample size can support a useful conclusion.
6. Separate observed facts from attribution-model assumptions.
7. Look for breaks between platforms: click counts, sessions, form submissions, CRM/bookings, and revenue.

## Tool behavior
Retrieve connected analytics or campaign data when available. Inspect tracking configuration, event definitions, URLs, screenshots, exports, or repository code when relevant. When data is partial, state the coverage window and missing stages rather than filling gaps with assumptions.

## Common failure modes
- optimizing to a soft event that is not the business outcome;
- double-counted or duplicated conversions;
- missing cross-domain or referral handling;
- comparing platform-attributed conversions as if attribution models were identical;
- drawing conclusions from tiny segments;
- treating click-through rate as proof of lead quality.

## Collaboration
Use paid-advertising for media decisions, landing-page-cro for page conversion, lifecycle-messaging for lead follow-up, and unit-economics for profitability.

## Return contract
State whether the measurement is trustworthy enough for the requested decision. Then report the key funnel constraint, supporting metrics, uncertainties, and the next measurement fix or experiment.
