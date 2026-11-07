# Documentation project instructions

## About this project

- This is a documentation site for [Jam](https://spreadjam.com) built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mintlify dev` to preview locally
- Run `mintlify broken-links` to check links

## API reference

- The endpoint pages (the **Endpoints** group under API and MCP reference) are created by Mintlify from the live OpenAPI spec at `https://api.spreadjam.com/openapi.json` (wired via the group's `openapi` URL in `docs.json`). Mintlify fetches it at build time, so the published reference always matches what the API serves. There is no spec file in this repo to regenerate or commit.
- The spec is derived from the app's route schemas; to change the reference, change the API in the Jam app repo and ship it. The docs pick up the new surface on the next Mintlify build.
- `api-reference/overview.mdx` is the hand-written getting-started page (auth, keys); edit it freely. Per-endpoint pages come from the spec, so do not hand-write them.

## Agent pages

- `onboard-with-your-agent/*` and `api-reference/*` document using the Jam product from an agent (REST, MCP at `https://api.spreadjam.com/mcp`, agent connect). The errors page has one anchor per error `code`; the API links to `api-reference/errors#<code>`, so keep the anchors in step with `API_ERROR_CODES` in the app repo.
- Copy rules: no em dashes, never the word "generated" (use "created").

## Terminology

- Use "Jam" to refer to the product
- Use "agents" not "bots" when referring to AI automation

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise. One idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document all user-facing features and APIs
- Do not document internal admin features

## Look

- `style.css` carries the marketing site's look (app repo `src/components/landing-v2/landing.css`): paper `#f1f1f1`, ink `#3d3b4f`, brand `#fa114e`, Geist and Geist Mono; dark paper `#1c1b24`, ink `#ecebf2`.
- `logo/light.svg` and `logo/dark.svg` are the mark next to the word "Jam", both in the text colour (the angled mark in light mode, the flat mark in dark), with the word drawn as paths so no font is needed.
