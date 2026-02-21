# CLAUDE.md — superpowers

## What This Is

**Superpowers** is an external open-source Claude Code plugin (by Jesse Vincent / obra). It provides a structured skills library for coding agent workflows: TDD, systematic debugging, brainstorming, plan execution, and subagent-driven development.

**This is NOT Serge's code.** It's an installed plugin from the marketplace. Treat it like a dependency.

## When Working Here

- You are likely debugging a skill, adding a custom skill, or investigating plugin behavior
- Skills live in `skills/<skill-name>/SKILL.md` — these are the core logic files
- Plugin config: `.claude-plugin/plugin.json` (version, metadata)
- Hook config: `hooks/hooks.json` (SessionStart automation)

## Skills Available

| Skill | Purpose |
|-------|---------|
| brainstorming | Socratic design refinement before coding |
| writing-plans | Detailed implementation plans |
| executing-plans | Batch execution with checkpoints |
| subagent-driven-development | Fast parallel iteration |
| test-driven-development | RED-GREEN-REFACTOR cycle |
| systematic-debugging | 4-phase root cause process |
| receiving-code-review | Technical feedback response |
| requesting-code-review | Pre-review checklist |
| using-git-worktrees | Isolated parallel branches |
| finishing-a-development-branch | Merge/PR decision |
| dispatching-parallel-agents | Concurrent subagent workflows |
| writing-skills | How to create new skills |
| using-superpowers | Introduction to the system |
| verification-before-completion | Verify fixes are real |

## Contributing / Customization

To add a skill: follow `skills/writing-skills/SKILL.md`.
To update: `/plugin update superpowers` in Claude Code.

## Issue Resolution

Before solving problems: `grep -i "keyword" ~/Documents/Documentation/System/ISSUES_KNOWLEDGE_BASE.md`
