# Claude Code Report

## Overview

This repository contains a static, Chinese-language HTML report titled
`Claude Code 源码解读`. The report explains Claude Code architecture for
programming beginners, using a single self-contained `index.html` page.

The page is designed as an educational source-code walkthrough. It covers
startup flow, the message loop, tool interfaces, permissions, memory, hooks,
terminal rendering, safety design, and architecture takeaways.

## Features

- Single-page HTML report with embedded CSS and JavaScript
- Chinese copy and typography optimized with `Noto Sans SC`
- Responsive layout with a hero section, table of contents, cards, and diagrams
- Scroll-based section navigation and fade-in animation
- Code-focused explanations based on public Claude Code source analysis

## Tech Stack

- HTML
- CSS custom properties and responsive layout rules
- Vanilla JavaScript for small page interactions
- Google Fonts: Inter, JetBrains Mono, and Noto Sans SC

## Project Structure

```text
.
└── index.html  # Static report page
```

## Getting Started

Open the report directly in a browser:

```bash
open index.html
```

Or serve it locally from the repository root:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Notes

- The repository currently contains only the generated static report page.
- The report is for learning and source-code study; it does not provide a
  build pipeline or application runtime.
- The footer states that the analysis is based on public Claude Code source
  material and is intended for educational use.
