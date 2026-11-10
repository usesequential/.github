# Sequential

**Session replay and analytics for teams with a website or app.**

Sequential finds the problems your visitors hit, hands each one to your own AI coding agent (like Claude Code or Cursor), and checks that the fix worked.

[Website](https://www.usesequential.com) · [Docs](https://www.usesequential.com/docs) · [Agent tools](https://www.usesequential.com/docs/agent-tools) · hello@usesequential.com

## How it works

Sequential does five steps. Your agent does two. You set the questions and review each fix.

| Step | Who | What happens |
|---|---|---|
| 1. Record | Sequential | Sequential records each visit as a session: the pages, taps and errors, and a replay that you and your agent can watch. Your agent adds Sequential to your app with one prompt. |
| 2. Judge | Sequential | Sequential's AI reads each session and answers your questions about it, like "Could the person check out?" Each answer is a verdict, like "No: the shop rejected the address." Sequential comes with built-in questions. You tailor them to your product, or your agent proposes changes. |
| 3. Evidence | Sequential | Sequential lists the sessions with their verdicts. |
| 4. Case | Sequential | Sequential opens a case for one product problem, with those sessions as its evidence. |
| 5. Fix | Your agent | Your agent connects over MCP (the standard way AI agents use tools), reads the case, watches its replays and writes the fix. Your team reviews and releases it. Sequential never changes your code. |
| 6. Report | Your agent | Your agent, or a release step in your CI, tells Sequential which release carries the fix and when it went live. |
| 7. Measure | Sequential | Sequential counts how often the problem happens before and after the release. When it stops happening, Sequential marks the case fixed. |

## Get started

Paste this prompt into your coding agent:

```text
Set up Sequential in this app. Read https://www.usesequential.com/docs/agent-trial.md, create a trial for <your work email>, install the SDK for this app's platform, check that events arrive (ask me to open the app if you cannot), and tell me to open the claim email.
```

It works for websites and for iOS, Android and React Native apps. You do not need an account first. Sequential sends you an email to claim the trial.

In Claude Code, you can install the plugin instead:

```text
/plugin marketplace add usesequential/claude-plugin
/plugin install sequential@usesequential
```

## Repositories

**Add Sequential to your app**

| Repository | What it is |
|---|---|
| [sequential-browser](https://github.com/usesequential/sequential-browser) | Browser SDK on npm (`@usesequential/browser`): analytics and session replay, the same code that Sequential's script tag loads. |
| [sequential-node](https://github.com/usesequential/sequential-node) | Node.js SDK (`@usesequential/node`): sends your backend's events and errors to the same person and browser session. |
| [gtm-template](https://github.com/usesequential/gtm-template) | Google Tag Manager tag template that loads Sequential. |
| [wordpress-plugin](https://github.com/usesequential/wordpress-plugin) | WordPress plugin that adds the Sequential tag to every page. |
| [examples](https://github.com/usesequential/examples) | A Next.js app and a Google Tag Manager guide. |

**Connect your agent**

| Repository | What it is |
|---|---|
| [mcp](https://github.com/usesequential/mcp) | Settings for Sequential's hosted MCP server (`https://api.usesequential.com/mcp`) in Claude Code, claude.ai, Cursor, Codex, Claude Desktop, Cline and Gemini CLI. |
| [claude-plugin](https://github.com/usesequential/claude-plugin) | Sequential plugin for Claude Code: adds Sequential to your app and reads sessions over MCP. |
| [sequential-cli](https://github.com/usesequential/sequential-cli) | Command-line tool (`@usesequential/cli`): the agent tools from a shell, a CI job or a script. It can also record releases. |

**Record releases**

| Repository | What it is |
|---|---|
| [release-action](https://github.com/usesequential/release-action) | GitHub Action and a small CLI (`@usesequential/release-cli`) that record a release: its version, the merged pull requests and the cases they fix. |

**Docs**

| Repository | What it is |
|---|---|
| [docs](https://github.com/usesequential/docs) | The Sequential docs as Markdown, a mirror of [usesequential.com/docs](https://www.usesequential.com/docs). |

---

Questions: hello@usesequential.com · [Privacy Policy](https://www.usesequential.com/privacy) · [Terms of Service](https://www.usesequential.com/terms)
