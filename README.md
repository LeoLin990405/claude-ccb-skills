# CCB Skills

This repository is public and unarchived. It is kept as a maintenance mirror and migration reference for the CCB skills.

The active canonical destination is:
- https://github.com/LeoLin990405/claude-code-skills

The canonical orchestration entry now lives under:
- https://github.com/LeoLin990405/claude-code-skills/tree/main/ai-collaboration/ccb-unified

Legacy installed skill names have been preserved in the monorepo as compatibility shims under:
- https://github.com/LeoLin990405/claude-code-skills/tree/main/ai-collaboration

Direct mapping summary:
- `claude-ccb-skills/skills/ask` -> `claude-code-skills/ai-collaboration/ask`
- `claude-ccb-skills/skills/all-plan` -> `claude-code-skills/ai-collaboration/all-plan`
- `claude-ccb-skills/skills/{cask,dask,dskask,gask,iask,kask,oask,qask}` -> `claude-code-skills/ai-collaboration/{cask,dask,dskask,gask,iask,kask,oask,qask}`
- `claude-ccb-skills/skills/{pend,ping}` -> `claude-code-skills/ai-collaboration/{pend,ping}`
- `claude-ccb-skills/skills/ccb-launcher` -> `claude-code-skills/ai-collaboration/ccb-launcher`
- `claude-ccb-skills/skills/stem-modeling` -> `claude-code-skills/research/stem-modeling`
- integrated orchestration behavior -> `claude-code-skills/ai-collaboration/ccb-unified`

## Maintenance

Use `claude-code-skills` for new features, routing updates, and installation flow changes. This repository remains available for historical source context, issue triage, and small compatibility fixes when needed.