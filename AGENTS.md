# Documentation project instructions

## About this project

- This is a documentation site for [Jam](https://spreadjam.com) built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mintlify dev` to preview locally
- Run `mintlify broken-links` to check links

## API Reference tab

- The API Reference tab is created by Mintlify from the live OpenAPI spec at `https://api.spreadjam.com/openapi.json` (wired via the tab's `openapi` URL in `docs.json`). Mintlify fetches it at build time, so the published reference always matches what the API serves. There is no spec file in this repo to regenerate or commit.
- The spec is derived from the app's route schemas; to change the reference, change the API in the Jam app repo and ship it. The docs pick up the new surface on the next Mintlify build.
- `api-reference/overview.mdx` is the hand-written getting-started page (auth, keys); edit it freely. Per-endpoint pages come from the spec, so do not hand-write them.

## Terminology

- Use "Jam" to refer to the product
- Use "agents" not "bots" when referring to AI automation
- Use "workflow" not "pipeline" for automation sequences

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise. One idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document all user-facing features and APIs
- Do not document internal admin features
