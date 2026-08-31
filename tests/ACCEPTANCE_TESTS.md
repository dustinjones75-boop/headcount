# ChatGPT Edition Acceptance Tests

The edition is ready only if these behaviors hold consistently.

## Routing
- Simple drafting requests use one writing specialist rather than over-routing.
- Paid-search diagnosis selects paid-advertising as primary and adds analytics/CRO/economics only when relevant.
- Website redesign selects UX/interface skills rather than generic marketing strategy.
- Automation design selects ai-workflow-architect; an existing broken flow selects systematic-debugging.
- Business growth questions distinguish constraint diagnosis from campaign execution.
- Uncertain strategic choices invoke scenario-planning only when the uncertainty can materially change the action.
- Travel-business questions use travel-advisor-strategist; simple consumer travel facts do not.

## Tool grounding
- Questions about a connected GitHub repo inspect repository evidence before diagnosing code.
- Questions dependent on current fares, availability, policies, news, laws, competitors, or platform behavior use fresh sources.
- Questions dependent on the user's connected/private data retrieve that data first when available.
- The answer never claims a source, connector, file, campaign, or repository was checked when it was not.

## Synthesis
- One primary specialist is always identifiable internally.
- No more than three supporting specialists are used by default.
- The response is a single integrated recommendation, not separate agent reports.
- Disagreement is resolved before the user sees the answer.

## Review
- Expensive, irreversible, high-risk, or public factual recommendations receive a reviewer pass.
- Reviewer objections are incorporated only when material.
- Uncertainty and missing evidence are stated instead of filled with invented facts.

## Quality
- Recommendations are prioritized.
- The highest-value next action is clear.
- Important assumptions are named.
- Success has a metric, verification step, or decision trigger where applicable.
- The system can say that no change is needed when evidence supports that conclusion.

## Regression prompts
Use `tests/ROUTING_TESTS.md` for scenario-level regression tests. Add a regression case whenever real use exposes a routing mistake.