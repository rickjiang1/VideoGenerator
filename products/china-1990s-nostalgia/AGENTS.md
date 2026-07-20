# China 1990s Nostalgia Product Instructions

## Product identity

Product key: `china-1990s-nostalgia`

This product creates original, AI-generated nostalgic videos inspired by ordinary life in China during the 1990s.

This is one product inside the multi-product `VideoGenerator` repository. Do not apply its creative rules, characters, locations, historical constraints, or tool decisions to another product.

## Current phase

MVP planning and workflow validation.

Do not treat a proposed duration, shot count, character count, geographic setting, exact year, aspect ratio, or release schedule as confirmed unless Rick explicitly approves it and the decision is recorded in `PRODUCT.md`.

## Confirmed MVP direction

- Start with an MVP before planning or generating a full season.
- Do not use narration, voice-over, or character dialogue in the current MVP.
- Use simple background music selected by Rick.
- Keep all generated images, videos, audio, music, renders, and downloads outside Git.
- Keep text-based planning, scripts, shot lists, prompts, manifests, and metadata in Git only after approval.

## Current tool responsibilities

The intended MVP workflow is:

- ChatGPT/Codex: discussion, research, writing, shot planning, prompts, documentation, and review.
- Google Flow: character references, locations, visual references, and storyboard or keyframe images.
- VEO Automation: Flow-side batch assistance when needed.
- Grok Imagine: image-to-video and other video generation.
- Grok Automation: batch submission, retry, download, and organization for Grok Imagine.
- Local editing software: sequencing, background music, titles, and final export.

These tool choices must be validated with a small test before committing to a full production batch.

## Historical and visual integrity

Before generation, lock the intended year, region, city type, household context, and visual style.

Prevent accidental mixing of the 1980s, 1990s, and 2000s.

Review every applicable shot for anachronisms such as:

- smartphones and modern mobile devices
- QR codes
- modern LED signage and lighting
- contemporary vehicles
- contemporary clothing, packaging, furniture, and appliances
- modern construction details and street infrastructure
- incorrect brand, media, or technology timelines

Separate verified historical detail from fictional story content.

Do not claim that a fictional AI-generated scene is authentic archival footage.

## Character and shot continuity

Once approved, treat character identity, age, face, hairstyle, body proportions, wardrobe, locations, props, time of day, and color language as locked references.

Use stable identifiers for products, episodes, characters, locations, props, shots, and generated variants.

Keep each generated video shot focused on one principal action.

Use reference images and filenames consistently across Flow, Grok, manifests, and review notes.

## Agent routing

The repository root `AGENTS.md` controls agent routing.

If Rick does not explicitly request a specialist agent, the main agent must handle the request without spawning subagents.

Product work may use the repository specialist agents only after Rick explicitly names or approves them.

## Approval gates

Rick's explicit approval is required before:

- moving from discussion into file implementation
- recording a proposed creative decision as confirmed
- generating a batch of media
- purchasing or enabling a paid generation plan
- committing or pushing product changes
- uploading or publishing the MVP

When a decision is still open, record it as open rather than guessing.
