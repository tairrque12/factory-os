# Factory OS

An AI-native software factory that builds and operates Option 5 businesses.

## North star
One person. One factory. A portfolio of agent-operated businesses. Spec to production with zero human touches in between.

## How the factory works
1. RIQ writes a spec (outcome + acceptance criteria)
2. Spec becomes a Linear ticket
3. Claude Code picks up the ticket autonomously
4. Agent writes code + tests, iterates until passing
5. PR opened — Bugbot reviews — CI runs 4 gates
6. CD deploys to staging — smoke tests — production
7. GBrain records everything — factory gets smarter

## Stack
- Runtime: Claude Code (async) + Cursor (sync)
- Memory: GBrain
- Agent roles: GStack (53 skills)
- CI/CD: GitHub Actions
- Hosting: Railway
- Ticketing: Linear
- Communication: Slack
- Monitoring: Sentry + PostHog
- Payments: Stripe

## Setup
Copy .env.example to .env and fill in your values.

## Agent rules
Every agent reads CLAUDE.md before touching this codebase. No exceptions.

## Structure
- .github/workflows — CI, CD, nightly maintenance
- src — application code
- tests/unit, integration, acceptance
- skills — GBrain + GStack agent skills
- docs — documentation
- CLAUDE.md — agent ruleset

## Departments
- Engineering: locked and operational
- Research: in progress
- Product/Design: planned
- Marketing/Sales: planned
