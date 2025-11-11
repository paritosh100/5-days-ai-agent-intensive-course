# 5-Day AI Course (Local Setup Guide)

This repository contains notebooks from the Kaggle 5-Day Agents course. Use this guide to run them locally while keeping secrets safe.

## 1. Prerequisites

- Python 3.11+
- `pip`
- [Node.js 18+](https://nodejs.org/) (required for MCP demos)
- Git

## 2. Create and Activate a Virtual Environment

```bash
python -m venv .venv
.venv\Scripts\activate    # Windows
source .venv/bin/activate  # macOS / Linux
```

## 3. Install Python Dependencies

The Kaggle notebooks rely on the Google ADK and support libraries.

```bash
pip install google-adk pillow kaggle kaggle-secrets google-generativeai
```

> Tip: check each notebook for any additional `pip install` lines and install them as needed.

## 4. Configure Environment Variables

Create a `.env` file or export variables in your shell (do **not** commit `.env`).

```
GOOGLE_API_KEY=your_api_key_here
``` 

Then load it before running code:

```bash
set GOOGLE_API_KEY=your_api_key_here            # Windows PowerShell
export GOOGLE_API_KEY=your_api_key_here         # macOS / Linux
```

## 5. Run Jupyter

```bash
pip install notebook
jupyter notebook
```

Open the notebook under `day 2` (or the relevant day) and run cells one by one.

## 6. MCP Tools (Optional)

If you want to use the Model Context Protocol examples:

```bash
npm install -g @modelcontextprotocol/server-everything
npm install -g @google/modelcontextprotocol-server-google-ai
```

Make sure your `GOOGLE_API_KEY` is set before invoking the Google MCP server.

## 7. Keep Secrets Safe

- Never commit API keys or secret values.
- Add `.env`, `.venv/`, and other sensitive paths to `.gitignore` if you create them.
- Use Kaggle Secrets when running on Kaggle.

## 8. Git Quick Start

```bash
git init
git add .gitignore README.md
git status
```

Commit frequently and push to your own remote when ready.

Happy hacking! 🎉
