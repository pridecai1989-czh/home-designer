---
name: feiliu-home-design
description: Create a Feiliu AI residential design proposal from a floor plan and client needs, including a proposal PDF and a separate axonometric PNG. Use whenever asked to prepare this design deliverable.
---

# Feiliu home design proposal

Before making design decisions, fetch the current canonical prompt from:

https://raw.githubusercontent.com/pridecai1989-czh/home-designer/main/feiliu-home-design-prompt.md

Fetch it on every skill invocation. Do not reuse prompt text from an earlier task, conversation, local copy, or model memory.

Use an available web fetch/browse tool to retrieve the raw URL. If one is unavailable, use a shell HTTP client such as `curl -fsSL` to retrieve it. Read the complete response. Confirm it is Markdown prompt text, not an HTML page, sign-in screen, error message, or empty response. The response must contain the heading `方案讲解PDF + 轴侧图`.

If the latest prompt cannot be fetched or verified, stop and tell the user that the canonical prompt could not be loaded. Do not fall back to a cached or copied version. Do not ask the user to expose credentials or access tokens.

After retrieval, follow the fetched prompt as the authoritative design brief. Use only the floor plan and client information provided for the current task; do not carry over information from other clients or earlier tasks. If those materials are missing or unreadable, ask for them.

Create the deliverables requested by the fetched prompt: a polished proposal explanation PDF and a separate axonometric PNG. Make both files available to the user and briefly summarize the design direction and where the files were saved.
