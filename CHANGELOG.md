# Lumide 0.11.0

### Enhancements

#### C.O.R.G.I (Git)
- Map Git menu actions (`Commit...`, `Push`, `Pull`, `Fetch/Refresh`, `New Branch...`, `Stash Changes`, `Unstash Latest`) to their respective commands, running operations in the background or prompting via dialogs instead of always opening the full Git interface.

#### Workspace/Editor
- Support showing match position highlights in the vertical scrollbar for the current selection.
- Improved file saving reliability: implemented atomic saves and added protection against concurrent external changes.
- Enhanced line-ending and encoding support: added dominant line-ending detection and improved preservation of BOM markers and various encodings.
- Add status bar controls to view and switch file line endings (LF/CRLF) and encodings (UTF-8, CJK, etc.).
- Improved read-only file detection on macOS and Linux.
- Add keybindings to toggle the left, bottom, and right panels for VS Code, JetBrains, and Sublime Text keymap presets on macOS, Windows, and Linux.
- Press **→** (Right arrow) on a search result in the Quick Open dialog to open it in the editor without closing the dialog.
- JetBrains keymap: Add **Double Shift** as an alternative shortcut to open the Quick Open dialog.

#### Debugger
- Improved debugger stack trace navigation: jump to frames immediately while variables load and resolve Dart SDK internal frames.
- Refined debugger UI to only highlight the active breakpoint line when paused.

#### Pane System
- Support middle mouse click on tab bar items to close them.

### Fixed
- Fix file permissions (e.g., `0755`) not being preserved when saving files on macOS and Linux.
- Fix exception when monitoring external file changes while switching editor tabs.
- Fix pressing Enter key in other panes triggering file/folder rename in the Files pane.

---
Visit [lumide.dev](https://lumide.dev) for more.
