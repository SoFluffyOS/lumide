# Lumide 0.13.0

### Enhancements

#### Editor
- Add Tree Indent Guide support.
- Add replace and replace-all support to Project Search, including preserve-case replacement.
- Change default font size from `14` to `13` and default line height from `20` to `22`.
- Git Blame: Hide inline ghost text on modified (dirty) lines and disable hover popups for uncommitted changes.

#### Pane System
- Terminal pane and Agent Chat pane can now be renamed.

#### Files
- Support to **Filter files** within the file tree.
- Support to **Select multiple files/folders** in the Files pane using modifier keys (Cmd/Ctrl/Shift).
- Single-clicking a file opens it temporarily. Edit or click that file again to keep the tab open.
- Add a dedicated settings category in Settings UI for Files.
- Add setting to show Git ignored files and folders in the file tree (enable by default).

### Fixed
- Fix hidden folders (e.g. `.dart_tool`) not being filtered out on macOS and Linux when show hidden files setting is off.
- Fix JetBrains keymap `Cmd + 1` failing to toggle the left panel.
- Fix normal text input fields (like Search field or Agent Chat Input,...) not accepting keyboard shortcuts.
- Fix closing an active tab not switching back to the previously active tab in history.
- Fix editor gutter diff misalignments by using Myers' Diff algorithm for diff calculation.

---
Visit [lumide.dev](https://lumide.dev) for more.
