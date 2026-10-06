# Documentation project instructions

## About this project

- This is a documentation site for [Jam](https://spreadjam.com) built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mintlify dev` to preview locally
- Run `mintlify broken-links` to check links

## API Reference tab

- `api-reference/openapi.json` is GENERATED, never hand-edited. The API Reference tab is created from it by Mintlify.
- Regenerate it from the Jam app repo when the API changes: `npm run export:openapi` (writes this file from the app's derived OpenAPI spec). Commit the result here.
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
