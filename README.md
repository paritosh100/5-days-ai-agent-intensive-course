# 🚀 5-Day AI Agents Course (Kaggle Edition)

A comprehensive hands-on course on building production-ready AI agents using Google's Agent Development Kit (ADK). This repository contains all the notebooks, slides, and resources from the Kaggle 5-Day AI Agents course.

## 📚 Course Overview

This course takes you from zero to production-ready AI agents, covering everything from basic prompt engineering to advanced observability and evaluation. Each day builds upon the previous concepts, culminating in a complete understanding of modern AI agent development.

### What You'll Learn

- **Day 1**: Foundation - From prompts to actions, agent architectures
- **Day 2**: Tools & Integration - Building tool-enabled agents, MCP protocol
- **Day 3**: Context & Memory - Session management, memory persistence
- **Day 4**: Quality & Reliability - Observability, evaluation, user simulation

## 📁 Repository Structure

```
5-day-ai-course-kaggle/
├── day 1/          # Foundation: Prompts → Actions, Agent Architectures
├── day 2/          # Tools: Tool-enabled agents, MCP demos
├── day 3/          # Context: Sessions & Memory management
├── day 4/          # Quality: Observability & Evaluation
└── README.md       # This file
```

### Day-by-Day Breakdown

#### 📅 Day 1: From Prompt to Action
**Notebooks:**
- `day-1a-from-prompt-to-action.ipynb` - Guided walkthrough of prompt design and tool use
- `day-1b-agent-architectures.ipynb` - Survey of agent patterns and orchestration strategies

**Key Topics:**
- Prompt engineering fundamentals
- Transforming ideas into runnable code
- Agent architecture patterns
- Design trade-offs and best practices

**Resources:**
- `Day_1_v4 (1).pdf` - Conceptual overview and reference material

---

#### 🔧 Day 2: Agent Tools & Best Practices
**Notebooks:**
- `day-2a-agent-tools.ipynb` - Building tool-enabled agents
- `day-2b-agent-tools-best-practices.ipynb` - Advanced tool integration patterns

**Key Topics:**
- Tool-enabled agent development
- Model Context Protocol (MCP) integration
- Third-party tool integration
- Tool performance optimization

**Resources:**
- `Day_2_v6.pdf` - Reference documentation

---

#### 💾 Day 3: Sessions & Memory
**Notebooks:**
- `day-3a-agent-sessions.ipynb` - Multi-turn conversation management
- `day-3b-agent-memory.ipynb` - Memory persistence and context engineering

**Key Topics:**
- Session management and state handling
- Short-term and long-term memory
- Context engineering tactics
- Memory persistence strategies

**Resources:**
- `Context Engineering_ Sessions & Memory.pdf` - Deep dive into context management

---

#### 🔍 Day 4: Observability & Evaluation
**Notebooks:**
- `day-4a-agent-observability.ipynb` - Logs, traces, and metrics
- `day-4b-agent-evaluation.ipynb` - Systematic evaluation and user simulation

**Key Topics:**
- **Observability (Reactive):**
  - Logging agent execution
  - Tracing agent workflows
  - Metrics and performance monitoring
  
- **Evaluation (Proactive):**
  - Creating test cases
  - Tool trajectory scoring
  - Response match scoring
  - User simulation for dynamic testing
  - Regression testing

**Resources:**
- `Agent Quality.pdf` - Quality assurance strategies

---

## 🛠️ Prerequisites

### Required
- **Python 3.9+** (3.11+ recommended for Day 2 tooling)
- **pip** for dependency management
- **Jupyter Notebook/Lab** for running notebooks
- **Git** (optional, for version control)

### Optional
- **Node.js 18+** for MCP server experiments (Day 2)
- **Google AI Studio API Key** - Get yours at [aistudio.google.com/app/api-keys](https://aistudio.google.com/app/api-keys)

## 🚀 Quick Start

### 1. Clone or Download This Repository

```bash
git clone <repository-url>
cd 5-day-ai-course-kaggle
```

### 2. Set Up Virtual Environment

```bash
# Create virtual environment
python -m venv .venv

# Activate virtual environment
# Windows PowerShell:
.venv\Scripts\Activate.ps1

# macOS/Linux:
source .venv/bin/activate
```

### 3. Install Dependencies

The main dependency is the Google ADK:

```bash
pip install google-adk
```

Additional packages may be required per notebook (install as prompted):
```bash
pip install pillow kaggle kaggle-secrets google-generativeai
```

### 4. Configure API Keys

**For Local Development:**
Create a `.env` file in the repository root (do NOT commit this file):

```env
GOOGLE_API_KEY=your_api_key_here
```

Or set as environment variable:
```bash
# Windows PowerShell:
$env:GOOGLE_API_KEY="your_api_key_here"

# macOS/Linux:
export GOOGLE_API_KEY="your_api_key_here"
```

**For Kaggle Notebooks:**
- Use Kaggle Secrets (Add-ons → Secrets)
- Create a secret named `GOOGLE_API_KEY`
- Access it in notebooks using `kaggle_secrets`

### 5. Launch Jupyter

```bash
pip install notebook jupyterlab
jupyter lab
# or
jupyter notebook
```

### 6. Start Learning!

Open the notebook for the day you're working on and follow along:
- Execute cells sequentially
- Read markdown cells for context
- Experiment and modify code
- Take notes on your learnings

## 📖 How to Use This Repository

### Working Through the Course

1. **Follow Sequential Order**: Days build upon each other, so complete them in order (Day 1 → Day 2 → Day 3 → Day 4)

2. **Read Before Running**: Each notebook contains valuable context in markdown cells. Read them before executing code.

3. **Experiment Freely**: 
   - Duplicate notebooks before major experiments
   - Try variations and modifications
   - Break things and learn from errors

4. **Take Notes**: 
   - Capture prompts that work well
   - Document parameter tweaks and outcomes
   - Record challenges and solutions

5. **Use Reference Materials**: 
   - PDF slides provide conceptual context
   - Day-specific READMEs have platform-specific setup details

### Best Practices

- ✅ **Run cells sequentially** - Later cells depend on earlier outputs
- ✅ **Keep secrets safe** - Never commit API keys or `.env` files
- ✅ **Version control** - Commit meaningful checkpoints with Git
- ✅ **Ask for help** - Join course discussion channels for support
- ✅ **Practice** - Build your own agents using the concepts learned

## 🔐 Security & Secrets Management

### What NOT to Commit

Add these to `.gitignore`:
```
.env
.venv/
__pycache__/
*.pyc
*.pyo
*.pyd
.Python
kaggle.json
*.ipynb_checkpoints
```

### Safe Practices

- ✅ Use environment variables or `.env` files locally
- ✅ Use Kaggle Secrets when running on Kaggle
- ✅ Never hardcode API keys in notebooks
- ✅ Review files before committing to Git

## 📚 Additional Resources

### Documentation
- [Google ADK Documentation](https://google.github.io/adk-docs/)
- [Gemini API Documentation](https://ai.google.dev/gemini-api/)
- [Model Context Protocol](https://modelcontextprotocol.io/)

### Course Materials
- Each day folder contains PDF slides with conceptual overviews
- Day-specific READMEs provide detailed setup instructions
- Notebooks include inline documentation and explanations

### Community Support
- Join course discussion channels (Slack/Discord)
- Kaggle forums for troubleshooting
- GitHub issues for repository-specific questions

## 🎯 Learning Path

```
Day 1: Foundation
  ↓
  Learn: Prompts, Actions, Architectures
  ↓
Day 2: Tools
  ↓
  Learn: Tool Integration, MCP, Best Practices
  ↓
Day 3: Context
  ↓
  Learn: Sessions, Memory, State Management
  ↓
Day 4: Quality
  ↓
  Learn: Observability, Evaluation, Testing
  ↓
Production-Ready Agents! 🎉
```

## 💡 Tips for Success

1. **Don't Skip Fundamentals**: Day 1 concepts are used throughout
2. **Practice Hands-On**: Run every code cell yourself
3. **Experiment Beyond Examples**: Try building your own agents
4. **Debug Actively**: When something breaks, use observability tools (Day 4)
5. **Evaluate Your Work**: Apply evaluation techniques to your own agents

## 🤝 Contributing

This is a learning repository. Feel free to:
- Add your own experiments and examples
- Share improvements and fixes
- Document your learnings
- Help others in the community

## 📝 License

This repository contains course materials from the Kaggle 5-Day AI Agents course. Please refer to individual notebooks for specific licensing information (Apache 2.0 for Google ADK materials).

## 🎓 Next Steps

After completing this course, you'll be ready to:
- Build production-ready AI agents
- Integrate agents with external tools and APIs
- Manage agent state and memory effectively
- Monitor and evaluate agent performance
- Deploy agents to production environments

**Ready to start?** Open `day 1/day-1a-from-prompt-to-action.ipynb` and begin your journey! 🚀

---

**Happy Learning!** If you have questions or need help, don't hesitate to reach out to the course community or check the documentation.
