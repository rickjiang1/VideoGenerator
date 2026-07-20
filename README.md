# VideoGenerator

A multi-product repository for AI-assisted video production workflows.

Each video product lives in its own directory under `products/<product-key>/`. Product-specific creative rules, scripts, prompts, and release requirements must remain isolated from other products.

## Current products

- `products/china-1990s-nostalgia/` — an MVP for AI-generated nostalgic videos inspired by everyday life in China during the 1990s.

## Repository layout

```text
VideoGenerator/
├── AGENTS.md
├── .codex/
│   └── agents/
├── products/
└── shared/
```

- `AGENTS.md` defines repository-wide coordination and safety rules.
- `.codex/agents/` contains reusable specialist agent definitions.
- `products/` contains isolated product specifications and text-based production artifacts.
- `shared/` is reserved for schemas, templates, and scripts that are genuinely reusable across products.

## Generated media policy

Generated images, videos, audio, music, renders, browser downloads, and other large binary outputs must not be committed to this repository. Keep generated media in a separate local asset directory.

Text artifacts such as product decisions, scripts, shot lists, prompts, metadata, manifests, and subtitles may be versioned in Git.

## Change policy

Do not commit, push, open a pull request, upload, or publish content unless Rick explicitly approves the action.
