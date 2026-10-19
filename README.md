# Ivor

**I build tools that help AI agents understand code, debug failures, and work across real systems.**

Senior Systems Engineer, GenAI Operations. Based in Madrid. My recent work spans execution recording, time-travel debuggers, agent harnesses, MCP integrations, and workflow automation. I work across TypeScript, Python, Go, and Java.

## Runtime evidence for people and agents

**[Pyokka](https://github.com/ivorpad/pyokka) · Python** and **[Tracelight](https://github.com/ivorpad/tracelight) · JavaScript / TypeScript**

Two projects built around the same question: what did this program actually do? They expose live values, recorded execution, and debugging through VS Code, a browser interface, a CLI, and MCP. An agent can inspect a run, follow a value's history, or pause the program and investigate alongside you.

[![Pyokka debugger driven from a terminal, with runtime values beside the code](https://raw.githubusercontent.com/ivorpad/pyokka/main/docs/media/pyokka.gif)](https://github.com/ivorpad/pyokka/blob/main/docs/media/pyokka.mp4)

*Pyokka in action: an agent drives the debugger through function breakpoints and stepping while the editor shows the paused values. [Watch the video](https://github.com/ivorpad/pyokka/blob/main/docs/media/pyokka.mp4).*

[Pyokka guide](https://github.com/ivorpad/pyokka/blob/main/docs/GUIDE.md) · [Tracelight runtime internals](https://github.com/ivorpad/tracelight/blob/main/docs/RUNTIME.md) · [Tracelight wire protocol](https://github.com/ivorpad/tracelight/blob/main/docs/PROTOCOL.md)

## From browser interactions to agent tools

**[Rewalk](https://github.com/ivorpad/rewalk)** records what someone does and says while using a web page, then connects spoken complaints to DOM changes and React components. Coding agents get the relevant browser evidence, bug reports, and replays. [Watch the demo](https://github.com/ivorpad/rewalk/blob/main/assets/demo.mp4).

**[agent-cli-scaffold / agtcli](https://github.com/ivorpad/agent-cli-scaffold)** is a Python runtime and scaffold for CLIs agents can drive. Generated tools start with structured output, typed exit codes, credential handling, request guards, and contract tests. A checker makes the interface rules inspectable.

**[har2cli](https://github.com/ivorpad/har2cli)** turns an authenticated browser network capture into a redacted HTTP contract, tests a selected GET request, and hands it to agtcli to generate a CLI. It keeps credentials separate from exported contracts and bounds the requests used to probe authentication.

## Agent infrastructure and applied AI

| Project | What it does |
| --- | --- |
| **[WorkDone](https://github.com/ivorpad/workdone)** | Coordinates Claude Code, Codex, and Cursor agents across machines through ChatGPT and MCP. Voice interaction, persistent sessions, agent events, and approval handling. |
| **[Farrier](https://github.com/ivorpad/farrier)** | Generates repository-specific agent harnesses with rules, tested guard hooks, and verification commands. Includes session analysis and evaluations that distinguish observed results from unproven benefits. |
| **[Claude Agent SDK for n8n](https://github.com/ivorpad/n8n-nodes-claude-agent-sdk)** | Runs agent tasks inside self-hosted workflows, with multiple providers, memory, human approvals, MCP tools, structured output, and persistence. |
| **[Mercadona CLI](https://github.com/ivorpad/mercadona-cli)** | Gives agents a structured interface to a real grocery service: product search, prices, and cart management. Written in Go and distributed as a standalone binary and through npm. |

<details>
<summary>More tools for agent context, integrations, and verification</summary>

**Debugging and agent context.** [PyCharm Debugger MCP](https://github.com/ivorpad/pycharm-debugger-mcp) exposes the IDE's debugger to agents. [sxr](https://github.com/ivorpad/sxr) searches Claude Code and Codex session histories; [transcript-reader](https://github.com/ivorpad/transcript-reader) provides a local reader for Claude Code sessions. [sk](https://github.com/ivorpad/sk) loads skills on demand instead of putting every skill into the initial context.

[orly](https://github.com/ivorpad/orly) gives agents access to O'Reilly Answers with book citations.

**Checks and integrations.** [konpy](https://github.com/ivorpad/konpy) enforces structural conventions in Python repositories. [CodeMie for n8n](https://github.com/ivorpad/n8n-nodes-claude-codemie) adds SSO proxy authentication to the Claude Agent SDK node. [Raycast Prompter](https://github.com/ivorpad/raycast-prompter) puts editable LLM writing prompts behind a keyboard shortcut.

I also build Herdr plugins for [agent notifications](https://github.com/ivorpad/herdr-notify), [agent lifecycle management](https://github.com/ivorpad/herdr-reap), [local ports](https://github.com/ivorpad/herdr-ports), and [tunnels](https://github.com/ivorpad/herdr-tunnel).

</details>
