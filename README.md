# 🛡️ VibeGuard Skill

**VibeGuard** is a universal skill & instruction set designed specifically for **Vibe Coders** using AI coding agents like **Anti-Gravity**, **Claude Code**, and **Codex / Cursor**.

---

## 🎯 The Two Core Pillars

### 1. 🚨 Proactive Risk & Safety Alerts
Prevents AI agents from silently breaking your project or burning your subscription quotas:
- **Destructive Actions (`🚨 HIGH RISK`):** Warns before modifying/deleting database tables, environment keys (`.env`), or running destructive git commands (`reset --hard`, force push).
- **Configuration Changes (`⚠️ CAREFUL`):** Alerts when major dependencies or core architecture settings are modified.
- **Quota & Token Limits (`💡 TOKEN ALERT`):** Warns you before reading huge files or running massive tasks that consume high context or risk hitting subscription rate limits.

### 2. 💬 Zero Jargon & Plain Explanations
Built for builders who care about the vibe and the product, not theoretical computer science jargon:
- **No Complex Jargon:** Bans confusing terms like AST parsing, race conditions, promise hydration, and low-level memory chatter.
- **Short & Punchy:** Explanations are kept to 2–3 plain sentences.
- **What & How-to-Test:** Tells you clearly what changed and where to click to see it working.

---

## 📁 Repository Structure

```text
├── vibe-guard/
│   └── SKILL.md       # Standard Agent Skill format (Anti-Gravity & Open Skills standard)
├── CLAUDE.md          # Ready-to-use config for Claude Code
├── .cursorrules       # Ready-to-use config for Cursor, Codex, and VS Code AI tools
└── README.md          # Setup guide and documentation
```

---

## 🚀 How to Use / Install

### 1. In Google Anti-Gravity
To make it available globally across all your Anti-Gravity sessions, copy the `vibe-guard` folder into your skills directory:
- **Global Path:** `%USERPROFILE%\.gemini\antigravity\skills\vibe-guard\`
- Or simply keep it in your workspace root under `.gemini/skills/vibe-guard/`.

Anti-Gravity will automatically discover and load the `vibe-guard` skill!

### 2. In Claude Code
Keep the [CLAUDE.md](file:///d:/skill-project/CLAUDE.md) file in the root of any project where you run `claude`. Claude Code automatically reads this file at the start of every session.

### 3. In Cursor / Codex / Copilot
Place [.cursorrules](file:///d:/skill-project/.cursorrules) in your project's root folder. Cursor / Codex will enforce these safety alerts and plain explanations across all prompt sessions.

---

## 🧪 Example in Action

### When touching the Database:
> [!WARNING]
> ### 🚨 HIGH RISK: Database Change
> **What I am about to do:** I need to reset the user table to apply the new login flow.
> **Risk:** Any test accounts in your local database will be deleted.
> **Should we make a quick backup first, or should I proceed?**

### When explaining code changes:
> **Goal:** We added a favorites button to the product cards.  
> **What changed:** Clicking the heart icon now saves the item to your favorites list so it stays there even after you refresh the page.  
> **How to test:** Open `index.html` in your browser and click on any heart icon.
