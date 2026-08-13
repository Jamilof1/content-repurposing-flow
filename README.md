# Prism — Content Repurposing Flow

Turn one source into editable LinkedIn, email, social, and follow-up drafts while keeping review visible. Project 07 in the Jamil Darwish Automation Lab.

## Modes

- **Demo:** deterministic templates create useful starting drafts locally.
- **AI:** your model creates a richer multi-channel bundle through a private local proxy.

## Quick start

Requires Node.js 22+.

```bash
git clone https://github.com/Jamilof1/content-repurposing-flow.git
cd content-repurposing-flow
npm install
npm run dev
```

For AI mode, copy `.env.example` to `.env`, add `AI_API_KEY`, and restart. PowerShell: `Copy-Item .env.example .env`.

## Provider configuration

The default is OpenAI Responses with `AI_MODEL=gpt-5`. For an OpenAI-compatible chat endpoint, set its base URL/model and `AI_API_STYLE=chat`. The API key remains server-side and `.env` is ignored by Git.

## Features

- Source, audience, tone, and call-to-action capture.
- Four editable channel drafts with approval progress.
- Optional AI content bundle grounded in the source.
- Per-draft copy and complete Markdown download.

## Commands

`npm run dev` starts client + API, `npm test` runs tests, `npm run build` creates `dist/`, and `npm start` serves it.

## Responsible use

Demo transformation stays local. AI mode sends the visible source and current drafts only after a click. Check facts, rights, links, brand voice, claims, and channel policies before publishing; the app never auto-publishes.

MIT — built by [Jamil Darwish](https://jamildarwish.com/).
