# Routing Test Scenarios

These examples are acceptance tests for the ChatGPT router. The goal is correct specialist selection without unnecessary fan-out.

| User request | Primary | Supporting | Reviewer? |
|---|---|---|---|
| My Google Ads get clicks but almost no leads. Figure out why. | paid-advertising | marketing-analytics, landing-page-cro | unit-economics if spend/scale decision |
| Review this cruise landing page and tell me what to change first. | landing-page-cro | travel-advisor-strategist, marketing-copywriting | no |
| Should I spend $500 more on this campaign? | unit-economics | paid-advertising, marketing-analytics | yes |
| Build a campaign for a resort with advisor-exclusive benefits. | travel-advisor-strategist | campaign-planner, paid-advertising, positioning-messaging | unit-economics if budget supplied |
| My mobile page is clipping content after a recent deploy. | systematic-debugging | release-and-deployment, completion-verification | no |
| Design a Make workflow to summarize flight data and email it. | ai-workflow-architect | implementation-planning, prompt-optimizer | no |
| Should this automation use an LLM or normal rules? | ai-workflow-architect | solution-architecture | no |
| Rewrite this email to a travel client. | marketing-copywriting | brand-voice if needed | no |
| Why did organic traffic fall? | seo-strategy | marketing-analytics | no |
| I want 100 destination pages for SEO. | programmatic-seo | seo-strategy, marketing-copywriting | yes if duplicate/thin-content risk is high |
| Research a company and pressure-test an investment-like business decision. | ai-research-analyst | ceo-advisor, scenario-planning | yes |
| Plan the technical implementation now that we chose the solution. | implementation-planning | completion-verification | no |

## Failure cases

The router fails if it:
- selects more than four specialists for a routine request;
- chooses a writing specialist as primary for a data-diagnosis problem;
- recommends campaign changes before checking available measurement evidence;
- treats a travel business request as only consumer travel research when commission, supplier benefits, or client conversion matter;
- declares a technical fix complete without a verification path;
- reports changing public facts without current research when current research is available.
