# Last Mile of Local-first

This talk uses [Marp](https://marp.app/) to generate presentation slides from Markdown.

## 🚀 Quick Start

### 1. Install Marp CLI

Requires Node.js 14+

```bash
npm install -g @marp-team/marp-cli
```

### 2. 🧪 Live Preview

To serve and auto-reload on changes:

```bash
marp . --html --watch --server
```

- Opens at http://localhost:8080
- Press S in browser to open presenter mode with notes

### 3. 📦 Export

Generate static files:

```bash
marp slides.md --html # HTML output
marp slides.md --pdf # PDF output
```

### 🧰 Tips

- Use Marp’s built-in themes: default, gaia, uncover
- Add --allow-local-files if embedding local images
- Add frontmatter options for customizations:

```
marp: true
theme: gaia
paginate: true
```

### 🧩 VS Code Alternative

Install Marp for VS Code for live preview and PDF export inside the editor.
