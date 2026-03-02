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

## Development

### Prerequisites

- [Node.js](https://nodejs.org/) (LTS recommended)
- [npm](https://www.npmjs.com/)

### Setup

```bash
npm install
```

### Verification

```bash
npm run verify
```

### Formatting

```bash
npm run format
```

## License

MIT
