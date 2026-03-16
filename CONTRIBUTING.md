# Contributing to Claude CCB Skills

Thank you for your interest in contributing! This guide will help you get started.

## Getting Started

1. **Fork** the repository on GitHub.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/<your-username>/claude-ccb-skills.git
   cd claude-ccb-skills
   ```
3. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/my-new-skill
   ```

## Adding a New Skill

Each skill lives in its own directory under `skills/` and must contain a `SKILL.md` file.

### SKILL.md Format

```yaml
---
name: skill-name
description: Brief description of what the skill does
triggers:
  - /command-name
---

# Skill Name

Full instructions for Claude Code to follow when this skill is invoked.
```

### Checklist for New Skills

- [ ] Created `skills/<name>/SKILL.md` with proper frontmatter
- [ ] Added the skill to the root `SKILL.md` index
- [ ] Updated `README.md` with the new skill in the appropriate table
- [ ] Tested the skill locally with Claude Code

## Modifying Existing Skills

- Keep changes focused and well-scoped.
- Update any affected documentation (README, SKILL.md index).
- Test your changes locally before submitting.

## Pull Request Process

1. Ensure your branch is up to date with `main`.
2. Fill out the pull request template completely.
3. Link any related issues.
4. Wait for review -- a maintainer will review your PR.

## Code of Conduct

- Be respectful and constructive.
- Focus on the technical merits of contributions.
- Help maintain a welcoming environment for all contributors.

## Reporting Issues

- Use the **Bug Report** template for bugs.
- Use the **Feature Request** template for new ideas.
- Provide as much context as possible.

## Questions?

Open a [discussion](https://github.com/LeoLin990405/claude-ccb-skills/issues) or reach out to the maintainers.
