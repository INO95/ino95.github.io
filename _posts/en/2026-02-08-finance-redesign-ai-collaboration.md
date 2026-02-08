---
layout: post
title: "Finance Webapp Redesign: AI Role Specialization in Practice"
date: 2026-02-08
categories: [project]
tags: [finance, ui-ux, portfolio, ai-collaboration, codex, gemini, antigravity]
lang: en
---

# Finance Webapp Redesign: AI Role Specialization in Practice

## Project Summary
This iteration focused on redesigning the finance webapp UI while keeping backend APIs and data models unchanged.  
The key objective was not only visual improvement, but also building a repeatable AI collaboration workflow for production work.

## Why This Case Matters
- Many teams use one model for everything and lose quality.
- In this project, I separated AI roles by strength:
  - **Gemini 3 Pro**: visual direction and redesign proposals
  - **Codex**: controlled implementation with minimal diffs
  - **Antigravity (+ Nano Banana 2)**: workflow orchestration and visual asset support
- This reduced rework and made output quality more stable.

## Role Split and Decision Logic
### 1) Gemini 3 Pro for design proposals
- Used for concept exploration, information hierarchy, and visual consistency.
- Best for quickly comparing alternatives before code changes.

### 2) Codex for implementation
- Applied only the accepted proposal (hybrid C + A).
- Constraint enforced: no API/data structure changes.
- Delivered predictable code-level edits and mobile breakage checks.

### 3) Antigravity for operation support
- Used for process coordination and asset handling.
- Visual materials (including Nano Banana 2 outputs) were managed as presentation-ready artifacts.

## Execution Process
1. Define redesign scope and constraints.
2. Generate multiple design proposals with Gemini 3 Pro.
3. Select final direction (hybrid C + A).
4. Implement with Codex under minimal-diff policy.
5. Capture desktop/mobile screenshots for portfolio.
6. Publish to GitHub Pages and sync project record to Notion.

## Outcomes
- Clear visual hierarchy and cleaner component balance.
- Mobile viewport (390px) verified without layout breakage.
- Portfolio-ready screenshots generated in desktop and mobile variants.
- Reusable AI division workflow documented for future projects.

## Screenshots
![Finance redesign desktop](/images/portfolio/finance-redesign-desktop-2026-02-08.png)
![Finance redesign mobile](/images/portfolio/finance-redesign-mobile-2026-02-08.png)

## Source Repositories
- Workspace source: [INO95/moltbot-workspace-202602](https://github.com/INO95/moltbot-workspace-202602)
- Blog source: [INO95/ino95.github.io](https://github.com/INO95/ino95.github.io)

## Professional Takeaway
This project demonstrates practical AI orchestration: choosing the right model for the right stage, then enforcing engineering constraints during implementation.  
The result is not just a better UI, but a scalable production process.
