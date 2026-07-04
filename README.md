<div align="center">
  <h1>🚀 WizTree MCP Server</h1>
  <p><strong>Supercharge your AI Assistant with the world's fastest disk space analyzer.</strong></p>
  
  <p>
    <img alt="Platform" src="https://img.shields.io/badge/Platform-Windows-blue?style=flat-square&logo=windows">
    <img alt="Python Version" src="https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python">
    <img alt="License" src="https://img.shields.io/badge/License-MIT-green?style=flat-square">
    <img alt="Protocol" src="https://img.shields.io/badge/Protocol-MCP-purple?style=flat-square">
  </p>
</div>

---

## 🌟 Overview

The **WizTree MCP Server** seamlessly bridges your AI assistant (Claude, Cursor, Antigravity, etc.) with [WizTree](https://diskanalyzer.com/), allowing your AI to instantly scan your hard drives, identify massive space hogs, and execute intelligent cleanups.

Turn your AI into a highly contextual storage manager!

## ✨ Features

- ⚡ **Lightning Fast:** Leverages WizTree's MFT (Master File Table) reading to scan drives in seconds.
- 🧠 **AI-Powered Workflows:** Ask your AI: *"What's eating up space on my C: drive?"* or *"Analyze my Downloads folder."*
- 🛡️ **Built-in Guardrails:** Comes with a comprehensive `/skills` directory to teach your AI strict deletion policies and safe handling of files.
- 💻 **Developer Focused:** Perfect for finding hidden `node_modules`, stray `__pycache__` folders, or giant dangling Docker images.

---

## 🚀 Installation

### 1. Prerequisites
- **Windows OS**
- **[WizTree](https://diskanalyzer.com/)** (installed at `C:\Program Files\WizTree\WizTree64.exe`)
- **Python 3.10+**

### 2. Clone the Repository
```bash
git clone https://github.com/sahmed730/Wiztree-Mcp.git
cd Wiztree-Mcp
```

### 3. Setup Virtual Environment
```bash
python -m venv .venv
.\.venv\Scripts\Activate
pip install -r requirements.txt
```

---

## ⚙️ Configuration

Add the server to your MCP client configuration (e.g., `mcp_config.json` for Antigravity, or `claude_desktop_config.json` for Claude):

```json
{
  "mcpServers": {
    "wiztree": {
      "command": "C:\\path\\to\\Wiztree-Mcp\\.venv\\Scripts\\python.exe",
      "args": [
        "C:\\path\\to\\Wiztree-Mcp\\server.py"
      ]
    }
  }
}
```
> ⚠️ **Note:** Replace `C:\\path\\to\\` with the exact absolute path to your cloned directory.

---

## 🤖 Example Prompts

Once connected, try asking your AI:
- 💬 *"Can you find the 15 largest files on my C: drive?"*
- 💬 *"My SSD is full. Find the largest folders in my user profile, skipping my personal photos."*
- 💬 *"Do a developer cleanup on my machine to free up at least 20 GB."*

---

<div align="center">
  <i>Built with ❤️ for the MCP Community</i>
</div>
