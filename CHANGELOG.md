# Lumide 0.16.1

### Fixed
- Fix clicking on result within Project Search removed that search result from the list.

# Lumide 0.16.0

### Enhancements

#### New Pane support
- Diff Pane: Easily compare differences between 2 text.
- Add `Compare with Clipboard` menu to file/editor/editor tab context menu.

#### JSON Viewer enhancement
- Add `Open in JSON Viewer` menu option for JSON files.
- Support format JSON file using built-in `Reformat Code` action.
- Count JSON Array and JSON Object length within JSON Viewer.

#### C.O.R.G.I.
- Refine UI to have more space for the changelist.
- Add Split layout (Stage/Unstaged) for changelist (disable in Settings > Git).
- Optimize performance of git operations (a lot).

#### Project Search
- Add Project Search pane to Add Pane menu.
- Add a button to open search result in left pane.
- Allow toggle Preview panel within Project Search popup.

#### Terminal
- Upgrade `xterm 5.1.0`, `flutter_pty2 1.0.1`.
- Hide terminal process loading indicator in tab bar when the terminal tab is active, replace terminal tab icon with loading indicator.
- Improve terminal glyph rendering, OSC links/colors, clear behavior, PTY stability, notifications, cursors, and progress.

#### Workspace
- Support  open a single file without open any workspace/folder.
- Improve responsiveness during large filesystem changes.

#### New APIs support
- Add `context.workspace.getPluginStorageDir()` for plugins to resolve a private, profile-aware writable storage directory.
- Allow plugin operations inside their `getPluginStorageDir()` directory without requiring extra `fileSystem` manifest permissions.

### Fixed
- Fix light color scheme not preserve after rename an active file.
- Fix Output panel selection loss when scrolling.

---
Visit [lumide.dev](https://lumide.dev) for more.
