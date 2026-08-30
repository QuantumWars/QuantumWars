<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/QuantumWars/QuantumWars/main/assets/header-dark.svg" />
  <img alt="Subha Prakash Pattnaik — AI Engineer & Architect" src="https://raw.githubusercontent.com/QuantumWars/QuantumWars/main/assets/header-light.svg" width="880" />
</picture>

</div>

Most agent demos stop at the model call. I build what's around it — orchestration, tool servers, retries, evaluation — the part that decides whether it survives contact with production.

### `01` What I build

<table>
<tr>
<td width="33%" valign="top">

**Agent infrastructure**

MCP servers and orchestration frameworks that give LLMs real tools — LangGraph pipelines, Claude Code integrations, multi-step research and generation systems.

</td>
<td width="33%" valign="top">

**Applied AI products**

End-to-end tools people actually use — video object removal and inpainting, presentation generation, asset discovery, content and media pipelines, voice and video automation.

</td>
<td width="33%" valign="top">

**Fundamentals**

Comfortable below the framework line — implementing the underlying math by hand instead of only calling an API.

</td>
</tr>
</table>

### `02` Selected work

`01` **[video-object-remover](https://github.com/QuantumWars/video-object-remover)** — Click an object in a video and get back either a matte that tracks it or the plate with it removed. SAM 2 tracks the object across the clip, ProPainter reconstructs the background behind it; the track is cached by prompt, so pulling a matte and then removing the same object pays for tracking once. Ships as a desktop app, a local web app, and a CLI.
<br>`Python` `SAM 2` `ProPainter` `PyTorch` `FFmpeg`

`02` **[propainter-delogo](https://github.com/QuantumWars/propainter-delogo)** — Removes a static logo or watermark and rebuilds what was behind it, instead of smearing pixels over it like `ffmpeg delogo`. Windowed and shot-aware, so only a crop around the logo is inpainted and composited back at native resolution — every other pixel is byte-for-byte the source. 4K-friendly, audio preserved.
<br>`Python` `ProPainter` `OpenCV` `FFmpeg` `CUDA / MPS`

`03` **[clipping-mcp](https://github.com/QuantumWars/video-editor-mcp)** — MCP server that gives Claude Code 41 tools to edit video and audio, on FFmpeg + ElevenLabs: trimming, multicam podcast editing, AI voiceover, timeline projects rendered through Remotion.
<br>`Python` `FFmpeg` `MCP` `ElevenLabs` `Remotion`

`04` **[Deep Research Framework](https://github.com/QuantumWars/DeepResearchAgent)** — Plugin-based multi-agent research system on LangGraph. Decomposes a query, retrieves from multiple sources, reflects on what's missing, and synthesizes a cited report, with automatic tool fallback and complexity-based model routing.
<br>`Python` `LangGraph` `Multi-agent orchestration`

`05` **[NanoBanana Shot Division](https://github.com/QuantumWars/nanobanana-workflow-claude-code)** — Cinematic shot-division workflow for Claude Code. Takes a creative brief, plans an adaptive DAG, and generates continuity-consistent multi-shot storyboards on fal.ai's image models.
<br>`Python` `Claude Code` `fal.ai`

`06` **[Reel Asset Engine](https://github.com/QuantumWars/PublicAssetScraper)** — AI asset search engine that aggregates images, video, and articles from SearxNG, Pinterest, Unsplash, Freepik, and Pexels, then uses LLMs to score and summarize what it finds.
<br>`Next.js` `TypeScript` `LLM scoring`

`07` **[PPT Maker](https://github.com/QuantumWars/ppt-maker)** — Turns a prompt into a structured, styled deck in seconds — nine layout variants, tone and purpose controls, built on GPT-4.
<br>`Next.js` `TypeScript` `OpenAI` `Tailwind`

`08` **[Project Companion](https://github.com/QuantumWars/project-companion)** — Project management that runs with your coding agent: a PRD, a Kanban board, and a git tree that proves what was actually built, all stored in one `.project` file the agent can read and update directly through a bundled MCP server.
<br>`Next.js` `TypeScript` `MCP` `React Flow` `Liveblocks`

`09` **[Context Graph Engine](https://github.com/QuantumWars/context-graph-engine)** — Context store for agentic systems: what an agent knew, decided, and derived, kept on a tamper-evident record that can still forget something on request — a scoped purge that removes the data while the verification chain stays unbroken.
<br>`TypeScript` `Bun` `MCP` `Tamper-evident logs`

### `03` Stack

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/QuantumWars/QuantumWars/main/assets/stack-dark.svg" />
  <img alt="Stack — Python, TypeScript, JavaScript, LangChain, LangGraph, MCP, Next.js, React, Node.js, Tailwind CSS, OpenAI, Anthropic, FFmpeg, Docker, Git" src="https://raw.githubusercontent.com/QuantumWars/QuantumWars/main/assets/stack-light.svg" width="880" />
</picture>

<br/><br/>

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/QuantumWars/QuantumWars/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/QuantumWars/QuantumWars/output/github-contribution-grid-snake.svg" />
  <img alt="contribution snake animation" src="https://raw.githubusercontent.com/QuantumWars/QuantumWars/output/github-contribution-grid-snake.svg" />
</picture>

</div>

### `04` Now

Building agent infrastructure and shipping applied AI products as co-founder at Boring People. Interested in tool-use, multi-agent orchestration, and the unglamorous plumbing that makes an agent reliable in production.

### `05` Contact

`mail` [subhapattnaik@theboringpeople.in](mailto:subhapattnaik@theboringpeople.in)
<br>`in` [in.linkedin.com/in/subha-pattnaik-929488222](https://in.linkedin.com/in/subha-pattnaik-929488222)
