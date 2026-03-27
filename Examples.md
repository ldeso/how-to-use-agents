# Examples

## Aerodrome Dashboard

- Repository: https://github.com/ldeso/aerodrome
- Workflow: Claude Code + GitHub

### Description

Claude Code created two scripts in TypeScript: one fetches Aerodrome data from
the blockchain, and one builds an HTML dashboard from the data. A GitHub Actions
workflow runs these scripts every week, and at every code change pushed to the
repository. Secret API keys that are required to access blockchain data
providers are stored as "secrets" in the repository settings on GitHub.

### Learnings

- Claude Code worked best when I gave it well-defined and separated tasks
- This led to a program architecture with one separate file for each action
- Claude Code preferred to add code rather than to reuse what was already there
- It was good at refactoring the code, when specifically asked for it

### Recommendations

- Ask agents to create simple deterministic scripts
- Use GitHub Actions to schedule tasks!
