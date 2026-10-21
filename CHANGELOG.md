# Lumide 0.24.0

Lumide goes multiplayer: share a workspace with anyone from a link, or work on another machine over SSH.

### Enhancements

#### Remote Development
- **[Share a Workspace](https://docs.lumide.dev/workspace/collaboration)**: Anyone joins from a link, in Lumide or their browser, as Viewer, Editor or Trusted. Share terminals and Agent Chats too, or run your own relay on a spare Android phone.
- **[Remote SSH](https://docs.lumide.dev/workspace/remote-ssh)**: Open a folder on another machine; files, terminals, Git and language servers run there.
- **[Lumide in the Browser](https://docs.lumide.dev/workspace/web)**: Serve a workspace to any browser with `lumide_server serve`.

#### Workspace
- **[Multi-root Workspaces](https://docs.lumide.dev/workspace/multi-root)**: Several folders in one window, saved as a `.lumide-workspace` file, each with its own settings.
- **Open with Lumide**: From your file manager, by drag & drop, or `lumide --add <folder>`.
- **[Plugin Recommendations](https://docs.lumide.dev/plugins)** for the files you open.
- Clone a repository from the Welcome screen.
- **Import Settings** from VS Code, Cursor, Zed or another Lumide: found on your machine, pasted, or from a file.
- Project Search: search some folders only, and exclude files. Find in Files can open in the Search Pane instead of a dialog.
- **Bottom Panel Layout**: Run the bottom panel across the whole window, or under the left or right panel.
- **Starting Layout**: Start new windows the way Lumide or VS Code lays them out.
- **Onboarding** asks which editor you're coming from, sets its shortcuts and layout, and offers to bring your settings over.

#### Git
- **AI Commit Messages**: Suggestions in your repository's style.
- **[Line History](https://docs.lumide.dev/git)** and **Several Repositories**: see who changed the selected lines, and fetch, pull, push and commit across repositories.
- Filter branches in the branch menu.

#### Editor
- Undo in natural steps, copy the whole line with nothing selected, and placeholders for binary files.
- Paste a copied file to insert its path.
- Syntax colors for SVG, with the CSS in its `<style>`, and XML formats such as `.csproj`, `.xaml` and `.storyboard`.
- **Mermaid Diagrams**: Class, state, ER, mindmap, git graph and many more diagram types in the Markdown preview, drawn in your theme.

#### Run & Debug
- **[Tests Pane](https://docs.lumide.dev/debugging)**: Run, rerun and debug tests, with lenses above Dart tests and coverage from plugins.
- Launch configurations and SDKs per workspace folder.

#### AI
- **[Agent Comments](https://docs.lumide.dev/ai)**: Comment on lines, diffs or the agent's changes, then send them all at once.
- Type in Agent Chat before an agent connects, reopen recent chats, and copy a message as HTML.

#### New APIs support
- Upgrade to `lumide_api: 1.13.0`: workspace folder APIs, `runsPerFolder` for language servers, and `InlineCompletionRequest.instructions`.

### Fixed
- CORGI: the commit message is readable in light themes.
- Agent Chat: code in Review Changes is colored for light themes too.
- Notifications use their own colors, so a notice no longer looks like an error.
- Fix the hierarchy gutter not showing; it's also faster in large files.
- CSS written without spaces, such as `a{color:red}`, no longer shows property names twice.
- Markdown preview: a tag in code, such as `<style>`, no longer hides the rest of the page.
- Read-only views, such as diffs, no longer change on Paste, Tab, Move Line or Undo.
- CORGI: ticking a file in separate staged and unstaged lists no longer shows the next file ticked.
- Faster typing in long sessions, and faster saves, also for large files.
- Format on save skips a formatter slower than 5 seconds.
- The launch dropdown keeps your selected configuration at startup.
- Git, language servers and plugins started at launch get your shell's `PATH`.
- Fix Inline Blame and its delay setting.
- Stage All skips files with conflict markers; switching to a missing branch no longer discards changes.
- Rolling back, discarding or unstaging a file whose name has `[`, `*`, `?` or a leading `-` touches only that file.
- Push and Force Push send only the current branch, to its own name, never onto another branch.
- Plugins installed from the marketplace start right away.
- Terminals report real exit codes.
- Keep folds, highlighting and breakpoints in place after multi-cursor edits.
- Project Search file patterns work as expected, and Find in Folder searches only that folder.
- Project Search and Quick Open include `bin` folders, where Dart and Go keep sources.
- **Linux**: Updates for the right architecture, `PATH` from your shell profile, Open With, trash, and the `Alt` app menu.

---
Visit [lumide.dev](https://lumide.dev) for more.
