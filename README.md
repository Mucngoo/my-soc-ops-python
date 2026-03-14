# 🎯 Soc Ops

> **The Social Icebreaker Game That Actually Works**

Break the ice at your next mixer with a modern, interactive bingo game. Find people who match your questions and get 5 in a row to win! Perfect for conferences, meetups, team events, and networking sessions.

## 🚀 Get Started in 60 Seconds

```bash
uv sync && uv run uvicorn app.main:app --reload
```

Then open **[http://localhost:8000](http://localhost:8000)** and start playing!

---

## ✨ Features

🎮 **Interactive Bingo Board** — Smooth, responsive gameplay powered by modern web tech  
👥 **Real-Time Networking** — Connect people through thoughtfully crafted questions  
🎨 **Beautiful UI** — Clean, engaging design that works on any device  
⚡ **Fast & Lightweight** — Built with FastAPI + HTMX for instant interactions  
🧪 **Fully Tested** — Comprehensive test suite ensures reliability  
📚 **Learning Lab** — Step-by-step guide to building with AI agents  

---

## 🎮 Try It Out

**[▶️ Play the Live Game](https://madebygps.github.io/vscode-github-copilot-agent-lab/)** | **[📖 View the Full Lab Guide](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/)**

---

## 📚 Complete Learning Path

Take the interactive lab to master advanced AI agent techniques:

| Step | Title | What You'll Learn |
|------|-------|---|
| **00** | [Overview & Checklist](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Project goals and setup verification |
| **01** | [Setup & Context Engineering](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Environment setup and AI agent configuration |
| **02** | [Design-First Frontend](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Building UIs with design agents |
| **03** | [Custom Quiz Master Agent](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Creating specialized agents for specific tasks |
| **04** | [Multi-Agent Development](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Coordinating multiple AI agents efficiently |

**[📖 Start the Lab](https://madebygps.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview)** | **[📝 Offline Guides](workshop/)**

---

## 🛠️ Development

### Requirements

- **[Python 3.13](https://www.python.org/downloads/)** or higher
- **[uv](https://docs.astral.sh/uv/)** package manager ([install guide](https://docs.astral.sh/uv/getting-started/installation/))

### Quick Start

```bash
# Install dependencies
uv sync

# Run the app
uv run uvicorn app.main:app --reload
```

Open **[http://localhost:8000](http://localhost:8000)** in your browser.

### Testing & Quality

```bash
# Run tests
uv run pytest

# Check code style
uv run ruff check .

# Auto-format code
uv run ruff format .
```

---

## 🚀 Deployment

This project auto-deploys to **GitHub Pages** on every push to `main`. The live version is always up-to-date!

---

## 🤝 Contributing

Found a bug? Have a feature idea? We'd love your help! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 📄 License

MIT License — See [LICENSE](LICENSE) for details.
