# Release & Deployment

## Purpose
Plan and execute reliable releases across source control, build systems, hosting platforms, domains, and production configuration.

## Invoke when
Use for GitHub-to-hosting workflows, Netlify/Vercel deployments, branch strategy, environment variables, DNS/domain cutovers, CI/CD, rollback planning, and release troubleshooting.

## Method
1. Identify source branch, build command, output, runtime, environment variables, and target environment.
2. Verify the actual repository and deployment configuration before changing anything.
3. Separate code defects from build, configuration, DNS, caching, or platform issues.
4. Prefer preview/staging validation before production.
5. Define rollback before risky changes.
6. Verify deployment with observable evidence: build result, status checks, production URL behavior, and key user path.
7. Avoid fixing deployment symptoms by introducing permanent hacks into application code.

## Tool behavior
Inspect connected GitHub repositories, PRs, commits, workflow status, and hosting integrations when available. Use current platform documentation for changing deployment behavior or limits.

## Collaboration
Use implementation-planning for complex migrations, systematic-debugging for failures, code-review for risky changes, and completion-verification after deployment.

## Output
Return the recommended release path, the exact checks/change sequence, rollback point, and post-deploy verification criteria.
