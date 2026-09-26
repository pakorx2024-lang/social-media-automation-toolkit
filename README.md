# Social Media Automation Toolkit

Open-source toolkit for automating social media content creation, adaptation, translation, publishing and analytics with AI and n8n.

## What it does

**Source content → AI transformation → content validation → translation → human approval → publishing → analytics**

Built for creators, developers and small teams who want to automate repetitive social-media workflows while keeping editorial control.

## Main components

- **Claude / AI skills** — reusable content-generation and adaptation workflows.
- **n8n workflows** — orchestration for generation, translation, publishing and analytics.
- **Templates** — reusable formats for posts, carousels, short-form video and thumbnails.
- **Documentation** — setup and customization guides.
- **Examples** — generic examples that can be copied and adapted.

## Design principles

1. Keep credentials and personal data out of the repository.
2. Keep a human approval step before automated publishing.
3. Make workflows provider-agnostic where practical.
4. Separate reusable open-source components from private production infrastructure.
5. Make examples generic and reproducible.
6. Prefer structured outputs over fragile free-form text.

## Architecture

```
Source Content
      ↓
AI / Claude
      ↓
Hook / Script / Caption / CTA
      ↓
Content Validation
      ↓
Translation
      ↓
Human Approval
      ↓
Publishing
      ↓
Analytics
      ↺
```

## Repository structure

```
.
├── .claude/
│   └── skills/
├── .github/
│   └── ISSUE_TEMPLATE/
├── docs/
├── examples/
├── workflows/
│   └── n8n/
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
└── README.md
```

## Getting started

1. Install n8n.
2. Import a workflow from `workflows/n8n/`.
3. Configure your own credentials in n8n.
4. Replace example content with your own source material.
5. Test generation without publishing.
6. Add your preferred approval mechanism.
7. Connect publishing adapters only after validation.

**Never commit API keys, OAuth tokens, cookies, credentials or private production data.**

## Status

The project is being built incrementally. The initial focus is a reliable content-generation and translation pipeline, followed by publishing and analytics adapters.

## Contributing

Contributions are welcome. See `CONTRIBUTING.md`.

## Security

See `SECURITY.md` for reporting sensitive issues.
