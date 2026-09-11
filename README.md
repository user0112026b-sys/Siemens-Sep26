# GitHub MCP Server & Siemens-Sep26

## GitHub MCP Server Setup (Python)

This project provides a Python MCP server for GitHub with tools to:
- Search repositories
- Get repository details
- List repository issues
- Create an issue

### 1. Create and activate a virtual environment

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 2. Install dependencies

```powershell
pip install -r requirements.txt
```

### 3. Add credentials in `.env`

Edit `.env` and set:

```env
GITHUB_TOKEN=your_github_personal_access_token
```

### 4. Run the MCP server

```powershell
python server.py
```

The server runs over stdio and is ready to be used by MCP clients.

### 5. Example MCP client config

```json
{
  "mcpServers": {
    "github": {
      "command": "python",
      "args": ["d:/Kiran/Synechron/Claude/Module 10 - MCP/github-mcp-server/server.py"]
    }
  }
}
```

### Notes
- `.env` is ignored by git.
- For private repos or write operations, ensure your token has required GitHub permissions.

---

## Siemens-Sep26
Siemens project - September 2026
