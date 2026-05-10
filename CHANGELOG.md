# Lumide 0.6.0

### Enhancements

#### Agent Chat
- Add session history: browse, search, and resume previous agent conversations.
- Add "New Chat" button to status bar and history page for quick session switching.
- Eager input: users can start typing immediately when selecting an agent — messages queue while connecting.
- Collapsible tool call groups in agent chat — collapsed by default, showing only the most recent tool.

### Fixed
- Fix Files failed to discover project files on drive that's not C:\ on Windows.
- Fix Project Search/Quick File Search not focus open tab correctly.

#### Lumide API
- Bump `lumide_api` to `1.3.0` to prevent memory leaks on plugins that use WebViews panel.

---
Visit [lumide.dev](https://lumide.dev) for more.
