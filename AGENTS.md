> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## About the product

- API docs for Checkobot (checkobot.ai), an AI image and deepfake detection API by SpoofSense. Base URL `https://api.checkobot.ai`.
- The source of truth is the API itself (`api/` in the checkobot repo). Keep request/response shapes, error codes and limits in sync with it.

## Terminology

- Verdicts are `ai` ("AI") and `no_ai` ("No AI detected"). Never call an image "real" or "genuine", or a person "fake".
- The voice here is SpoofSense (plain, technical), not the Checko mascot.

## Style preferences

{/* Add any project-specific style rules below */}

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Never claim detection of audio, liveness, real-time video or "all deepfakes"; IDs and documents only as "coming soon".
- No single accuracy % without its dataset and profile; no internal benchmarks or model weak spots.
- Never show 100% or 0%.
- Don't document internal endpoints (`/v1/quota`, `/v1/account/claim`, thumbnails, image visibility, `/i/...`).
