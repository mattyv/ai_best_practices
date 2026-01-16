# AI-Assisted Development Best Practices

Practical guidelines for working effectively with AI coding tools (Claude Code, Cursor, Copilot, etc.) without letting them undermine your codebase.

## Contents

- **[Best Practices](jason_turner_ai_tool_best_practices.md)** — Comprehensive guide covering mental models, workflow, and 12 best practices for AI-assisted development
- **[Project Requirements Checklist](ai_project_requirements.md)** — Minimum requirements your project needs before using AI tools effectively

## The Core Problem

AI coding assistants are powerful but will:
- Disable your warnings and static analysis to make code "work"
- Skip tests or modify them to match buggy behavior
- Forget instructions after context compaction
- Take shortcuts that circumvent your safeguards

These guidelines help you get the productivity benefits while maintaining code quality.

## Quick Start

1. Set up your project with the [minimum requirements](ai_project_requirements.md)
2. Create a `CLAUDE.md` with build instructions and coding standards
3. Enable warnings-as-errors (non-negotiable)
4. Get test coverage before letting AI refactor anything
5. Review every change like it's a PR from a stranger

## Key Principles

- **Don't vibe** — Always verify AI work; never trust blindly
- **More than autocomplete, less than autonomous** — Give meaningful chunks of work, but stay engaged
- **It's an intern with a short attention span** — Fast, well-read, but easily distracted and needs constant reminding
- **Positive directives only** — "Always run all tests" not "Never skip tests"

## Attribution

Based on Jason Turner's presentation "Best Practices for AI Tool Use" with additional commentary from Claude and GPT included in the original material.

- Jason Turner: [@lefticus](https://twitter.com/lefticus) | [C++ Weekly](https://www.youtube.com/@cppweekly) | [cppbestpractices.com](https://cppbestpractices.com)

## License

This is a distillation of publicly presented material. Original content copyright Jason Turner.
