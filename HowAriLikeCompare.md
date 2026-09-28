# HowAriLikeCompare.md — The Comparison Style Guide

*How Jarvis makes comparisons that Ariel actually wants to read.*

---

## The Philosophy

Ariel doesn't want a wall of text. He doesn't want a markdown table on WhatsApp. He wants to **see** the difference — visually, instantly, without reading an essay first.

These comparisons are designed to answer one question fast: **"What are my options and which one should I pick?"**

## Design Principles

### 1. Dark Theme, Always
Navy/dark backgrounds. Easy on the eyes. Looks good on mobile screenshots. Matches the dev aesthetic.

### 2. Color-Coded Sides
Each option gets its own color identity throughout the entire comparison — headers, values, borders, badges. You should be able to tell which column you're reading from the color alone.

### 3. Cards, Not Tables
Side-by-side cards. Each option is self-contained — you can read one card top to bottom without cross-referencing. Tables force horizontal scanning. Cards flow naturally.

### 4. Specs First, Opinions Later
Lead with the hard facts — cost, setup, dependencies, performance. Then follow with pros/cons. Let the reader form their own opinion from specs, then validate with yours.

### 5. Tags for Quick Scanning
Green/yellow/red tags for values like cost, quality, difficulty. The eye catches color faster than text. A green "Free" tag communicates more instantly than the word "free" in a sentence.

### 6. One Verdict
End with a clear recommendation. Not wishy-washy "it depends" — give a real opinion. "Right now X, when we scale Y, quick win Z." Ariel wants direction, not diplomacy.

### 7. The "How It Works" Section
When comparing technical options, add a short visual explainer of the less obvious one. 4 boxes, one sentence each. Demystify without drowning in detail.

### 8. Standalone HTML
Single self-contained HTML file. No external CSS, no JS frameworks, no build step. Copy the file anywhere and it renders. Screenshot it for WhatsApp. Link it from GitHub via htmlpreview.

## Structure Template

```
Title + Subtitle
├── Side-by-side cards (2-3 options)
│   ├── Badge (what category: current / built-in / new approach)
│   ├── Name + icon
│   ├── One-line description
│   ├── Spec list (label: value with color tags)
│   ├── Pros (green checkmarks)
│   └── Cons (red X marks)
├── How It Works (optional, for technical comparisons)
│   └── 2-4 boxes explaining the less obvious option
└── Verdict
    └── Clear recommendation with context
```

## What NOT to Do

- No markdown tables (WhatsApp can't render them)
- No walls of text before the comparison starts
- No "it depends" without a follow-up recommendation
- No external dependencies (fonts, CDNs, frameworks)
- No light themes
- Don't compare more than 3-4 options (cognitive overload)
- Don't hide the trade-offs — Ariel respects honesty over salesmanship

## When to Make a Comparison

- Ariel asks "what are my options?"
- There's a technical decision with real trade-offs
- Two or more approaches exist and the winner isn't obvious
- Explaining architecture differences (like Hub vs Heartbeat)
- Research tasks that end with a recommendation

## Checklist — Every Comparison Must

1. **Security scan before push** — check the HTML for leaked IPs, ports, usernames, paths, tokens, or any private infra detail. Strip anything found.
2. **Add to README** — include the comparison in the repo README with an htmlpreview.github.io link: `https://htmlpreview.github.io/?https://github.com/bresleveloper-ai-agents/JarvisComparisons/blob/main/<filename>.html`
3. **Push to repo** — commit and push to JarvisComparisons. No comparison is done until it's pushed.

---

*This is a living document. Update it when the style evolves.*
