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

### <ins>*For VS Code:*</ins>
- Go to [Microsoft Playwright MCP Repository](https://github.com/microsoft/playwright-mcp)

- Click the **Install Server: VS Code** button


<img width="1165" height="387" alt="image" src="https://github.com/user-attachments/assets/eb6ed0ad-786c-4f19-9e63-30b1255c622b" />

- Click **Open Visual Studio code** 

<img width="1232" height="738" alt="image" src="https://github.com/user-attachments/assets/46354c52-d5d3-49b4-9d09-6bba81134a73" />

- In VS Code, click **Install** 

<img width="693" height="460" alt="image" src="https://github.com/user-attachments/assets/695ab129-2f2f-471f-80fa-95563de8001e" />

- Start the server (if not already started)  

<img width="497" height="546" alt="image" src="https://github.com/user-attachments/assets/1847c930-e439-4dd5-8abe-cbe8bfcf0a1c" />

---

### <ins>*For IntelliJ:*</ins>
- Go to *Settings*
  
- Click *Tools > MCP Server*

<img width="978" height="497" alt="image" src="https://github.com/user-attachments/assets/bc2a4cc3-9dae-432a-a41e-cbc2d8e11392" />

 - *Enable MCP Server*

<img width="616" height="532" alt="image" src="https://github.com/user-attachments/assets/596b16c7-45d8-4987-9260-96880aa65f7a" />

- To point Copilot to the MCP server, go to *Tools > GitHub Copilot*

<img width="503" height="405" alt="image" src="https://github.com/user-attachments/assets/d6b0fb60-3870-4ed1-939a-76ae8371dc54" />

- Click *Configure*

<img width="630" height="537" alt="image" src="https://github.com/user-attachments/assets/7e9a3d8c-b686-4298-9d5b-432a9520316a" />

- Paste the [Microsoft Playwright MCP standard config .json](https://github.com/microsoft/playwright-mcp) over the current configuration:

![Animation](https://github.com/user-attachments/assets/2f78c8bf-cc35-4c82-8f27-dc44747ebb33)

1. Make sure to change *Ask* to *Agent* in your Copilot chat.
2. Install the *microsoft/playwright-mcp* from the MCP Registry
 
<img width="707" height="960" alt="image" src="https://github.com/user-attachments/assets/45b55922-575d-4ac2-b018-9916cb5c16d8" />










  
---

### 4. Playwright setup:

Running Playwright MCP tests does not specifically require Playwright setup, only the server, but running tests on browsers does require browser binaries, so adding them using: 
``` npx playwright install ``` or installing Playwright is necessary.
For any additional hands-on testing, Playwright setup is also a must, so **setting it up is recommended**.

- You can follow the **Visual Studio Code Playwright installation guide** [here](https://playwright.dev/docs/getting-started-vscode);
  
  or
  
- **IntelliJ Playwright installation guide** [here](https://www.jetbrains.com/help/idea/playwright.html).
