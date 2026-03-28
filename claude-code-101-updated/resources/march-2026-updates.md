# 🆕 March 2026 — What's New in Claude Code

> Last updated: March 28, 2026 | Sources: TechCrunch, Anthropic Official, Builder.io

This file tracks every major Claude Code update shipped in March 2026. Bookmark it — things are moving fast.

---

## 🎤 Voice Mode — Ship Date: March 3, 2026

Claude Code now supports push-to-talk coding directly in your terminal.

**How to use it:**
```bash
/voice        # toggle voice mode on/off
# Hold SPACE to speak → release to send
# Supports 20 languages
```

**What you need to know:**
- Rolling out gradually — check your welcome screen for access
- Works across macOS, Linux, and Windows
- Covered by: [TechCrunch (March 3, 2026)](https://techcrunch.com/2026/03/03/claude-code-rolls-out-a-voice-mode-capability/)

---

## 🤖 Auto Mode — Ship Date: March 24, 2026

Instead of you approving every single action manually, an AI classifier reviews each action and auto-approves safe ones while blocking risky ones.

**What this means for beginners:**
- No more clicking "approve" on every file change
- Risky actions (deleting files, running dangerous commands) still require your approval
- Works with Claude Sonnet 4.6 and Opus 4.6 only
- Currently in **research preview** — best used in sandboxed/test environments

Covered by: [TechCrunch (March 24, 2026)](https://techcrunch.com/2026/03/24/anthropic-hands-claude-code-more-control-but-keeps-it-on-a-leash/)

---

## 🔁 `/loop` — Scheduled Recurring Tasks

Run any prompt on a timer — like a background cron job inside Claude Code.

```bash
/loop 5m check if the deploy succeeded    # every 5 minutes
/loop 1h run the full test suite          # every hour
/loop 20m summarize new issues            # loop over any task
```

**Notes:**
- Tasks are session-scoped (expire after 3 days)
- Interval supports: `s`, `m`, `h`, `d` units
- Defaults to 10 minutes if no interval specified

---

## 🖥️ Remote Control — March 2026

Control your desktop Claude Code session from your phone.

**How it works:**
1. Run `/remote-control` (or `/rc`) in your terminal session
2. Scan the QR code with your Claude mobile app
3. Send instructions from your phone → Claude executes on your Mac

**Real use case:** Start a long refactor, go to a meeting, check progress and send new instructions from your phone.

Available on: Pro and Max subscribers

---

## 📐 New Commands Added in March 2026

| Command | What It Does |
|---------|-------------|
| `/voice` | Toggle push-to-talk voice mode |
| `/loop [interval] [task]` | Schedule a recurring background task |
| `/rc` or `/remote-control` | Start a remote control session via mobile |
| `/simplify` | Detect over-engineering in changed code and auto-fix |
| `/batch` | Large-scale refactors using parallel agents |
| `/insights` | Usage analytics and optimization report |
| `/status` | See session state and context usage |
| `/context` | Detailed token usage breakdown |
| `/tasks` | Monitor background loop tasks |
| `/effort` | Set reasoning depth (low / medium / high) |

---

## 📊 March 2026 By The Numbers

- **$2.5 billion** run-rate revenue — more than doubled since January 2026
- **Weekly active users doubled** since January 2026
- **4% of all public GitHub commits** made by Claude Code (~135,000/day)
- **40.8% developer adoption** — 4th most-used AI dev tool (Stack Overflow Survey)
- Claude mobile app hit **#1 on the US App Store** in March 2026

---

## 🔗 Official Sources

- [Claude Code Official Changelog](https://docs.anthropic.com/en/release-notes/claude-code)
- [Anthropic News](https://www.anthropic.com/news)
- [TechCrunch: Voice Mode (March 3)](https://techcrunch.com/2026/03/03/claude-code-rolls-out-a-voice-mode-capability/)
- [TechCrunch: Auto Mode (March 24)](https://techcrunch.com/2026/03/24/anthropic-hands-claude-code-more-control-but-keeps-it-on-a-leash/)
