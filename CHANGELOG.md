# Lumide 0.26.0

Find your way around code the IntelliJ way: usages, call hierarchy, the file's structure, sticky scroll and inlay hints, with the keys you already know. And C.O.R.G.I. can now drop, reword and squash commits.

### Enhancements

#### 🧭 Code Intelligence
- **[Go to Type Definition, Implementation and Super Member](https://docs.lumide.dev/languages/hover-and-definitions#type-definition-implementation--super-member)**: `Ctrl + Shift + B`, `Cmd + Alt + B` and `Cmd + U`, as in IntelliJ.
- **[Sticky scroll](https://docs.lumide.dev/editor#sticky-scroll)**: The class and method you're in stay pinned at the top of the editor, and open folders at the top of Files.
- **[Inlay hints](https://docs.lumide.dev/editor#inlay-hints)**: Hold `Ctrl + Option` to see inferred types and parameter names in the code. Double-click one to write it in.
- **[Spell check](https://docs.lumide.dev/editor#spell-check)**: Typos in comments, strings and names get a faint underline. Right-click to fix one or add it to a dictionary.
- **[Surround With](https://docs.lumide.dev/editor/snippets#surround-with-cmd--alt--t)**: `Cmd + Alt + T` wraps the selection in an if, a loop, a try or a Flutter widget.
- **[Postfix completion](https://docs.lumide.dev/editor/snippets#postfix-completion)**: `user.isActive.if` becomes `if (user.isActive) {}`. `.var`, `.for`, `.not` and more, in Dart.
- **[Usages pane](https://docs.lumide.dev/languages/hover-and-definitions#find-usages-alt--f7)**: Every usage of a symbol, by file, to work through with Next Usage. `Alt + F7`, as in IntelliJ.
- **[Call Hierarchy](https://docs.lumide.dev/languages/hover-and-definitions#call-hierarchy-ctrl--alt--h)**: Who calls a function, and what it calls, as a tree in a pane of its own.
- **[Symbols in the breadcrumb](https://docs.lumide.dev/getting-started/interface)**: The editor header goes on past the file to the class and member you're in. Click one to jump through the file.
- **[Structure pane](https://docs.lumide.dev/navigation#structure-pane-cmd--7--alt--7)**: The file's classes and members as a tree that follows your caret. `Cmd + 7`, as in IntelliJ.

#### ✏️ Editor
- **[Previews as you left them](https://docs.lumide.dev/editor/markdown-preview#display-modes)**: A Markdown, SVG or HTML file opens in the mode you last picked for its kind. Drag the line of a split view to resize it, and a narrow pane puts the preview below the code.
- **[Long Line Wrap](https://docs.lumide.dev/editor#soft-wrap)**: With soft wrap off, only lines over 2,000 columns wrap, to keep minified files fast. The header says when they do, and Settings → Editor → Long Line Wrap changes the limit.

#### 🗂️ Workspace
- **[Where Panes Open, for every tool](https://docs.lumide.dev/getting-started/interface#where-panes-open)**: Search, Structure, Problems, Output, Tests, Debug, previews and the rest each have a place of their own, and stay where you move them. Agent-first opens the tools on the right and previews beside Agent Chat.
- **[Open with Lumide](https://docs.lumide.dev/workspace/workspaces#open-with-lumide-from-your-file-manager)**: Right-click a folder or file in Finder, File Explorer, Dolphin or Files to open it in Lumide. On Windows and Linux, Lumide asks before adding it.

#### 🐶 C.O.R.G.I.
- **[Commit dates](https://docs.lumide.dev/git/corgi#visual-commit-graph)**: Hover a date for how long ago it was and its time zone, or show every date as "3 days ago" with Commit Date Format. Click a hash to copy it.
- **[Hidden lines](https://docs.lumide.dev/git/corgi#staging-files--hunks)**: Each hunk starts with how many unchanged lines it hides and the function it's in, instead of Git's `@@ -248,7 +248,7 @@`. Hover it to show 20 more lines, or all of them.
- **[Drop, Reword, Squash and Fixup](https://docs.lumide.dev/git/corgi#rewriting-history)**: Right-click commits in the graph, or press `d`, `r`, `s` or `f` as in lazygit. One rebase that keeps merges and your local changes, with Undo right after.
- **[Tags](https://docs.lumide.dev/git/corgi#branches-tab)**: `T` tags a commit or a branch, annotated when you give it a message, and can push it right away. `P` pushes a tag and `d` deletes it here, on a remote or both, as in lazygit. The graph shows every tag on a commit, and Push… offers to push the tags on the commits it sends.

#### 💬 Agent Chat
- **[Files beside Agent Chat](https://docs.lumide.dev/getting-started/interface#where-panes-open)**: With Agent Chat in the center, opening a file splits it to the right instead of covering the chat. Close the last file and the chat takes the center back.
- **[Wide tables](https://docs.lumide.dev/ai#context--mentions)**: A table in a reply grows past the text, up to the whole pane, so its columns aren't squeezed. One wider still scrolls sideways, and Open Larger shows it in a dialog.
- **[Message Claude Code while it works](https://docs.lumide.dev/ai#opening-agent-chat)**: It reads your message right away and keeps going, as in the Claude CLI. No more waiting for the turn to end, or stopping it.

### Fixed
- **Clipboard reads in the terminal**: A program can no longer read your clipboard by printing an escape sequence (OSC 52), which a file shown with `cat` could do. Set `terminal.clipboard_read` to `ask` to allow it case by case.
- **Links printed in the terminal**: Lumide asks before opening a link a program prints, so a file shown with `cat` can't open a page or an app by itself. A clicked link that isn't a web or mail link asks too.
- **Pictures in Agent Chat**: A web picture in a reply waits for you to click Load Image, so a reply can't send your data to a server just by showing one. Pictures on another computer's share never load.
- **Korean, Japanese and Chinese input**: Typing with a composing input method works in the editor, the terminal and Agent Chat. `한글` no longer comes out as `ㅎㅏㄴㄱㅡㄹ`.
- **Review Changes**: Code takes your theme's syntax colors again in a light theme, and the gutter fits line numbers of three digits and more.
- Resuming a long chat no longer lags, and its old commands and subagents stay out of the Agents sidebar while it loads.
- A local plugin starts again after you stop it, Restart runs it again instead of only stopping it, and it runs instead of an installed copy of the same plugin until you remove it.
- Uninstalling a plugin removes it from both Puro's pub cache and the default one, so it doesn't come back on the next start, and an update loads the version it installed.
- Quitting Lumide or closing an Agent Chat stops the servers and commands its agent left running in the background.
- Coming back to a file shows its problems, code lenses and inheritance marks at once, and moving quickly between files no longer keeps the language server busy with the ones you left.
- Opening a Flutter project no longer starts the Python plugin, and files Git ignores no longer start any plugin.

---
Visit [lumide.dev](https://lumide.dev) for more.
