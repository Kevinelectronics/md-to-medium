# Markdown to Medium Converter

A free, browser-based tool to convert Markdown files into clean, publish-ready content for Medium — no login, no installation, no data sent anywhere.

**[→ Open the tool](https://kevinelectronics.github.io/md-to-medium/)**

---

## What It Does

Paste your Markdown on the left. Get a Medium-ready preview on the right. Click **Copy for Medium** and paste directly into the Medium editor with `Ctrl+V`.

That's it.

---

## Who This Is For

This tool is useful if you:

- **Write technical articles on Medium** and draft them in Markdown (VS Code, Obsidian, Notion, Typora, Bear, iA Writer, etc.)
- **Use AI tools** like ChatGPT or Claude to generate long-form content in Markdown and need to publish it fast
- **Maintain a blog or newsletter** and cross-post from a Markdown-based CMS (Jekyll, Hugo, Ghost, Docusaurus) to Medium
- **Write developer tutorials** with code blocks, headers, and lists that need to survive the copy-paste into Medium's editor
- **Create content at scale** — batch-converting multiple articles without reformatting each one by hand
- **Work in documentation tools** (GitHub READMEs, Confluence, Notion) and want to repurpose content as Medium posts

---

## Why Not Just Paste Markdown Directly into Medium?

Medium's editor doesn't parse raw Markdown. If you paste `**bold**` you get literal asterisks. If you paste a code block with triple backticks you get a wall of text.

This tool renders your Markdown into formatted HTML first, then copies the rich text so Medium receives it as styled content — headings, bold, italics, code blocks, bullet lists, blockquotes, and all.

---

## Features

- Live preview as you type
- Medium-style typography (Georgia serif, 18px, 1.8 line height)
- Proper rendering for: `h1`–`h3`, paragraphs, `**bold**`, `*italic*`, `- lists`, `1. ordered lists`, `> blockquotes`, `` `inline code` ``, and fenced code blocks
- `---` separators are automatically removed (Medium turns them into unwanted "· · ·" dots)
- No build step, no dependencies, no server — single HTML file, runs entirely in your browser
- Works offline

---

## How to Use

1. Open `index.html` in any browser (Chrome, Firefox, Edge, Safari)
2. Paste your Markdown into the left panel
3. Review the preview on the right
4. Click **Copy for Medium**
5. Open your Medium draft and press `Ctrl+V` (or `Cmd+V` on Mac)

---

## Keyboard Shortcuts

| Action | Shortcut |
|--------|----------|
| Copy for Medium | Click the button (or select all in preview + `Ctrl+C`) |
| Clear input | Select all in textarea + `Delete` |

---

## Local Setup

No installation needed. Just download and open:

```bash
git clone https://github.com/Kevinelectronics/md-to-medium.git
cd md-to-medium
# Open index.html in your browser
```

Or [download the ZIP](https://github.com/Kevinelectronics/md-to-medium/archive/refs/heads/main.zip) and open `index.html` directly.

---

## Tech Stack

- Vanilla HTML + CSS + JavaScript
- [marked.js](https://marked.js.org/) for Markdown parsing (loaded via CDN)
- Zero frameworks, zero build tools

---

## Limitations

- Images must be hosted externally — Medium doesn't accept base64 images on paste
- Very complex tables may lose some formatting in Medium's editor
- Syntax highlighting in code blocks is visual only (Medium doesn't support it natively)

---

## Contributing

Found a formatting issue or want to add a feature? Open an issue or submit a PR.

---

## License

MIT — free to use, modify, and distribute.

---

*Built by [Kevin Meneses](https://www.linkedin.com/in/kevin-meneses-gonzalez/) · If this saved you time, [follow me on Medium](https://medium.com/@kevinmeneses)*
