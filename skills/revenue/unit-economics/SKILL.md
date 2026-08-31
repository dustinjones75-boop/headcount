---
name: unit-economics
description: Evaluates whether acquisition, offers, and customer economics create enough contribution to scale, including commission-based and service businesses.
---

# Unit Economics

## Invoke when
Use for CAC/CPL/CPA decisions, marketing budget ceilings, contribution margin, commission economics, incentives, payback, lead-to-sale assumptions, or deciding whether a campaign can scale profitably.

## Core model
Start with the economic unit that matches the business: booking, client, order, cabin, policy, project, or retained customer.

Calculate only from defensible inputs:
- gross revenue or commission;
- variable supplier/fulfillment cost where applicable;
- advisor-funded or seller-funded incentives;
- payment/transaction cost;
- variable servicing cost when material;
- acquisition cost;
- expected cancellation/refund leakage where relevant.

Contribution per acquired customer = economic value retained after variable costs and acquisition.

When the funnel is incomplete, connect the stages explicitly: CPC → click-to-lead rate → CPL → lead-to-sale rate → CAC → contribution.

## Tool behavior
When the request concerns the user's actual financial accounts, spending, or transaction history, use the appropriate connected finance data before concluding. For campaign economics, retrieve connected marketing data when available. Otherwise show assumptions and ranges rather than presenting estimates as observed facts.

## Decision rules
- Do not scale from revenue alone.
- Do not use average commission when product mix materially changes economics.
- Separate one-time customer value from repeat/referral value; do not count future value without an evidence-based assumption.
- Include advisor/seller incentives as costs even when they are positioned as client benefits.
- Use sensitivity analysis when conversion or margin is uncertain.

## Return contract
State the economic unit, inputs, break-even acquisition cost, current/estimated acquisition cost, contribution, and which assumption most affects the decision. Give a scale/hold/stop recommendation only if the data supports it.
