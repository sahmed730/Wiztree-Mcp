# WizTree MCP Server

An MCP (Model Context Protocol) server that integrates with [WizTree](https://diskanalyzer.com/), the world's fastest disk space analyzer. It allows AI assistants (like Claude Desktop, Cursor, and Antigravity) to instantly scan your hard drives and identify the largest space-consuming files and folders.

## Features
- **Lightning Fast**: Leverages WizTree's MFT (Master File Table) reading capabilities to scan drives in seconds.
- **AI-Powered Cleanup**: Ask your AI to "find the 15 largest files on my C: drive" or "analyze my Downloads folder."
- **Safe & Non-Destructive**: Only reads and analyzes disk space; it does not delete files automatically, keeping your data secure.

## Requirements
- Windows OS
- [WizTree](https://diskanalyzer.com/) installed at the default location: `C:\Program Files\WizTree\WizTree64.exe`
- Python 3.10 or higher

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sahmed730/Wiztree-Mcp-.git
   cd Wiztree-Mcp-
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   .\.venv\Scripts\Activate
   pip install -r requirements.txt
   ```

## Configuration

Add the server to your MCP client configuration file (e.g., `mcp_config.json`, or Claude Desktop's `claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "wiztree": {
      "command": "C:\\path\\to\\Wiztree-Mcp-\\.venv\\Scripts\\python.exe",
      "args": [
        "C:\\path\\to\\Wiztree-Mcp-\\server.py"
      ]
    }
  }
}
```
*(Make sure to replace `C:\\path\\to\\` with the actual absolute path to where you cloned this repository.)*
