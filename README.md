## 5-Day AI Course (Kaggle Edition)

This workspace tracks hands-on material from the Kaggle 5-Day AI Agents course. Each daily folder contains the slides, notebooks, and quick-reference notes used during the sessions. Use this repository as a scratchpad while you experiment with the workflows introduced across the week.

### Folder Guide
- `day 1/` — Prompt-to-action workflows, agent architecture patterns, and the Day 1 reference paper.
- `day 2/` — Tool-enabled agents, Model Context Protocol demos, and the Day 2 reference paper.
- `day 3/` — Context engineering tactics, multi-turn agent session workflows, and memory persistence experiments.

Each day includes a dedicated `README.md` with setup notes that expand on the instructions below.

### Prerequisites
- Python 3.9+ (3.11+ recommended for Day 2 tooling).
- `pip` for dependency management.
- (Optional) Node.js 18+ for MCP server experiments.
- Git, if you plan to version control your work.

### Quick Start
1. Create a virtual environment in the repository root:
   - `python -m venv .venv`
   - Windows PowerShell: `.venv\Scripts\Activate.ps1`
   - macOS/Linux: `source .venv/bin/activate`
2. Install dependencies as prompted inside each notebook (`pip install <package>`).
3. Launch Jupyter with `jupyter lab` or `jupyter notebook`, then open the notebook for the day you are working on.

### Managing Secrets
- Store API keys (e.g., `GOOGLE_API_KEY`) in a local `.env` file or environment variables.
- Keep secrets out of version control (`.env`, `.venv/`, Kaggle token files, etc.).
- When running on Kaggle, prefer Kaggle Secrets instead of hardcoding credentials.

### Working Through the Course
- Execute notebook cells sequentially and read the inline guidance before modifying code.
- Duplicate notebooks before major experiments to keep an untouched reference version.
- Capture lessons learned, prompts, and results in markdown cells or a separate journal.
- Commit meaningful checkpoints if you are using Git.

### Additional Resources
- Refer to the PDF slides in each day’s folder for conceptual context.
- Follow the per-day `README.md` files for platform-specific setup details.
- Join the course discussion channels for troubleshooting tips and peer support.

