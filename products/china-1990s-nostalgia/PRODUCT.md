# China 1990s Nostalgia

## Product record

- Product key: `china-1990s-nostalgia`
- Owner: Rick
- Repository: `rickjiang1/VideoGenerator`
- Status: MVP planning
- Primary theme: nostalgic stories and moments inspired by life in China during the 1990s
- Primary distribution target: YouTube

This file is the source of truth for confirmed product decisions. Proposed ideas must remain in the open-decisions section until Rick explicitly approves them.

## Confirmed decisions

### Repository and product boundaries

- This is one product inside a repository that will contain multiple products.
- Product-specific files belong under `products/china-1990s-nostalgia/`.
- Rules and creative decisions from this product must not leak into another product.
- Generated images, videos, audio, music, renders, and browser downloads must not be committed to Git.

### Working model

- Discussion and product decisions may happen in ChatGPT Work mode.
- Local ChatGPT/Codex is the preferred execution environment for repository work, local files, browser-assisted production, and generated media.
- GitHub is used for approved text artifacts, schemas, templates, scripts, prompts, manifests, and documentation.
- The main agent is the default conversation partner.
- Specialist agents must not be called unless Rick explicitly requests or approves delegation.

### MVP scope

- Build and validate an MVP before expanding into a full season.
- The current MVP does not need narration, voice-over, or character dialogue.
- The MVP may use simple background music selected by Rick.
- Music selection and usage rights remain Rick's responsibility unless a later task explicitly adds a music review.

### Current intended tool roles

- ChatGPT/Codex: topic discussion, research, scripts, shot lists, prompts, documentation, SEO text, and review.
- Google Flow: fixed characters, locations, storyboard images, and keyframes.
- VEO Automation: batch assistance on the Google Flow side when useful.
- Grok Imagine: video generation.
- Grok Automation: batch video submission, retry, download, and organization.
- Local editing software: assembly, background music, titles, and export.

The final video generator must be selected through a small MVP test rather than assumed to be superior without evidence.

## Open decisions

The following decisions are not yet approved:

- the first MVP story or topic
- the exact year within the 1990s
- the region, city type, and household context
- target duration
- shot count and average shot duration
- aspect ratio and export resolution
- number and identity of recurring characters
- recurring locations and props
- realistic, illustrated, cinematic, or other visual style
- whether the Grok watermark is acceptable for a published YouTube video
- whether Grok Free, SuperGrok, or another usage option is needed
- whether Grok or Veo will be the final MVP video generator
- local generated-media directory and backup strategy
- editing software
- exact background music and license
- MVP success and acceptance criteria
- YouTube channel, publishing cadence, and release date

## Current workflow hypothesis

This workflow is proposed for testing and is not yet an approved production batch:

1. Confirm the MVP topic and historical setting.
2. Create a short visual story without narration or dialogue.
3. Create and approve character and location references in Google Flow.
4. Generate and approve storyboard or keyframe images.
5. Test a small number of identical keyframes in Grok and Veo when comparison is useful.
6. Select the video generator based on identity consistency, motion quality, prompt adherence, artifacts, generation time, quota use, and watermark impact.
7. Generate only the approved MVP shots.
8. Assemble the selected clips locally with background music.
9. Review continuity, historical accuracy, technical quality, AI disclosure, and YouTube metadata.
10. Publish only after Rick's explicit approval.

## Decision log

### 2026-07-20

- Selected `rickjiang1/VideoGenerator` as the GitHub repository.
- Confirmed that the repository will host multiple distinct video products.
- Confirmed that generated image and video assets must stay outside Git.
- Confirmed the main-agent default and explicit specialist-agent routing.
- Confirmed four reusable specialist roles: story researcher, visual director, pipeline engineer, and release reviewer.
- Confirmed an MVP-first approach with no voice and simple background music selected by Rick.
