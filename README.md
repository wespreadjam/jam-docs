# jam-docs

Source for the Jam documentation at [docs.spreadjam.com](https://docs.spreadjam.com), built with [Mintlify](https://mintlify.com).

## Local development

```bash
npx mint dev
```

The docs are served at `http://localhost:3000`. Check them with `npx mint validate` and `npx mint broken-links`.

## Structure

```
├── index.mdx                    # Introduction
├── get-started/                 # Quickstart, concepts
├── onboard-with-your-agent.mdx  # Connecting agents (overview)
├── onboard-with-your-agent/     # Claude, Claude Code, ChatGPT, Cursor, other clients, agent connect, copy prompt
├── tracking/                    # Prompts, scans, answers, analytics
├── research/
├── actions/                     # The Plan, doing the work
├── delivery/                    # GitHub, Markdown
├── api-reference/               # API overview, MCP server, errors, webhooks (endpoints come from the live OpenAPI spec)
├── billing/
├── style.css                    # Site styling (matches the marketing site)
└── docs.json                    # Mintlify configuration
```

## License

MIT
