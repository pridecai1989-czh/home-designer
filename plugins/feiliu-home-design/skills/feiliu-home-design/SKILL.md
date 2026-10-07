---
name: feiliu-home-design
description: 根据户型图和客户需求，制作飞流 AI 住宅设计提案 PDF 与独立轴侧图 PNG。需要完成住宅设计方案或方案讲解交付时使用。
---

# 飞流 AI 住宅设计方案

开始设计前，必须先读取 GitHub 上的最新版完整提示词：

https://raw.githubusercontent.com/pridecai1989-czh/home-designer/main/feiliu-home-design-prompt.md

每次调用本 Skill 都要重新读取，不得沿用此前任务、对话、记忆或本地副本中的提示词。

优先使用当前可用的网页浏览或网页读取能力打开上述 raw 链接，并读取完整内容。如果无法通过网页读取，可使用可用的 HTTP 工具获取链接内容。确认返回的是非空 Markdown 提示词，而非 HTML 页面、登录页面或错误信息；内容中必须包含标题“方案讲解PDF + 轴侧图”。

如果无法读取或验证最新版提示词，立即停止，并告知用户无法加载 GitHub 上的正式提示词。不得退回旧版本或缓存副本，也不得要求用户提供凭证或访问令牌。

成功读取后，严格以该最新版提示词作为本次设计任务的依据。只使用当前任务提供的户型图和客户资料，不得带入其他客户或此前任务的信息。如果材料缺失或无法辨认，先向用户索取。

按提示词要求制作可交付的方案讲解 PDF 和独立轴侧图 PNG。完成后提供两个文件，并简要说明设计方向和文件保存位置。---
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
