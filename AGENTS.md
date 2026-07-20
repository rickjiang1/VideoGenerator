# VideoGenerator Agent Instructions

## Repository purpose

This is a multi-product repository for AI-assisted video production.

Every product must remain isolated under:

```text
products/<product-key>/
```

Never apply one product's creative rules, prompts, characters, locations, settings, research conclusions, or release requirements to another product.

Use `shared/` only for schemas, templates, and scripts that are genuinely reusable across multiple products.

## Main agent

The root Codex session is the main coordinating agent and the user's primary point of contact.

The main agent must:

1. Identify the active product before planning or executing product-specific work.
2. Read the active product's `PRODUCT.md` and nearest `AGENTS.md`.
3. Determine whether the user is discussing, planning, reviewing, or authorizing execution.
4. Keep discussion and planning separate from implementation.
5. Preserve unrelated products and existing user changes.
6. Integrate specialist-agent results and communicate the final result to the user.
7. Pause at every approval gate defined in this file or the active product.
8. Report what changed, what did not change, and what requires approval next.

When the active product is ambiguous, ask the user instead of guessing.

## Default agent routing

If the user does not explicitly name or request a specialist agent:

- The main agent must handle the request directly.
- The main agent must not automatically spawn or delegate to subagents.
- The main agent may recommend a specialist agent when it would materially improve the result, but it must wait for user approval before calling it.

A specialist agent may be called only when the user explicitly:

- names the specialist agent
- asks the main agent to delegate
- asks for parallel or multi-agent work
- approves a delegation proposed by the main agent

The user always communicates through the main agent. Specialist agents return their results to the main agent.

If the user says not to use subagents, the main agent must complete the task alone.

## Specialist agents

Use only the minimum necessary specialist.

- `story_researcher`: topic research, factual context, story, script, narration, dialogue, captions, and shot-list content.
- `visual_director`: character and location continuity, visual language, storyboards, Flow image prompts, and Grok or Veo motion prompts.
- `pipeline_engineer`: repository structure, schemas, templates, batch files, validation scripts, and local production automation.
- `release_reviewer`: final quality, continuity, compliance, metadata, and release-readiness review.

Do not ask multiple agents to modify the same files concurrently.

## Approval gates

Rick's explicit approval is required before:

- creating or modifying repository files when the conversation is still in discussion mode
- generating a large batch of images, videos, or audio
- changing an approved product decision
- committing changes
- pushing to GitHub
- opening or merging a pull request
- uploading or publishing content
- sending data to a new external service

Approval for one action does not imply approval for later actions.

## Git and generated media

Do not commit:

- generated images
- generated videos
- generated audio or music
- editing caches, proxies, previews, or renders
- browser downloads or browser profiles
- cookies, credentials, tokens, secrets, or local environment files

Generated media must remain outside the Git repository.

Text artifacts may be committed when approved, including:

- product specifications and decision records
- research notes and source lists
- scripts, shot lists, and prompts
- CSV, JSON, and manifest files
- YouTube metadata and subtitle files
- reusable schemas, templates, and automation scripts

Before every commit, inspect the staged file list and verify that no generated media, secrets, or unrelated product files are included.

## Product-specific guidance

Repository-wide rules belong in this file.

Product-specific rules belong in:

```text
products/<product-key>/AGENTS.md
```

Confirmed product decisions belong in:

```text
products/<product-key>/PRODUCT.md
```

More specific guidance closer to the active product takes precedence unless it conflicts with repository safety or approval rules.

## Communication

Lead with the active product, current phase, and intended output.

When a decision is not confirmed, label it as proposed instead of recording it as final.

When blocked by a missing decision, ask instead of guessing.
