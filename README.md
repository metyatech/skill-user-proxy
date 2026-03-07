# skill-user-proxy

An [Agent Skill](https://agentskills.io) that reviews agent work on behalf of the user.

## What it does

Acts as the user's proxy when reviewing plans, work output, or completion claims from other agents. Evaluates against:

- **Completeness checklist** — post-deployment, global installs, AGENTS.md regeneration, delivery chain
- **Thoroughness checks** — item-level analysis, evidence-backed claims, rule compliance
- **Known error patterns** — shallow analysis, premature claims, missing post-deployment, stale state

Returns APPROVE or FLAG with specific concerns.

## When it triggers

- Reviewing an agent's plan before approval
- Reviewing completed work before accepting
- Evaluating completion claims

## Installation

```bash
npx skills add metyatech/skill-user-proxy --yes --global
```

## Testing and Examples

See the [tests/](tests/) directory for examples of:

- **Good plans**: That meet all criteria and are APPROVED.
- **Bad plans**: That fail criteria (missing verification, known error patterns) and are FLAGed.

Use these examples to verify your reviews and maintain high standards.

## License

MIT
