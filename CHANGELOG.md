# Lumide 0.18.2

### Fixed
- Fix a Settings UI crashed due to enum parsing failure after editing AI policy options.

# Lumide 0.18.1

### Fixed
- Double-tap not open search result in Project Search dialog.

# Lumide 0.18.0

### Enhancements

#### C.O.R.G.I.
- Add a separate `Stashes` tab. You can now preview stash content before taking any actions.
- Add `Remotes` tabs to view/add/edit/remove remote.
- Add a review dialog before pusing commits (press `Cmd/Ctrl + Shift + K` or access in `Git` > `Push...` menu).
- Add `Git Rollback` action to roll backc an unstaged change at the editor cursor or all changes in selected files and folders (press `Cmd/Ctrl + Alt + Z` or access in `Git` > `Rollback...` menu).
- Add option to `Discard All Changes...` or `Discard Unstaged Changes...` when discarding files and folders with both staged and unstaged changes.

#### Editor
- Add a Filter within code Quick Actions.
- Improve `JSON` and `YAML` syntax highlight to provide more colors.
- Support to press Backspace to remove empty white space quickly.
- Add new action `Extend Selection Word Left/Right with CamelHumps Mode`.
- Correct `Extend Selection Word Left/Right` to only select words separated by space.

#### Files
- Switch editor tab now won't Reveal active file as default (configurable in `Settings` > `Files` > `Auto Reveal Active File`).
- Click on an active editor tab to Reveal the file in Files pane (configurable in `Settings` > `Files` > `Reveal File on Active Tab Click`).
- Choose whether `File Open Mode` opens files on a single click or selects them until double-clicked.
- Control automatic Files pane selection with `Auto Reveal Active File`.
- Enable `Reveal File on Active Tab Click` to reveal files only when their active editor tab is clicked.

#### Pane System
- Browse or filter Add Pane options, then use Up/Down and Enter to choose a pane.
- Use `View` > `Add Pane` and `Toggle Pane` menus.
- Agent Chat now will be show as default pane in Right pane.

#### Project Search
- Add customizable shortcuts for Match Case, Whole Word, Regex, Replace, Preserve Case, Ignored Files, and Preview.

#### Settings
- **General**: Add `Confirm Before Exiting the IDE` to skip the quit prompt while still saving files and application state.
- **Editor**: Add `Show JSON Annotations` to show or hide object and array counts in the JSON Viewer.
- **Keymap**: Support to remove keybindings to any shortcut.

---
Visit [lumide.dev](https://lumide.dev) for more.
