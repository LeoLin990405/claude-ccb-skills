<h1 align="center">Claude CCB Skills</h1>

<p align="center">
  <strong>Multi-AI Coordination Toolkit for Claude Code</strong><br>
  <em>Route tasks to 9 AI providers, orchestrate parallel workflows, synthesize results</em>
</p>

<p align="center">
  <a href="https://github.com/LeoLin990405/claude-ccb-skills/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/LeoLin990405/claude-ccb-skills" alt="License">
  </a>
  <a href="https://github.com/LeoLin990405/claude-ccb-skills/stargazers">
    <img src="https://img.shields.io/github/stars/LeoLin990405/claude-ccb-skills" alt="Stars">
  </a>
  <a href="https://github.com/LeoLin990405/claude-ccb-skills/issues">
    <img src="https://img.shields.io/github/issues/LeoLin990405/claude-ccb-skills" alt="Issues">
  </a>
  <img src="https://img.shields.io/badge/Claude%20Code-Skill-8A2BE2?logo=anthropic&logoColor=white" alt="Claude Code Skill">
</p>

<p align="center">
  <a href="#features">Features</a> &middot;
  <a href="#quick-start">Quick Start</a> &middot;
  <a href="#skills-reference">Skills Reference</a> &middot;
  <a href="#orchestration-patterns">Patterns</a> &middot;
  <a href="#contributing">Contributing</a>
</p>

---

## Features

| Feature | Description |
|---------|-------------|
| **9 AI Providers** | Delegate tasks to Codex, Gemini, OpenCode, DeepSeek, iFlow, Kimi, Qwen, Droid, or any provider by name |
| **Async Delegation** | Non-blocking task submission via Gateway API with automatic result retrieval |
| **4 Orchestration Patterns** | Parallel fan-out, sequential pipeline, consensus voting, specialist routing |
| **3 Workflow Templates** | Ready-to-use templates for parallel review, consensus decisions, and research delegation |
| **Provider Monitoring** | Ping connectivity checks and pending-reply fetching |
| **Auto-Routing** | Router SKILL.md automatically selects the best provider based on task type |
| **Bilingual** | Full English and Chinese documentation |

---

## Quick Start

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### Usage

```bash
# Direct provider delegation
/gask "analyze this codebase"
/cask "review this PR"
/dskask "solve this algorithm"

# Monitor results
/pend gemini
/ping codex

# Multi-AI workflows
/all-plan          # Collaborative planning across providers
/stem-modeling     # STEM academic modeling
/ccb-launcher      # CCB environment management
```

The toolkit auto-routes based on your request:

| Request | Routed To |
|---------|-----------|
| "Review this code with Gemini and Codex" | Parallel fan-out + parallel-review template |
| "Get opinions on this architecture" | Consensus-decision template |
| "Ask DeepSeek to solve this algorithm" | `/dskask` |

---

## Skills Reference

### Delegation (9 providers)

| Provider | Skill | Command | Best For |
|----------|-------|---------|----------|
| Codex | [cask](skills/cask/SKILL.md) | `/cask <msg>` | Code generation, refactoring, PR review |
| Gemini | [gask](skills/gask/SKILL.md) | `/gask <msg>` | Long-context analysis, research, multimodal |
| OpenCode | [oask](skills/oask/SKILL.md) | `/oask <msg>` | Code analysis, debugging, architecture |
| DeepSeek | [dskask](skills/dskask/SKILL.md) | `/dskask <msg>` | Reasoning, math, algorithms |
| iFlow | [iask](skills/iask/SKILL.md) | `/iask <msg>` | Workflow automation, integrations |
| Kimi | [kask](skills/kask/SKILL.md) | `/kask <msg>` | Long documents, Chinese-language tasks |
| Qwen | [qask](skills/qask/SKILL.md) | `/qask <msg>` | Multilingual, general-purpose analysis |
| Droid | [dask](skills/dask/SKILL.md) | `/dask <msg>` | Mobile/Android development |
| Generic | [ask](skills/ask/SKILL.md) | `/ask <provider> <msg>` | Any provider by name |

### Monitoring

| Skill | Command | Description |
|-------|---------|-------------|
| [pend](skills/pend/SKILL.md) | `/pend <provider>` | Fetch latest reply from a provider |
| [ping](skills/ping/SKILL.md) | `/ping <provider>` | Check provider connectivity |

### Workflows

| Skill | Command | Description |
|-------|---------|-------------|
| [all-plan](skills/all-plan/SKILL.md) | `/all-plan` | Multi-AI collaborative planning |
| [stem-modeling](skills/stem-modeling/SKILL.md) | `/stem-modeling` | STEM academic modeling |
| [ccb-launcher](skills/ccb-launcher/SKILL.md) | `/ccb-launcher` | CCB environment management |

---

## Orchestration Patterns

| Pattern | When to Use |
|---------|-------------|
| **Parallel Fan-Out** | Same task to N providers, synthesize results |
| **Sequential Pipeline** | Chain providers: output of one feeds the next |
| **Consensus Voting** | Multiple providers vote on a decision |
| **Specialist Routing** | Route sub-tasks to the best-fit provider |

---

## Project Structure

```
claude-ccb-skills/
├── SKILL.md                          # Root skill index
├── README.md                         # This file
├── LICENSE                           # MIT License
├── CONTRIBUTING.md                   # Contribution guidelines
├── CHANGELOG.md                      # Release history
├── .github/
│   ├── workflows/
│   │   └── claude-review.yml         # Claude Code review action
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.yml            # Bug report template
│   │   ├── feature_request.yml       # Feature request template
│   │   └── config.yml                # Issue template config
│   └── PULL_REQUEST_TEMPLATE.md      # PR template
└── skills/
    ├── ask/SKILL.md                  # Generic async delegation
    ├── cask/SKILL.md                 # Codex delegation
    ├── dask/SKILL.md                 # Droid delegation
    ├── dskask/SKILL.md               # DeepSeek delegation
    ├── gask/SKILL.md                 # Gemini delegation
    ├── iask/SKILL.md                 # iFlow delegation
    ├── kask/SKILL.md                 # Kimi delegation
    ├── oask/SKILL.md                 # OpenCode delegation
    ├── qask/SKILL.md                 # Qwen delegation
    ├── pend/SKILL.md                 # Fetch provider replies
    ├── ping/SKILL.md                 # Check provider connectivity
    ├── all-plan/                     # Multi-AI collaborative planning
    │   ├── SKILL.md
    │   └── references/flow.md
    ├── ccb-launcher/SKILL.md         # CCB environment management
    └── stem-modeling/                # STEM academic modeling
        ├── SKILL.md
        └── references/template.md
```

---

## Contributing

Contributions are welcome! Please read the [Contributing Guide](CONTRIBUTING.md) before submitting a pull request.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">
  <sub>Built with collaboration between human and AI</sub>
</p>
