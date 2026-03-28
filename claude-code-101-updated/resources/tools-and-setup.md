# 🛠️ Tools, Setup & Tips

> Everything you need to install Claude Code and get productive fast. Updated March 2026.

---

## ✅ What You Need Before Starting

| Tool | Purpose | Cost | Link |
|------|---------|------|------|
| **Claude Pro** | Powers Claude Code — required | $20/mo | [claude.ai](https://claude.ai) |
| **Node.js** | Required runtime | Free | [nodejs.org](https://nodejs.org) |
| **VS Code** | Best beginner-friendly code editor | Free | [code.visualstudio.com](https://code.visualstudio.com) |
| **Git** | Safety net — tracks every change Claude makes | Free | [git-scm.com](https://git-scm.com) |

**Can I use the free Claude plan?**
No. Claude Code requires Claude Pro ($20/mo), Claude Max ($100/mo), or API credits. Pro is enough for most beginners.

---

## 📦 Installing Claude Code (March 2026 Method)

> ⚠️ **Important:** Many older tutorials say `npm install -g @anthropic-ai/claude-code`. While it still works, the official docs now recommend the **native installer** for better performance.

### macOS / Linux
```bash
# Option 1 — Native installer (recommended)
# Visit https://claude.ai/code and follow the installer for your OS

# Option 2 — npm (still works)
npm install -g @anthropic-ai/claude-code
```

### Windows
```
Download the Windows installer from: https://claude.ai/code
Run as Administrator
```

### System Requirements
- **macOS:** 13.0+ (Intel or Apple Silicon)
- **Windows:** Windows 11 (or Windows 10 version 1809+ via WSL2)
- **Linux:** Ubuntu 22.04+, Debian 12+
- **RAM:** Minimum 4 GB (8 GB recommended)
- **Internet:** Stable connection required

### First Run
```bash
cd your-project-folder    # navigate to any project
claude                    # start Claude Code
# Browser opens for one-time login via claude.ai
# Credentials stored locally — no need to log in again
```

---

## 🔌 VS Code Extensions

| Extension | What It Does |
|-----------|-------------|
| **Claude Code** (official Anthropic) | Inline diffs, real-time change sidebar, context sharing |
| **GitLens** | See exactly what Claude changed and when |
| **Prettier** | Auto-formats code Claude writes |

---

## 🧠 CLAUDE.md Quick Setup

The single highest-impact thing you can do in your first session:

```bash
/init   # auto-generates CLAUDE.md based on your project structure
```

**What to keep in CLAUDE.md:**
- Build / run / test commands
- Code style preferences different from defaults
- Architectural decisions Claude can't infer from the code
- Project-specific gotchas

**What to delete from CLAUDE.md:**
- Anything Claude could figure out by reading your code
- Generic advice that applies to every project

**File locations:**
- `~/.claude/CLAUDE.md` — global preferences, applies to all projects
- `./CLAUDE.md` — project-level, commit to git to share with your team
- `CLAUDE.local.md` — personal overrides, add to `.gitignore`

**Deep dive:** [CLAUDE.md Design Guide — ClaudeWorld (March 20, 2026)](https://claude-world.com/tutorials/s17-claude-md-design/)

---

## ⚡ Sonnet vs Opus — When to Use Which

A practical model-switching strategy:

- **Sonnet 4.6** → Use for 80% of tasks. Fast, cost-effective, handles everyday coding well.
- **Opus 4.6** → Switch for the other 20%. Complex multi-file refactoring, architectural decisions, hard debugging, Agent Teams.

```bash
/model          # switch models inside a session
/effort high    # trigger deep reasoning without switching models
```

> The `think` keyword also triggers adaptive deep reasoning on Opus 4.6.

---

## 🛡️ Safety Tips for Beginners

**Always commit before big changes:**
```bash
git commit -m "checkpoint before Claude refactor"
```

**Use Plan Mode before large changes:**
```bash
/plan
Refactor the entire auth module to use JWT tokens
# Claude lists every file it will touch → you approve → then it acts
```

**Context management:**
- At ~70% context → `/compact focus on [what matters]`
- At ~90% context → `/clear` and start fresh
- Check usage anytime with `/status` or `/context`

---

## 🔧 Useful Community Tools

| Tool | What It Does | Link |
|------|-------------|------|
| **Claude Code Ultimate Guide Cheatsheet** | Full command reference, updated March 2026 | [GitHub](https://github.com/FlorianBruniaux/claude-code-ultimate-guide) |
| **claude-code-best-practice** | Community best practices collection | [GitHub](https://github.com/shanraisshan/claude-code-best-practice) |
| **claude-code-tips** (ykdojo) | 45 advanced tips | [GitHub](https://github.com/ykdojo/claude-code-tips) |
| **claudecodetube.dev** | Find tutorials by topic and skill level | [Website](https://claudecodetube.dev) |
| **roadmap.sh/claude-code** | Step-by-step visual learning path | [Website](https://roadmap.sh/claude-code) |
