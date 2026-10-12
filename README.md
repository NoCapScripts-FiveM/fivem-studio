<div align="center">

<img src="assets/fivem-studio-logo.png" alt="FiveM Studio" width="128" height="128" />

# FiveM Studio

**A fast, focused code editor built for FiveM resource development.**

Lua autocomplete for every native · live linting · NUI scaffolding · one-click preview

![Electron](https://img.shields.io/badge/Electron-37-47848F?logo=electron&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Monaco](https://img.shields.io/badge/Editor-Monaco-007ACC)
![Platform](https://img.shields.io/badge/Windows-ready-0078D4?logo=windows&logoColor=white)
![Version](https://img.shields.io/badge/version-1.0.5-orange)

</div>

---

## 👋 Welcome

FiveM Studio is a lightweight desktop editor made for people who write FiveM resources. You get the Monaco editor you already know from VS Code, plus tooling that understands FiveM: natives, `fxmanifest.lua`, client/server scripts and NUI.

Open a folder, start typing `GetPlayer...`, and the editor already knows what you mean.

## ✨ Features

### 🧠 FiveM-aware Lua
- **Autocomplete and hover docs** for FiveM natives, with parameters, return types and descriptions.
- Natives are downloaded from `runtime.fivem.net` on first launch, then cached for offline use.
- **Client vs. server awareness**: get warned when a native is used on the wrong side.

### 🔍 Built-in linting
- Syntax errors, with CfxLua extras (backticks, `+=`, `<const>`) tolerated.
- Infinite loops without a `Wait` are flagged.
- Hints for deprecated patterns like `Citizen.*` and `GetPlayerPed(-1)`.
- `fxmanifest.lua` checks.
- Everything shows up in a **Problems** panel.

### 🧩 NUI scaffolding and preview
- Create a **new NUI resource** in seconds: `fxmanifest.lua`, client and server Lua, and a UI.
- Choose **Alpine.js** (CDN, no build step) or **React + Vite**.
- **NUI preview window**: open any `.html` file, press *Preview*, send test messages and watch NUI callbacks in the log.

### 🗂️ Editor essentials
- File explorer with **drag-and-drop** moves, create, rename and delete (to trash).
- Multi-tab editing with unsaved-change tracking.
- Integrated **terminal** panel (PowerShell on Windows).
- Resizable sidebar.
- Syntax highlighting for Lua, TypeScript, JavaScript, JSON, HTML, CSS, Markdown, Python and C#.

### 🎨 Themes
Pick your vibe under **Appearance**: `dark` · `chocolate` · `latte` · `light` · `contrast`

## 🚀 Quick start

```bash
# 1. install dependencies
npm install

# 2. run in development (hot reload)
npm run dev
```

Then:

1. Click **Open Folder** and pick your resource (or your whole `resources/` directory).
2. Open the **FiveM tools** tab to scaffold a new NUI resource.
3. Open a `.lua` file and start coding.

> 💡 **First launch needs internet.** Monaco loads from a CDN and the natives list is fetched once. After that the natives are cached.

## ⚠️ Known limitations

- The terminal is a plain PowerShell process with no TTY. It's great for commands, not for interactive programs.
- React NUI previews need `npm run build` inside the resource's `web/` folder first.

## 🧭 Roadmap ideas

- [ ] Resource-wide search and replace
- [ ] Git integration
- [ ] Snippets for common ESX / QBCore / ox_lib patterns
- [ ] Auto-update

## 🤝 Contributing

Ideas, bug reports and pull requests are welcome. Open an issue describing what you'd like to change, or fork the repo and send a PR.

## 📄 License

Add your license here (MIT is a popular choice).

---

<div align="center">

Made with ☕ for the FiveM community.

</div>
