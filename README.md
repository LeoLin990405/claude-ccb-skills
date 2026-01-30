# Claude CCB Skills

[English](#english) | [中文](#中文)

---

## English

Claude Code Bridge (CCB) multi-AI collaboration toolkit for Claude Code.

### Overview

This skill collection enables multi-AI collaboration workflows, allowing Claude Code to delegate tasks to other AI assistants (Codex, Gemini, OpenCode, iFlow, Kimi, Qwen, DeepSeek, Droid) running in separate terminal sessions.

### Skills Included

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

### Installation

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### Usage

After installation, you can use these skills in Claude Code:

```
/ask gemini "analyze this code"
/cask "review this PR"
/ping codex
```

### Requirements

- Claude Code CLI
- WezTerm or tmux for multi-session management
- Respective AI CLI tools installed (codex, gemini-cli, etc.)

---

## 中文

Claude Code Bridge (CCB) 多 AI 协作工具集。

### 概述

此技能集支持多 AI 协作工作流，允许 Claude Code 将任务委托给在独立终端会话中运行的其他 AI 助手（Codex、Gemini、OpenCode、iFlow、Kimi、Qwen、DeepSeek、Droid）。

### 包含的技能

| 技能 | 描述 |
|------|------|
| `ask` | 通用异步委托 |
| `cask` | Codex 异步委托 |
| `dask` | Droid 异步委托 |
| `dskask` | DeepSeek 异步委托 |
| `gask` | Gemini 异步委托 |
| `iask` | iFlow 异步委托 |
| `kask` | Kimi 异步委托 |
| `oask` | OpenCode 异步委托 |
| `qask` | Qwen 异步委托 |
| `pend` | 获取 provider 回复 |
| `ping` | 检查 provider 连接 |
| `ccb-launcher` | CCB 环境管理 |
| `all-plan` | 多 AI 协作规划 |
| `stem-modeling` | STEM 学术建模 |

### 安装

```bash
cd ~/.claude/skills
git clone https://github.com/LeoLin990405/claude-ccb-skills.git
```

### 使用方法

安装后，可在 Claude Code 中使用：

```
/ask gemini "分析这段代码"
/cask "审查这个 PR"
/ping codex
```

### 依赖

- Claude Code CLI
- WezTerm 或 tmux（多会话管理）
- 相应的 AI CLI 工具（codex、gemini-cli 等）

---

## License

MIT License - see [LICENSE](LICENSE) for details.
