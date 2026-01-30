# Claude CCB Skills

Claude Code Bridge (CCB) multi-AI collaboration toolkit for Claude Code.

## Overview

This skill collection enables multi-AI collaboration workflows, allowing Claude Code to delegate tasks to other AI assistants (Codex, Gemini, OpenCode, iFlow, Kimi, Qwen, DeepSeek, Droid) running in separate terminal sessions.

## Skills Included

| Skill | Description |
|-------|-------------|
| `ask` | Generic async delegation to any provider |
| `cask` | Async delegation to Codex |
| `dask` | Async delegation to Droid |
| `dskask` | Async delegation to DeepSeek |
| `gask` | Async delegation to Gemini |
| `iask` | Async delegation to iFlow |
| `kask` | Async delegation to Kimi |
| `oask` | Async delegation to OpenCode |
| `qask` | Async delegation to Qwen |
| `pend` | Fetch latest provider replies |
| `ping` | Check provider connectivity |
| `ccb-launcher` | CCB environment management |
| `all-plan` | Multi-AI collaborative planning |
| `stem-modeling` | STEM academic modeling with distributed AI |

## Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

## Usage

After installation, you can use these skills in Claude Code:

```
/ask gemini "analyze this code"
/cask "review this PR"
/ping codex
```

## Requirements

- Claude Code CLI
- WezTerm or tmux for multi-session management
- Respective AI CLI tools installed (codex, gemini-cli, etc.)

## License

MIT License - see [LICENSE](LICENSE) for details.
