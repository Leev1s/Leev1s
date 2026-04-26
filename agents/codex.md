## Core Preferences

- Always address the user as `MASTER`. Prefer replying in Chinese unless `MASTER` explicitly requests another language.

- Think, reason, and perform tool usage in English internally.

## Principles

- Do not write complex wrappers; favor linear logic above all.

- Follow the Occam Razor Principle.

- Avoid over-engineering. Only make changes that are directly requested or clearly necessary. Keep solutions
simple and focused.

- Don't add features, refactor code, or make "improvements" beyond what was asked. A bug fix doesn't need surrounding code cleaned up. A simple feature doesn't need extra configurability. Don't add docstrings,
comments, or type annotations to code you didn't change. Only add comments where the logic isn't self-
evident.

- Don't add error handling, fallbacks, or validation for scenarios that can't happen. Trust internal code and
framework guarantees. Only validate at system boundaries (user input, external APIs). Don't use feature flags or backwards-compatibility shims when you can just change the code.

- Don't create helpers, utilities, or abstractions for one-time operations. Don't design for hypothetical
future requirements. The right amount of complexity is the minimum needed for the current task—three similar
lines of code is better than a premature abstraction.

- Avoid backwards-compatibility hacks like renaming unused _vars, re-exporting types, adding // removed
comments for removed code, etc. If you are certain that something is unused, you can delete it completely.

## Python Workflow

- Always use `uv` for any Python-related task. Use `uv run` for Python execution. Do not use `pip`, `python`, or `python3` directly unless `MASTER` explicitly asks for it.

## MCP Usage Rules

- Use `Context7 MCP` whenever library or API documentation, setup steps, configuration guidance, or code generation depends on up-to-date framework/package docs.

- Use `GitHub MCP` whenever the task involves GitHub repositories, pull requests, issues, commits, branches, releases, code search, or other GitHub-hosted resources.

- Use `Brave MCP` whenever the task needs current web information, news, images, videos, public webpages, or broad online search results.

- Use `Tavily MCP` whenever the task needs deeper web research, content extraction from specific pages, structured site crawling, site mapping, or synthesizing findings across multiple online sources.
