# Personal OS — Research-Grade Life Operating System

> *Design once. Execute cheaply. Let compounding do the rest.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Made with HTML](https://img.shields.io/badge/Built%20with-HTML%2FCSS%2FJS-orange.svg)]()
[![No dependencies](https://img.shields.io/badge/Dependencies-none-brightgreen.svg)]()
[![GitHub Pages](https://img.shields.io/badge/Deployed-GitHub%20Pages-blue.svg)]()

A single-file, zero-dependency personal productivity system built on the principle that **systems beat willpower**. Inspired by research workflows at top institutions — where output quality depends not just on effort, but on how that effort is structured.

**[→ Live Demo](https://duanbiao2000.github.io/personal-os)**

---

## The Problem This Solves

Most productivity advice optimizes for motivation. Motivation is volatile.

This system optimizes for **low marginal execution cost** — the upfront investment in SOPs, templates, and calendar architecture reduces the daily cognitive overhead of *deciding what to do* so you can spend that budget on *actually doing it*.

```
Without system:  each day starts from scratch → high decision fatigue → inconsistent output
With system:     each day runs on autopilot   → low decision fatigue → compounding output
```

---

## What's Inside

The system is organized into five modules, accessible via tab navigation:

| Module | Contents | Time Cost |
|--------|----------|-----------|
| **Overview** | Design principles, system architecture, operating constraints | Read once |
| **Daily SOPs** | Morning Boot · Deep Work Block · Shutdown Ritual | 35 min/day |
| **Templates** | Daily Log · Weekly Plan · Project Scaffold · Decision Log | Fill brackets |
| **Calendar** | Ideal week structure, themed days, meeting hygiene rules | Set up once |
| **Weekly Review** | 45-min Friday protocol, 4-week activation roadmap | 45 min/week |

---

## Quick Start

### Option 1 — Use directly (zero setup)

```bash
# Clone and open
git clone https://github.com/your-username/personal-os.git
open personal-os/index.html
```

### Option 2 — GitHub Pages (recommended)

1. Fork this repository
2. Go to **Settings → Pages**
3. Set Source to `main` branch, `/ (root)`
4. Access at `https://your-username.github.io/personal-os`
5. Bookmark it. Add to phone home screen.

### Option 3 — Direct download

Download [`index.html`](./index.html) → open in any browser. Works offline, no server needed.

---

## System Architecture

```
Personal OS
│
├── Layer 1: Daily Rhythm          (3 fixed anchors × every day)
│   ├── Morning Boot               20 min — preview, pre-load, intention
│   ├── Deep Work Blocks           2 × 90 min — protected, ritualized
│   └── Shutdown Ritual            15 min — capture, close loops, pre-load tomorrow
│
├── Layer 2: Weekly Architecture   (2 bookends × every week)
│   ├── Monday Planning            45 min — load week, pre-schedule DW blocks
│   └── Friday Review              45 min — process, calibrate, pre-load next week
│
├── Layer 3: Project Templates     (scaffold × every new project)
│   ├── Project Scaffold           North star, DoD, milestones, progress log
│   └── Decision Log               Context, options, review trigger
│
└── Layer 4: Quarterly Calibration (2hr × every ~12 weeks)
    └── OKR review + 90-day reset
```

**Core numbers:** 4h peak deep work/day · 90-min work blocks · 3 MIT tasks/day max · 52 weekly reviews/year

---

## Design Principles

The system is built on five constraints that prevent collapse under load:

1. **Capture everything, process once** — one inbox, fixed processing times, nothing lives in your head
2. **Time-box before you to-do** — tasks go on the calendar, not a list; a list is a wish
3. **Protect the first 90 minutes** — no email or meetings before Deep Work Block 1 completes
4. **Distinguish doing from deciding** — planning sessions decide; work blocks execute; never mix
5. **Debt-free closure** — every day ends with open loops converted to scheduled actions

---

## Calendar Logic

Themed days reduce context-switching cost. Research suggests 15–25 min recovery time per context switch.

```
Monday    → Planning day     (week preview, no meetings before noon)
Tuesday   → Deep work day    (no meetings AM, admin PM)
Wednesday → Collaboration    (meeting window, 1:1s, async catch-up)
Thursday  → Deep work day    (mirror of Tuesday)
Friday    → Review + close   (weekly review, pre-load next week)
```

**Email policy:** twice daily at 11:30 and 16:00. Continuous monitoring is the enemy of deep work.

**Meeting rules:** written agenda 24h prior · default 30 min not 60 · written next actions + owner at close · no agenda = decline or convert to async.

---

## Adapting to Your Context

This is a starting template, not a prescription. Common adaptations:

**For researchers / PhD students**
- Deep Work Block 1 = writing/analysis (highest leverage)
- Deep Work Block 2 = reading/literature (second priority)
- Wednesday meetings = advisor meetings, seminars, lab

**For founders / operators**
- Collapse Wednesday meetings to Tuesday PM
- Add a "fire-fighting buffer" block daily (30 min)
- Weekly review adds team status sweep

**For individual contributors**
- Add standup to the calendar template
- Protect at least one 90-min block from meeting creep
- Use the project scaffold for every multi-week initiative

---

## File Structure

```
personal-os/
└── index.html          # Entire system — single file, zero dependencies
└── README.md           # This file
```

That's it. The entire system is one HTML file. No build step, no npm, no framework.

---

## Customization

Everything is in a single `<style>` block at the top of `index.html` with CSS variables:

```css
:root {
  --accent: #c8401a;     /* Primary accent color */
  --accent2: #2d5a8e;    /* Secondary accent */
  --paper: #f5f2eb;      /* Background */
  --ink: #0f0e0c;        /* Text */
}
```

To add a new template: copy any `.template-box` block and fill in your fields. To add a new SOP: copy any `.sop-block` and add `.step-item` elements.

---

## The 4-Week Activation Roadmap

Don't implement everything at once. Staged rollout:

| Week | Action | Time investment |
|------|--------|-----------------|
| W1 | Install Morning Boot + Shutdown Ritual only | 35 min/day |
| W2 | Add 2×90 min Deep Work blocks to calendar | +180 min/day |
| W3 | Run first Weekly Review on Friday | +45 min/week |
| W4 | Full system live: templates + calendar theming | Maintenance mode |

---

## Contributing

Contributions welcome. Especially:

- **Adaptations** for specific contexts (academia, startups, creative work)
- **Template additions** that fill gaps in the current set
- **Translations** — the system should be accessible in any language

Please open an issue before submitting a large PR to align on direction.

---

## References & Influences

This system synthesizes ideas from:

- Cal Newport — *Deep Work*, *Time Block Planner*
- David Allen — *Getting Things Done* (capture/process separation)
- Andy Grove — *High Output Management* (leverage-based prioritization)
- Research on cognitive switching costs (Rubinstein, Meyer & Evans, 2001)
- Huberman Lab — ultradian rhythm research (90-min focus cycles)

---

## License

MIT License — use freely, adapt openly, attribution appreciated but not required.

---

*Built with the conviction that a well-designed system is an act of respect for your own time.*
