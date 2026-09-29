# Repository Guidelines

## Project Structure & Module Organization

This repository is a documentation-first specification for AI-generated interactive product prototypes; it has no application source tree. `SKILL.md` holds cross-end rules: core principles, workflow, page states, shared component rules, interaction flow, the acceptance checklist, and pointers to the end references. End-specific rules live under `references/`: `b-end.md` (desktop web / SaaS) and `c-end.md` (mobile, tablet, mini programs, apps), while `design-tokens.md` defines default colors, typography, spacing, and visual treatments shared by all ends. `README.md` explains the repository and how to invoke the specification. Keep every rule in exactly one place: end-specific rules in the matching reference, cross-end rules in `SKILL.md`, and pointers instead of restatements elsewhere. Do not add implementation code.

## Build, Test, and Development Commands

There is no build system, package manifest, or automated test command in this repository. Edit the Markdown sources directly and inspect the rendered documents in a Markdown preview. For changes affecting prototype requirements, check that the workflow, design tokens, acceptance checklist, and the matching end reference agree. When reviewing a generated prototype, open it in a browser and exercise its interactions and required empty, loading, success, and failure states.

## Writing Style & Conventions

Use Markdown headings and concise, actionable bullets. Keep the user-facing specification in Chinese, consistent with `SKILL.md` and `references/design-tokens.md`; use English where needed for technical terms. Preserve existing terminology such as “标注层”, “空态”, and “失败/异常态”. Put visual defaults in `references/design-tokens.md`, cross-end workflow and acceptance rules in `SKILL.md`, and end-specific rules (carrier, layout baselines, component defaults, delivery notes) in `references/b-end.md` or `references/c-end.md`; `SKILL.md` should point to the matching reference rather than restate it. Update `README.md` when repository usage or structure changes. Do not introduce unsupported tools, frameworks, or commands as project requirements.

## Validation Guidelines

Before submitting documentation changes, review the rendered Markdown, verify relative file references, and check for contradictory or duplicated requirements. For prototype-spec changes, walk through the applicable items in the acceptance checklist in `SKILL.md`; no test framework or coverage target is configured here.

## Commit & Pull Request Guidelines

The short history includes subjects like `Update README.md` and `产品原型规范初版`; no formal commit convention is established. Use a brief imperative subject that names the change. PRs should summarize the purpose and affected guidance files, note any rule changes, and include screenshots only when a rendered prototype or visual example changes. Link a related issue when one exists.
