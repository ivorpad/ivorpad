# Ivor

Senior software engineer in Madrid. I build tools for AI agents: debuggers that expose what a program actually did, harnesses that enforce repository rules, and integrations that let agents work with real services.

Most of my recent work is in **agent infrastructure, developer tools, and applied AI**. I work across TypeScript, Python, Go, and Java, from runtime instrumentation and IDE plugins to MCP servers and workflow integrations.

## Selected work

| Project | What I built |
| --- | --- |
| **[Tracelight](https://github.com/ivorpad/tracelight)** | Execution recording, live debugging, and code history for JavaScript and TypeScript. A VS Code extension, browser interface, CLI, and MCP tools give people and agents access to runtime evidence. |
| **[WorkDone](https://github.com/ivorpad/workdone)** | A ChatGPT plugin and MCP server for coordinating Claude Code, Codex, and Cursor agents across machines. Includes voice interaction, agent events, approval handling, and remote file and shell access. |
| **[Farrier](https://github.com/ivorpad/farrier)** | Generates coding-agent harnesses from repository evidence: rules, hooks, verification commands, and context files. Includes behavioral checks and session analysis, with explicit limits on what the evaluations establish. |
| **[Claude Agent SDK for n8n](https://github.com/ivorpad/n8n-nodes-claude-agent-sdk)** | Runs agent tasks inside self-hosted workflows, with multiple providers, session memory, human approvals, MCP tools, structured output, and persistence. |
| **[Mercadona CLI](https://github.com/ivorpad/mercadona-cli)** | A Go CLI that lets agents search a real grocery catalog, inspect products, and manage a cart through structured output. Distributed as a standalone binary and through npm. |
| **[Rewalk](https://github.com/ivorpad/rewalk)** | Records browser interactions and spoken feedback, then connects complaints to DOM changes and React components. Produces bug reports and replay artifacts a coding agent can use. |

## More of the work behind those tools

**Debugging and agent context.** [Pyokka](https://github.com/ivorpad/pyokka) brings live values and time-travel debugging to Python. [PyCharm Debugger MCP](https://github.com/ivorpad/pycharm-debugger-mcp) exposes the IDE's debugger to agents. [sxr](https://github.com/ivorpad/sxr) searches Claude Code and Codex session histories; [transcript-reader](https://github.com/ivorpad/transcript-reader) provides a local reader for Claude Code sessions. [sk](https://github.com/ivorpad/sk) loads skills on demand instead of putting every skill into the initial context.

**Tools agents can drive.** [agtcli](https://github.com/ivorpad/agent-cli-scaffold) is a runtime and scaffold for CLIs with explicit output contracts, failure codes, and credential handling. [har2cli](https://github.com/ivorpad/har2cli) turns browser network captures into redacted HTTP contracts and CLI scaffolds. [orly](https://github.com/ivorpad/orly) gives agents access to O'Reilly Answers with book citations.

**Checks and integrations.** [konpy](https://github.com/ivorpad/konpy) enforces structural conventions in Python repositories. [CodeMie for n8n](https://github.com/ivorpad/n8n-nodes-claude-codemie) adds SSO proxy authentication to the Claude Agent SDK node. [Raycast Prompter](https://github.com/ivorpad/raycast-prompter) puts editable LLM writing prompts behind a keyboard shortcut.

I also build Herdr plugins for [agent notifications](https://github.com/ivorpad/herdr-notify), [agent lifecycle management](https://github.com/ivorpad/herdr-reap), [local ports](https://github.com/ivorpad/herdr-ports), and [tunnels](https://github.com/ivorpad/herdr-tunnel).
