<div align="center">

<img src="https://dswa1xdat8uez.cloudfront.net/2q43l%2Fpreview%2F81605402%2Fmain_large.png?response-content-disposition=inline%3Bfilename%3D%22main_large.png%22%3B&response-content-type=image%2Fpng&Expires=1792777392&Signature=YN9myDRhOm7NEnQYCuUh04uRRglt3tA4M-9cfMIDj3MD~vXJ31We23irvB48~nzos3YvXBVIiiROTgImXSArmlsVUEYegjzyIpdwmdG~YF20gv5tXRAEXR1EZiuk9HuPxLTrubndck6xBeESbOCu9LKUSC-SL6cQLMP7Z2xGYx7elNq~V26iUtvsjdSSonodiJdpsFgNdCmwz4EBkj5n0Vc56WQrnCZ8rDXTRGYhZ1HGG062XLuXP~REK5rLwWBeEa9tGAqreT-l1Cl0Bb3fPx0AHQhEThnrdDGILcK7tv4yjEXJWbygXkXDR1bIu9fBjR5BKXvjE2xeDb7iIxkckg__&Key-Pair-Id=APKAJT5WQLLEOADKLHBQ" alt="AB ZentiumLab AI" width="100%"/>

<br/>

![Version](https://img.shields.io/badge/version-3.0-b45cff?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.14-3de1ff?style=for-the-badge&logo=python&logoColor=white)
![Cross Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-b45cff?style=for-the-badge)
![Providers](https://img.shields.io/badge/AI%20providers-15%2B-b45cff?style=for-the-badge)
![MCP](https://img.shields.io/badge/MCP-supported-3de1ff?style=for-the-badge)

**An AI coding and system assistant that lives in your terminal.**
Ask in plain language. It reads your project, edits files, runs commands, searches the web, and asks you before it does anything risky.

[Install](#-installation) · [Demo](#-see-it-in-action) · [Features](#-features) · [Commands](#-commands-cheat-sheet) · [FAQ](#-faq)

</div>

---

## ✨ What is AB ZentiumLab AI?

**AB ZentiumLab AI** is a standalone, terminal-based AI agent. You describe what you want — *"fix the failing test"*, *"find which process is using port 8080"*, *"refactor this module"* — and it gets to work: exploring your files, making changes, running your tests, and reporting back.

It runs on **Windows, Linux, and macOS**, and requires **Python 3.14** (or later).

> **Why people like it**
> - 🧠 **Bring your own model** — Claude, OpenAI, Gemini, Groq, DeepSeek, local Ollama and more. Switch any time.
> - 🛡️ **You stay in control** — risky actions always need your approval, and file changes can be undone.
> - 🖥️ **Understands your machine** — it knows your OS, shell, and package manager and uses the right commands.
> - 🔌 **Extensible** — connect MCP servers and add your own skills.

---

## 🎬 See it in action

<div align="center">
<img src="https://i.imageupload.app/a972a4bb61c3a2542cda.svg" alt="Animated terminal demo of AB ZentiumLab AI" width="100%"/>
</div>

<sub>An illustration of a typical session: the assistant searches and reads code, edits a file, runs the tests, asks permission before a system-level action, and reports the result.</sub>

---

## 🚀 Features

### 🤖 Agentic coding
| | |
|---|---|
| **Explore** | Fast file search by name or content, code outlines (classes, functions, headings), and reading large files in pages. |
| **Edit safely** | Exact replacements, multi-edit (all-or-nothing), line inserts, full-file writes, unified-diff patches, and Jupyter notebook editing. |
| **Git aware** | Status, diff, log, and show — read-only, so it can understand your history without touching it. |
| **Run & verify** | Runs your tests and builds, supports **background commands** you can check on or stop. |
| **Plan first** | `/plan` makes it investigate and propose a plan; nothing changes until you `/approve`. |
| **Task list** | It keeps a visible to-do list while it works. You can edit it too. |
| **Sub-agents** | Hands self-contained jobs to a helper with a fresh context, so long sessions stay focused. |
| **Undo** | Every turn is checkpointed. `/undo` reverts the file changes of the last turn(s). |

### 💻 System assistant
| | |
|---|---|
| **System info** | OS and distro, CPU, RAM, disks, uptime, battery, shell. |
| **Processes & services** | List, find, and stop processes. Manage services (systemd, OpenRC, launchd, Windows Services, and more). |
| **Packages** | Search, install, remove, and upgrade using your machine's **native** package manager (apt, dnf, pacman, winget, brew, and others). |
| **Admin tasks** | Runs elevated commands (sudo / UAC) — **always after your explicit approval**. |
| **Network tools** | Interfaces, ping, DNS, listening ports and the programs that own them. |
| **Environment** | Read and change environment variables and your `PATH`. |
| **Desktop helpers** | Clipboard, desktop notifications, open files/folders/URLs, screenshots. |
| **Desktop control** | Optionally move the mouse, type, and manage windows. Can be switched off. |

### 🌐 Web & browser
- **Web search with no API key** needed (multiple engines). Add a Tavily, Brave, or Serper key for even better results.
- **Page fetching** that turns web pages into clean, readable text.
- **Real browser control** — it can drive an installed Chromium-based browser (Chrome, Edge, Brave…) when a task needs it.

### 🎤 Voice
Talk instead of typing with `/voice`. Speech recognition via Groq, OpenAI, local Whisper (offline), or Google. Turn on `/speak` to have answers read aloud.

### 🔌 MCP & Skills
- **MCP (Model Context Protocol)** — connect external tool servers over stdio or HTTP, with OAuth login for remote servers. Add them with a guided wizard: `/mcp add`.
- **Skills** — drop simple Markdown instruction packs into a folder and the assistant can load them when relevant.
- **Project rules** — put your standing instructions in an `AB-ZENTIUM-LAB.md` file in your project (`AGENTS.md` and `CLAUDE.md` work too).

### 💾 Sessions
Every conversation is **auto-saved**. Continue where you left off with `/resume` or `/continue`, rename and export sessions to Markdown, and even **switch AI provider mid-conversation** — your history is converted and kept.

---

## 🧩 Works with your favourite models

<div align="center">
<img src="https://cdn.jumpshare.com/preview/ZNnZbyilxiyZh1GTGQ27iPcFjrhpu5buOdXotWMzebj7il6Ao22u4HeXdP3BiGTgssDmy1AqIZfNjiWBzlkbNzWaz42S391efyM9nFooKfk-kPHS19H4h3unf" alt="Supported AI providers" width="100%"/>
</div>

Anthropic (Claude) · OpenAI · Google Gemini · Groq · OpenRouter · Mistral · DeepSeek · xAI (Grok) · GLM (Z.ai) · Together AI · Fireworks AI · Cerebras · Perplexity · **Ollama** (local) · **LM Studio** (local) · plus **any OpenAI-compatible endpoint**.

Run `/config` for a friendly wizard that sets your provider, API key, and model. Want to stay fully offline? Pair the app with a local model through Ollama or LM Studio.

---

## 🛡️ You are always in control

<div align="center">
<img src="assets/permissions.svg" alt="Permission levels" width="100%"/>
</div>

Every action is classified by risk. **System-level and critical actions always ask you first — in every mode.** Critical approvals can never be "remembered".

| Mode | Behaviour |
|---|---|
| `auto` *(default)* | Asks only for SYSTEM and CRITICAL actions. |
| `confirm` | Also asks before every file write and command. |
| `strict` | Asks before anything that isn't read-only. |
| `readonly` | Nothing that changes anything is allowed. |

Switch any time with `/permission <mode>`. Create permanent allow/deny rules with `/allow` and `/deny`, and review everything with `/audit`.

---

## 📦 Installation

**Requirement:** Python **3.14** or later must be installed on your system.

Clone the repository first:

```bash
git clone https://github.com/ahmadbutterror404/AB-Zentium-Lab-AI.git
cd AB-Zentium-Lab-AI
```

Then pick the installer for your OS:

### 🐧 Linux / 🍎 macOS

```bash
chmod +x ./install.sh
./install.sh
```

### 🪟 Windows

**PowerShell:**
```powershell
.\install.ps1
```

**Command Prompt:**
```cmd
install.bat
```

### 🐍 Fallback — any OS with Python

If a platform script doesn't suit your setup, the Python installer works everywhere Python 3.14 runs:

```bash
python install.py
```

Each installer checks for Python 3.14+, sets up a virtual environment, installs all dependencies, and prepares the app for first run.

### ⚡ First launch
1. Run the setup wizard — it starts automatically on first run, or type `/config`.
2. Choose a **provider**, paste your **API key**, pick a **model**.
3. Start chatting. Type `/help` to see everything.

> 💡 A desktop icon / menu entry is created for you where supported. You can add or remove it any time with `/install` and `/uninstall`.

---

## ⌨️ Commands cheat sheet

Type these inside the app.

| Group | Command | What it does |
|---|---|---|
| **Session** | `/resume` · `/continue` · `/sessions` | Pick up a previous conversation |
| | `/undo [n]` | Revert file changes of the last *n* AI turns |
| | `/compact` | Summarise older turns to free up context |
| | `/export [file.md]` · `/rename <title>` · `/reset` | Export, rename, or start fresh |
| | `/usage` · `/about` · `/doctor` · `/clear` | Token usage, about, environment check, clear screen |
| **Model** | `/config` | Wizard: provider, API key, model, custom endpoint |
| | `/provider <name>` · `/model <name>` | Switch (your conversation is kept) |
| | `/models [live]` · `/key [provider]` | List models · set an API key |
| **Files** | `/workspace [path]` | Show or change the working folder |
| | `/attach` · `/upload` · `@path` | Attach files or images to a message |
| **Agent** | `/plan` · `/approve` · `/reject` · `/plan-off` | Plan-first workflow |
| | `/todos` · `/todo add\|done\|rm` | View or edit the task list |
| | `/permission <mode>` · `/allow` · `/deny` · `/rules` · `/audit` | Safety controls |
| | `/tools [group on\|off]` · `/skills` | Toggle tool groups, list skills |
| **MCP** | `/mcp` · `/mcp add` · `/mcp auth <name>` · `/mcp doctor <name>` | Manage MCP servers |
| **Voice** | `/voice [on\|off\|once\|test]` · `/speak on\|off` | Talk to it / hear answers |
| **System** | `/install` · `/uninstall` · `/logo` · `/browser` · `/search <query>` | Icon, branding, browser, web search |

### Launch options
Run the program from a terminal with these flags:

| Flag | Meaning |
|---|---|
| `"your request"` | One-shot mode: run a single prompt and exit |
| `-p`, `--provider` | Choose provider for this run |
| `-m`, `--model` | Choose model for this run |
| `-w`, `--workspace` | Work in a specific folder |
| `--permission <mode>` | Set permission mode for this run |
| `--resume` · `--continue` | Resume a session / continue the last one |
| `--plan` | Start in plan mode |
| `--voice` | Start with voice input on |
| `--setup` | Open the setup wizard |
| `--install` · `--uninstall` | Add / remove desktop icon and menu entry |
| `--doctor` | Check your environment |
| `--version` | Show the version |

**Example**
```bash
./AB-ZentiumLab-AI -w ~/projects/my-api --permission confirm "find and fix the failing tests"
```

---

## 📁 Where is my data?

The app keeps settings, API keys, sessions, skills, and logs in one tidy folder:

| OS | Location |
|---|---|
| Windows | `%APPDATA%\AB-ZentiumLab-AI` |
| Linux / macOS | `~/.config/AB-ZentiumLab-AI` |

Set the `AB_ZENTIUM_LAB_HOME` environment variable to use a different location. Your API keys are stored **only on your computer**, in a private file in that folder.

---

## ❓ FAQ

<details>
<summary><b>What do I need before installing?</b></summary>

Python **3.14** or later. Everything else (virtual environment, dependencies) is handled automatically by the installer scripts.
</details>

<details>
<summary><b>Is it free? Do I need an API key?</b></summary>

The app is free to use. To talk to a cloud AI model you need an API key from that provider (billing is between you and them). If you use a local model with **Ollama** or **LM Studio**, no key is needed.
</details>

<details>
<summary><b>Can it delete my files or break my system?</b></summary>

It can only act through its tools, and risky ones need your approval. File changes made by the assistant are checkpointed so you can `/undo` them, and deletions go to a recoverable trash inside your workspace. Still, AI can make mistakes — start in `confirm` or `readonly` mode if you want extra caution, and keep backups of important work.
</details>

<details>
<summary><b>Does it work offline?</b></summary>

With a local model (Ollama / LM Studio) and local Whisper for voice, yes. Web search and fetching naturally need internet.
</details>

<details>
<summary><b>Which languages can I talk in?</b></summary>

The assistant replies in the language you write in — English, Urdu, Roman Urdu, and many more, depending on the model you choose.
</details>

<details>
<summary><b>Something isn't working. What do I do?</b></summary>

Run `/doctor` (or `--doctor`) for an environment check, then open an [issue](https://github.com/ahmadbutterror404/AB-Zentium-Lab-AI/issues) and include its output. Please **remove any API keys** before pasting logs.
</details>

---

## ⚠️ Responsible use

AB ZentiumLab AI can run commands, change files, install software, and control your desktop **on your behalf**. Review what it asks to do before approving, especially for SYSTEM-level actions. You are responsible for the actions you approve. The software is provided **"as is"**, without warranty of any kind.

---

## 👤 Author

**Ahmad Butt**

[![GitHub](https://img.shields.io/badge/GitHub-ahmadbutterror404-181717?style=flat-square&logo=github)](https://github.com/ahmadbutterror404)
[![Instagram](https://img.shields.io/badge/Instagram-@ahmadbutt3137-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://instagram.com/ahmadbutt3137)
[![Email](https://img.shields.io/badge/Email-ahmadbutterror4004%40gmail.com-b45cff?style=flat-square&logo=gmail&logoColor=white)](mailto:ahmadbutterror4004@gmail.com)
[![Email](https://img.shields.io/badge/Email-ahmadbutterror404%40outlook.com-0078D4?style=flat-square&logo=microsoftoutlook&logoColor=white)](mailto:ahmadbutterror404@outlook.com)

---

<div align="center">

If this project helps you, please consider giving it a ⭐ — it really helps!

<sub>Made with 💜 by Ahmad Butt</sub>

</div>
