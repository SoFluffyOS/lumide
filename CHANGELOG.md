# Lumide 0.14.0

### Enhancements

#### Agent Chat
- Support custom OpenAI-compatible agents.
- Support custom ACP-compatible agents (not in ACP registry).

#### Workspace
- Optimize Project Search and File Search significantly.
- Add support to toggle Git Ignore filter within search.

#### Files
- Support Copy & Paste files/folders across applications.

#### New APIs support
- Upgrade to lumide_api: 1.6.0
- New Menu API — Add new APIs for plugins to register custom actions in menu.
  - Add Pane menu.
  - File/Folder item's context menu.
  - Tab bar item's context menu.
  - Editor's context menu.
- Add a method to File System API for plugins to create directory.

### Fixed
- Fix save failure of settings.json file can reset all settings.
- Fix editor files sometimes opening in non-visible panel. Now files always open in center panel.
- Fix Agent Chat timeout exceptions.

---
Visit [lumide.dev](https://lumide.dev) for more.
