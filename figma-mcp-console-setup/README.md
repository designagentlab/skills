# figma-mcp-console-setup

**v1.7.0**

A guided setup skill for designers. It connects Claude Desktop to Figma Console MCP — step by step, no Terminal knowledge required.

The skill checks your system automatically, installs what is missing, writes the config file, and walks you through Figma — one clear step at a time.

---

## Before You Start

You will need:

- **Claude Desktop app** — not the browser version → [Download](https://claude.ai/download)
- **Claude Pro, Max, Team or Enterprise**
- **Figma Professional or above**
- **Figma Desktop app** — not the web version → [Download](https://www.figma.com/downloads/)

---

## Install

**If you have Node.js**, ask Claude:

> *"Install the figma-mcp-console-setup skill from github.com/designagentlab/skills/figma-mcp-console-setup"*

**If you are thinking: WTF is Node.js?**
Paste this into Claude Desktop:

> *"Read and follow the setup at raw.githubusercontent.com/designagentlab/skills/main/figma-mcp-console-setup/SKILL.md"*

Claude handles the rest. No Terminal needed.

---

## What the Skill Does

Once installed, just say:

> *"Set up Figma Console MCP"*

The skill will guide you through 9 steps:

1. Check Claude Code is enabled
2. Detect your OS — Mac or Windows
3. Check and install Homebrew *(Mac)* or Node.js *(Windows)*
4. Check and install Node.js
5. Confirm Figma Desktop is installed
6. Get your Figma Personal Access Token
7. Write the MCP config file automatically
8. Import the Figma Desktop Bridge plugin
9. Launch the plugin and verify the connection

**Estimated time: ~10 minutes**

---

## Platform Support

| Platform | Status |
|----------|--------|
| macOS | ✅ Supported |
| Windows | ✅ Supported |
| Linux | 🔜 Coming soon |

---

## Changelog

**v1.7.0**
- Fixed Windows process kill command — replaced `taskkill /F /IM node.exe` (kills all Node processes) with a targeted command that only kills figma-console-mcp
- Removed "run only one Claude Desktop session" advice — multi-instance support has been available since Figma Console MCP v1.10.0
- Added official docs link to resources

**v1.6.0**
- Softer opening message — friendly suggestion to use Claude Desktop instead of aggressive warning
- Improved Cmd+Shift+G explanation for Mac Finder navigation
- Clearer instructions for finding the imported plugin in Figma

---

## Credits

Built on top of [Figma Console MCP](https://github.com/southleft/figma-console-mcp) by TJ and Southleft, LLC.
Official docs: [docs.figma-console-mcp.southleft.com](https://docs.figma-console-mcp.southleft.com)

---

## Part of Design Agent Lab

An open source library of Claude agent skills for designers.

[designagentlab.com](https://designagentlab.com) — [github.com/designagentlab/skills](https://github.com/designagentlab/skills)

*Automate routine. Craft exceptional.*
