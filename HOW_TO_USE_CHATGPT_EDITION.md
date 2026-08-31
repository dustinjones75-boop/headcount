# How to Use the ChatGPT Edition

## What this is

This branch adapts Headcount's specialist organization for ChatGPT. It is not a Claude Code plugin and does not require slash commands. The value is the routing policy plus a curated set of specialist instruction files that can be loaded when relevant.

## Recommended operating pattern

1. Load or reference `CHATGPT_BOOTSTRAP.md` at the start of the workspace/session that will use this system.
2. The bootstrap points to `CHATGPT_ROUTER.md`, `TOOL_ROUTING.md`, and the curated skill roster.
3. For each request, choose one primary specialist and no more than three supporting specialists by default.
4. Read only the relevant `SKILL.md` files; do not stuff the whole repository into context.
5. Use connected/private data before answering data-dependent questions and fresh web research when public facts may have changed.
6. For consequential decisions or public factual claims, apply `CHATGPT_REVIEWER.md` before finalizing.
7. Return one integrated answer. The user should not have to reconcile separate agent reports.

## Practical ChatGPT prompt

When a ChatGPT environment can access this repository, a useful bootstrap instruction is:

> Use the ChatGPT edition in this repository. Read `CHATGPT_BOOTSTRAP.md`, route my request using `CHATGPT_ROUTER.md`, load only the relevant specialist skill files, follow `TOOL_ROUTING.md`, and apply the reviewer when required. Give me one integrated answer rather than separate specialist reports.

## Example routing

**Paid search underperforming:** paid-advertising + marketing-analytics + landing-page-cro + unit-economics.

**Website redesign:** ux-product-auditor + interface-redesign + landing-page-cro + positioning-and-messaging.

**Automation build:** ai-workflow-architect + solution-exploration + implementation-planning; systematic-debugging when repairing an existing flow.

**Travel campaign:** travel-advisor-strategist + marketing-campaign-planner + paid-advertising + unit-economics.

**Business decision:** ceo-advisor or business-growth-consultant, with scenario-planning and financial-modeling when uncertainty or economics are material.

## Direct specialist use

Routing is optional. A user can explicitly request a specialist by name, e.g. “Use the Landing Page CRO skill to audit this page.” Direct invocation should still follow tool-routing and evidence rules.

## Maintenance

Upstream Headcount can continue evolving independently. When pulling upstream changes, review rather than blindly overwriting ChatGPT-edition skills because these files intentionally include ChatGPT-specific tool behavior and routing conventions.

## License

This fork retains the upstream MIT license. Adapted material should continue to preserve applicable attribution and license terms.