# Playwright MCP Setup Guide

**[Microsoft Playwright MCP Server Repository](https://github.com/microsoft/playwright-mcp)**

**[Playwright MCP Server Info](playwright-mcp-server.md)**

**[Prompt Examples](playwright-mcp-promt-examples)**

## Prerequisites:

### 1. Node.js install:
- Go to **https://nodejs.org/en/download**.
- Choose and **download the latest version** for your OS.
- **Run the installer** - Keep defaults (includes npm). If prompted about “Tools for Native Modules” (build tools), you can skip unless you know you need it. *If on Intellij, install the necessary Node.js plugin.*
- Open a new terminal (PowerShell/cmd for Windows) and **verify version**:
```
node -v
npm -v
```
---

### 2. Install or enable Copilot Chat:

- Install/enable [GitHub Copilot](https://code.visualstudio.com/docs/copilot/setup) + Copilot Chat (or another MCP-capable chat/agent experience in VS Code).

- Open Copilot Chat and switch to **Agent mode** (this is where tools can be invoked).
  
- **IntelliJ difference**: If using Copilot in [JetBrains](https://docs.github.com/en/copilot/get-started/quickstart?tool=jetbrains), open Copilot Chat and ensure you’re in Agent mode there too.
(If using JetBrains [AI Assistant](https://www.jetbrains.com/help/ai-assistant/installation-guide-ai-assistant.html) instead of Copilot, MCP tools appear in AI Assistant chat once configured.)

---

### 3. Playwright MCP server install:

- Go to [Microsoft Playwright MCP Repository](https://github.com/microsoft/playwright-mcp)
- ... WIP 




  
---

### 4. Playwright setup:

Running Playwright MCP tests does not specifically require Playwright setup, only the server, but running tests on browsers does require browser binaries, so adding them using: 
``` npx playwright install ``` or installing Playwright is necessary.
For any additional hands-on testing, Playwright setup is also a must, so **setting it up is recommended**.

- You can follow the **Visual Studio Code Playwright installation guide** [here](https://playwright.dev/docs/getting-started-vscode);
  
  or
  
- **IntelliJ Playwright installation guide** [here](https://www.jetbrains.com/help/idea/playwright.html).
