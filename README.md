# 🔍 FC GitLens AI

**Architectural Intelligence & Repository Inspector**

GitLens AI is a high-performance, web-based repository explorer that leverages the **Google Gemini 3** series models to provide deep architectural insights, code analysis, and visual representations of any public GitHub repository.
#
*TRY it NOW(no API key required):*  https://ai-git.replit.app
---

## 🚀 Core Features

### 1. **Deep Repository Exploration**
- **Recursive Tree Mapping**: Instantly index and browse the entire file structure of any public GitHub repository.
- **Multi-Media Support**: Preview code (with PrismJS syntax highlighting), images, videos, audio, and PDFs directly in the browser.
- **File Finder**: Lightning-fast file searching using global keyboard shortcuts (`Cmd/Ctrl + K` or `Cmd/Ctrl + P`).

### 2. **AI Architect Agent**
- **Contextual Analysis**: Get instant summaries, complexity ratings, and refactoring recommendations for any file.
- **Snippet Analysis**: Select any block of code to trigger a targeted explanation of that specific logic.
- **Project-Wide Reasoning**: Add multiple files to a "Project Context" to ask complex questions about cross-file data flows and architectural patterns.
- **Smart File Linking**: AI responses automatically link to files in the repo; hover over them for a "Peek" summary.

### 3. **Visual Intelligence**
- **Dependency Blueprint**: Interactive D3.js force-directed graph mapping imports and logic connections between files.
- **Codebase Treemap**: Heatmap visualization of the project's composition, sized by file weight and categorized by language.
- **Onboarding Brief**: AI-generated "Welcome" documentation for any repo, explaining the tech stack, entry points, and overall architecture.

### 4. **Developer DNA**
- Analyze the repo owner's profile to understand their primary coding "DNA," strengths, and project ecosystem.

---

## 🛠️ Technical Stack

- **Framework**: React 19 (ESM)
- **Styling**: Tailwind CSS with custom glassmorphism components
- **AI**: Google Gemini API (`gemini-3-flash-preview` for speed, `gemini-3-pro-preview` for complex reasoning)
- **Visuals**: D3.js (Force graphs & Treemaps)
- **Syntax**: PrismJS with support for 20+ languages
- **Utilities**: `html2canvas` for exporting onboarding briefs, `diff` for commit comparisons.

---
<img width="1906" height="1857" alt="image" src="https://github.com/user-attachments/assets/f924e243-be45-404f-8a9d-2c20db549351" />
<img width="1917" height="2792" alt="image" src="https://github.com/user-attachments/assets/9d609bbc-f7d0-4b86-8d5c-ebd48b4c9bff" />
<img width="1925" height="2767" alt="image" src="https://github.com/user-attachments/assets/03780e18-db20-4682-9d57-4cfa2f32b484" />
<img width="1908" height="1636" alt="image" src="https://github.com/user-attachments/assets/36de211c-e3b6-4257-a97f-b15c4c4ff62e" />

## ⚙️ Configuration

### Gemini API Key / Open router
This application requires a API key to function. Ensure it is provided via the environment:
```env
API_KEY=your_gemini_api_key or openrouterAPI
```

### GitHub Personal Access Token (PAT)
To avoid the default GitHub API rate limit (60 requests/hour), you can provide a Personal Access Token in the **Settings** panel (top right). This increases your limit to 5,000 requests/hour.
1. Go to GitHub Settings > Developer Settings > Personal Access Tokens (classic).
2. Generate a token with `repo` scope (for public/private access) or no scope (for public access only).
3. Paste it into the GitLens AI Settings panel.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| `Cmd/Ctrl + K` | Open File Finder |
| `Cmd/Ctrl + [` | Toggle Sidebar |
| `Esc` | Close Peek Cards / Modals |

---

## 🎨 Themes

GitLens AI supports four premium visual modes:
- **Deep Sea** (Default): High-contrast blue-dark mode.
- **Forest**: Emerald-tinted professional interface.
- **Ruby Nebula**: Crimson-accented creative mode.
- **Midnight**: Pure black OLED-optimized interface.

---

*Built with ❤️ for architects and developers who want to understand code faster.*
