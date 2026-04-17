# 🦊 Lumide — Pure Light. Pure Speed.

[![Lumide](https://lumide.dev/favicon.ico)](https://github.com/SoFluffyOS/lumide)
![Built with Flutter](https://img.shields.io/badge/Built%20with-Flutter-02569B?style=flat&logo=flutter)

**Lumide** is a desktop-first code editor built with **Flutter** and **Impeller**, providing GPU-accelerated rendering and an ultra-smooth editing experience. The legacy Electron era ends today.

[Website](https://lumide.dev) | [Documentation](https://docs.lumide.dev) | [Blog](https://blog.lumide.dev)

---

## 🚀 Not just Fast. **So Fast.**

Designed to be featherweight, Lumide is built from the ground up to be the fastest editor you've ever used.

*   **💙 Built with Flutter**: A modern, unified desktop experience powered by the same engine that drives high-performance mobile apps.
*   **⚡ Blazing Fast Editor**: Custom-built text rendering engine with virtualized scrolling and a **Rope-based** data structure (O(log n) operations).
*   **🧠 Memory Efficient**: Ultra-light footprint (~80 MB idle). No more multi-gigabyte RAM overhead from browser-based editors.
*   **💎 GPU Accelerated**: Leveraging the **Impeller** engine for silky-smooth 120 FPS rendering on modern displays.
*   **🔌 Infinite Extensibility**: Tap into the world's largest Dart ecosystem. Install themes, language servers, and tools directly from **pub.dev**. Hot-load plugins with ease.
*   **🤖 AI-Powered Completion**: High-performance inline suggestions via plugins. Support for **GitHub Copilot**, **Mistral Codestral**, and **Mercury** with silky-smooth **"Ghost Text"** UX.
*   **🕵️ AI Agent Protocol (ACP)**: First-class support for autonomous AI agents. Connect to **Claude, Gemini, OpenAI, goose, Cline**, and more via the Agent Client Protocol.
*   **🐶 C.O.R.G.I. Git Client**: A flow-driven Git interface with a "Split-Brain" layout. Features **Context-First navigation**, **Granular Staging**, **Integrated Stash**, and **Interactive Diff Editor**.
*   **🛠️ Rich Intelligence**: Full **LSP** support for completions, diagnostics, and go-to-definition. First-class support for **Dart & Flutter**.
*   **🌿 Native Git Insights**: Inline **Git Blame** (Ghost Text), status colors in file tree, and **Gutter/Scrollbar diff markers** (Added, Modified, Deleted).
*   **🎹 Muscle Memory**: Customizable keymaps with presets for **JetBrains**, **VS Code**, and **Sublime Text**.
*   **🗂️ Flexible Pane System**: A docking system that adapts to your workflow, keeping your workspace organized.

---

## 📦 Download

Visit **[lumide.dev](https://lumide.dev)** to download the latest version for your platform.

Alternatively, you can find all versions on our [Releases](https://github.com/SoFluffyOS/lumide/releases) page.

- **macOS** (Universal / Apple Silicon)
- **Windows** (x64)
- **Linux** (Coming Soon)

---

## 📂 Repository Structure

This repository ([SoFluffyOS/lumide](https://github.com/SoFluffyOS/lumide)) serves as the public host for Lumide compiled releases and issue tracking. 

- `README.md`: This file.
- `CHANGELOG.md`: Current version release notes.
- `CONTRIBUTING.md`: Feedback and bug report guidelines.

---

## 🏗️ Technical Integrity

Lumide is engineered with a strict performance mandate: **one keystroke should touch O(log n) rope nodes, a handful of visible lines, and nothing else synchronously.**

- **Virtualized Rendering**: Only what you see is what we draw.
- **Asynchronous Pipeline**: Syntax highlighting and diagnostics run off the main thread to keep the input loop lag-free.
- **Rope Data Structure**: High-performance text manipulation that handles large files with ease.

---

## 🛡️ Privacy & Security

Lumide is designed to be a private and secure tool for developers.
- **Local First**: Your code stays on your machine.
- **No Telemetry**: We don't track your keystrokes or project data.
- **Zero bloat**: No background analytics processes.

---

## 🤝 Community

Join the journey to build the ultimate developer environment.

- **Issues**: Report bugs or suggest features on our [Issue Tracker](https://github.com/SoFluffyOS/lumide/issues).
- **Discord**: [Join the SoFluffy community](https://discord.gg/VP6p5JQdgt).

---

*Made with 💖 by SoFluffy in 2026.*
