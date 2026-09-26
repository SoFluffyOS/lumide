# Lumide 0.22.0

### Enhancements

#### Run & Debug
- Add keyboard shortcuts to Run, Debug, and Stop.
- Add top-level `Run` menu and shortcut hints in toolbar tooltips.
- Open debug controls in the left pane and show session logs in the separate Output pane.
- Compact the Debug header and add a menu to show or hide Stacktrace, Variables, and Breakpoints.

#### Editor
- Add CodeLens support for language servers, including clickable actions in the editor.
- Add syntax highlighting for Jenkinsfile and nginx configurations file.

#### Plugins & Panes
- Allow plugins to open webview panels in any pane region.
- Match Debug and Output headers to Files, make Debug sections transparent, and reduce the gap below the Debug header.
- Move Output visibility options to the filter icon, add a search button, and use a trash icon for clearing output.

#### Terminal
- Upgrade `flutter_pty2: 2.0.0` with performance tweaks.

#### Agent Chat
- Support authentication flow for agents.
- Add a settings to Display raw HTML Tags in chat message instead of rendering them as HTML.
- Add message queue. You can interrupt and send immediately or just wait for the next turn.
- Add token usage progress bar with token context window metrics.
- Allow to restore rejected agent changes within 10-second countdown.
- Add ACP Protocol Inspector to view JSON-RPC messages and stderr output.
- Support for project and global `AGENTS.md` rules and `SKILL.md` agent skills with `/skill` autocompletion.

### Fixed
- Fix Agent Chat not restored user's messages correctly.
- Fix cannot enter chat message in second+ Agent Chat.
- Fix some text contrast issue.

---
Visit [lumide.dev](https://lumide.dev) for more.
