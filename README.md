# 🦞 JarvisComparisons

Visual side-by-side comparisons for technical decisions. Dark-themed, color-coded, mobile-friendly.

---

## Comparisons

### 1. [Hub API vs Heartbeat/Cron Flow](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/hub-vs-heartbeat-flow.html)
How messages reach WhatsApp through two different OpenClaw paths — the Chat Completions API (what the Hub uses) vs the built-in Heartbeat/Cron system. Same brain, different plumbing.

### 2. [Memory Search Options](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/memory-search-options.html)
Three approaches to searching AI memory files — keyword matching (current), Voyage AI cloud embeddings (OpenClaw built-in), and local embeddings via fastembed (what LocalGPT uses).

### 3. [Full IDS vs Lightweight Stack](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/ids-comparison.html)
OSSEC/Wazuh (full IDS platform) vs the lightweight combo of AIDE + psad + auditd. Resource usage, features, setup complexity, and when to use each.

### 4. [OpenClaw Security Architecture Deep Dive](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/openclaw-sandboxing-deep-dive.html)
Gateway vs Main Agent vs Sub-Agent — full comparison of trust levels, Docker's 48 blocked syscalls mapped to OpenClaw impact, and what the community says about restricting AI agents.

### 5. [Secrets Management — Plain Files vs Encrypted vs Vault](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/secrets-management-comparison.html)
Five approaches to managing secrets on a VPS: plain .env + permissions (current), systemd credentials, SOPS+age, HashiCorp Vault, and environment-only. Shows what we already cover (~80%).

### 6. [VPN Scenarios — No VPN vs WireGuard vs VPS Gateway vs NordVPN](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/vpn-scenarios-comparison.html)
Four VPN approaches for an OpenClaw VPS: hardened Linux only, local WireGuard on same machine, separate VPS as WireGuard gateway, and commercial VPN (NordVPN). Includes attack scenario matrix and inbound vs outbound IP visibility breakdown.

### 7. [Tor × OpenClaw — Can an AI Agent Live on the Dark Web?](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/tor-openclaw-comparison.html)
Three Tor integration scenarios for an AI assistant: half Tor (split routing for research), full Tor (everything through onion routing — spoiler: everything dies), and half Tor + VPN gateway (the paranoid's dream). Includes OpenClaw service compatibility matrix.

### 8. [Cron vs Heartbeat — Timing, Sessions & Delivery](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/cron-heartbeat-docs.html)
Complete reference for OpenClaw's scheduling system: Cron jobs (exact times, isolated sessions, manual/one-shot reminders) vs Heartbeats (periodic checks with main session context). Covers all config options including sessionTarget, payload types (systemEvent vs agentTurn), delivery modes, ackMaxChars threshold, lightContext, isolatedSession, and how response delivery actually works.

### 9. [OpenClaw Personalization — Messages, Reasoning & Thinking](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/openclaw-personalize-messages.html)
Complete guide to OpenClaw's personalization layers: Messages (queue modes, debounce, ack reactions, TTS), Reasoning (on/off/stream visibility), and Thinking (effort levels from off to xhigh). Includes practical config examples for WhatsApp bots, debug mode, and group chat optimization.

### 10. [Hooks vs Plugins — When to Use Which](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/hooks-plugins-comparison.html)
Lightweight event-driven scripts (Hooks) vs full npm packages (Plugins) — what's built-in, what's for external integrations, and how to choose.

### 11. [Messaging Paths — message vs chat/completions vs sessions_send](https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/messaging-context-paths-comparison.html)
Three-way comparison for OpenClaw messaging/control flow, with explicit context-awareness per option. Covers when to use the public `message` tool, how `/v1/chat/completions` becomes context-aware only with stable sessions, and why `sessions_send` is ideal for isolated-cron handoff into main context.

---

## Style Guide

See [HowAriLikeCompare.md](HowAriLikeCompare.md) — the design philosophy behind these comparisons.

**TL;DR:** Dark theme, color-coded cards, specs before opinions, clear verdict. Single HTML files, no dependencies.

---

Built by Jarvis de la Ari & Ariel @ Bresleveloper AI 🦞


---

[![YouTube](https://img.shields.io/badge/YouTube-BresleveloperAI-red?logo=youtube)](https://www.youtube.com/@BresleveloperAI/videos)

[ישראלי/דובר עברית? כנס ליוטיוב שלי לתכנים נוספים על בינה מלאכותית (לא לשכוח להרשם ♥, פעמון ♥, לייק ♥, ולשלוח לחבר ♥♥♥)](https://www.youtube.com/@BresleveloperAI/videos)
