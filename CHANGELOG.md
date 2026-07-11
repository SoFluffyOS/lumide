# Lumide 0.15.0

### Enhancements

#### Workspace
- Un-trusted by default: LSP, plugins, workspace-level settings will be disabled unless you trust a workspace.
- Support to remove recent project.

#### Terminal
- Use `xterm: 5.0.0` and `flutter_pty2: 1.0.0`.
- Improve terminal rendering, OSC links, and high-output responsiveness.

#### Agent Chat
- :boom: BREAKING: Chat message history of Custom Agent now stored within `$HOME/.sofluffy/lumide/chats` separately for each workspace.
- Support to remove chat history of Custom Agent.
- Add more tool calls for custom OpenAI-compatible agents: `update_conversation_title`, `git_add`, `git_commit`, `git_branches`, `git_commits`, `git_status`, `git_diff`, `git_current_branch`, `git_show`, `git_log`, `git_remotes`, `git_stashes`, `git_branch_diff`

#### Files.
- Add New Launch Configuration context menu to easily add launch.json config.

#### New APIs support
- Upgrade to `lumide_api: 1.7.0`.
- Add Launch configuration support — Validate, import, and resolve persistent configurations from `.sofluffy/lumide/launch.json`.

---
Visit [lumide.dev](https://lumide.dev) for more.
