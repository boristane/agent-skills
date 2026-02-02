# Agent Skills

A collection of skills for AI coding agents. Skills are packaged instructions and scripts that extend agent capabilities. Works with Claude Code, AdaL, and other AI coding agents.

Skills follow the [Agent Skills](https://agentskills.io/) format.

## Available Skills

### logging-best-practices

Logging best practices focused on wide events (canonical log lines). Contains guidelines for effective logging that enables powerful debugging and analytics.

**Use when:**
- Writing or reviewing logging code
- Adding console.log, logger.info, or similar
- Designing logging strategy for new services
- Setting up logging infrastructure

**Key concepts:**
- Wide Events (Critical) - One context-rich event per request per service
- High Cardinality & Dimensionality (Critical) - Many fields, unique identifiers
- Business Context (Critical) - User subscription, cart value, feature flags
- Environment Context (Critical) - Commit hash, version, region, instance ID
- Single Logger (High) - One logger instance, configured at startup
- Middleware Pattern (High) - Infrastructure in middleware, business context in handlers

**References:**
- [Logging Sucks](https://loggingsucks.com)
- [Observability Wide Events 101](https://boristane.com/blog/observability-wide-events-101/)
- [Stripe - Canonical Log Lines](https://stripe.com/blog/canonical-log-lines)

## Installation

```bash
npx add-skill boristane/agent-skills
```

## Usage

Skills are automatically available once installed. The agent will use them when relevant tasks are detected.

**Examples:**
```
Add logging to this endpoint
```
```
Review my logging code
```
```
Help me set up logging for this service
```

## Skill Structure

Each skill contains:
- `SKILL.md` - Instructions for the agent
- `rules/` - Individual guideline files
- `metadata.json` - Version and references
