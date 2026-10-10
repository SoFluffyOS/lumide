# Lumide 0.23.0

C.O.R.G.I. gets its biggest update yet: a branch tree, lazygit-style keys, a PR-style review and a full merge conflict editor.

### Enhancements

#### C.O.R.G.I.
- **Conflict Editor**: Linear, Side by Side or Three Panels. Pick Current, Incoming or Both from the keyboard; a wand fixes simple conflicts.
- **Paused Operations**: One banner for merges, rebases, cherry-picks and reverts: resolve, then Continue, Skip or Abort.
- **Review**: Every uncommitted change in one scroll, like a pull request. Edit, stage or discard each hunk.
- **Branches**: Branches, remotes and tags in one tree, with folders, favourites and ahead/behind counts.
- **Branch Switcher**: Fuzzy search, recent first, create from your query, stash-and-switch.
- **Graph**: All branches, stashes and working changes. Search the whole history and cherry-pick or revert several commits at once.
- **Keyboard**: lazygit-style keys in every panel, all rebindable. Press `?` for the list.
- Conflict bars in normal editor tabs.

#### Git
- **Git Avatars**: Author and co-author avatars in Blame and Commit Inspector.
- **Git Hosting Providers**: GitHub, GitLab, Bitbucket, Azure DevOps, Gitea, Forgejo, SourceHut and self-hosted.
- Blame popup previews line changes; click the hash to inspect the commit.
- Open Commit Inspector as a modal or a tab.
- Diff view mode and soft wrap are remembered.

#### Run & Debug
- Edit breakpoint conditions and log messages from the Breakpoints panel.
- Add Tests pane for plugin test runs, with a failed-only filter.

#### New APIs support
- Upgrade to `lumide_api: 1.12.0`. 💥 BREAKING: `on*` listeners now return a `LumideDisposable`.
- Formatting, Diagnostics and Progress APIs: plugins can format documents, report problems and show status bar progress.
- Tests API: report test runs to the new Tests pane.
- Commands API: `commands.executeCommand`; `onCommand:` commands show in the Command Palette before the plugin starts.
- Workspace events: `onDidChangeTextDocument` now receives edits; add `onDidChangeFiles`.
- Process API: `environment` and `stdin` for shell commands, signals for `shell.kill`, and `sdks.spawn`.
- Keybindings: `mod` key (Cmd on macOS, Ctrl elsewhere) and `when` clauses.
- Debug API: `logMessage` for breakpoints.
- Manifest `executable` field for asset-only plugins, and per-extension language IDs for language servers.

#### Editor
- Syntax highlighting for Git files, `.plist` and lockfiles.
- Multiline regex in Find & Replace.

#### Language Servers
- Run several language servers per file.
- Stop or disable a language server per workspace.

#### Workspace
- Move, resize and maximize dialogs; drag the window while one is open.
- Hide empty pane regions automatically.
- Open the active `settings.json` from the settings header.

### Fixed
- Fix C.O.R.G.I. with non-ASCII file names.
- Fix C.O.R.G.I.'s "Accept All Conflicts" writing the file path into the file.
- Fix creating a branch from a commit; new branches no longer track their source branch.
- Show files inside new untracked folders, stashes and merge commits in C.O.R.G.I.
- Fix crash in Add Custom Agent dialog.
- Fix `Show JSON Annotations` ignored when disabled.
- Fix blame diff paths on Windows and in sibling folders.
- Keep edits during saves, tab close and Vim save-and-quit.
- Keep unsaved markers and AI completions after renames and Save As.
- Keep Git file highlighting after opening files, switching themes and renaming.
- Keep ANSI colors in truncated output.
- Keep Hot Exit backups when a restore fails.
- The font picker no longer blocks the UI.

---
Visit [lumide.dev](https://lumide.dev) for more.
