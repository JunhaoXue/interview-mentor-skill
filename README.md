<p align="center">
  <h1 align="center">Interview Mentor Skill</h1>
  <p align="center">
    Your AI-powered interview mentor — not a generic question bank, but an adaptive system that gets sharper the more you use it.
  </p>
</p>

<p align="center">
  <a href="https://github.com/JunhaoXue/interview-mentor-skill/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-green?style=for-the-badge" alt="License"></a>
  <a href="#commands"><img src="https://img.shields.io/badge/commands-14-blue?style=for-the-badge" alt="Commands"></a>
  <a href="#supported-languages"><img src="https://img.shields.io/badge/languages-8-orange?style=for-the-badge" alt="Languages"></a>
  <a href="https://github.com/JunhaoXue/interview-mentor-skill/stargazers"><img src="https://img.shields.io/github/stars/JunhaoXue/interview-mentor-skill?style=for-the-badge" alt="Stars"></a>
</p>

<p align="center">
  Works with: <strong>Claude Code</strong> · <strong>OpenAI Codex</strong> · <strong>Any SKILL.md Agent</strong>
</p>

---

> **3 steps to start:** `git clone` → `mv SKILL.md CLAUDE.md` → say **"kickoff"**
>
> Share your resume, and you're being mentored in under 2 minutes.

---

## Why Interview Mentor?

Most interview prep tools give you the same advice regardless of your patterns. Interview Mentor is different:

- It **scores you on 5 dimensions**, tracks your scores over time, and diagnoses root causes behind weak spots
- It builds a **storybank with thinking depth** — not just WHAT you did, but HOW you thought through it
- It transforms your resume into **proof of impact** and your career into **a coherent narrative**
- It adapts its mentoring based on what the data reveals — **every candidate gets a different path**
- It remembers your previous sessions and **gets sharper the more you use it**

---

## Quick Start

### Claude Code (recommended)

```bash
git clone https://github.com/JunhaoXue/interview-mentor-skill.git
cd interview-mentor-skill
mv SKILL.md CLAUDE.md
```

Open in Claude Code and say `kickoff`.

### OpenAI Codex

```bash
git clone https://github.com/JunhaoXue/interview-mentor-skill.git
cd interview-mentor-skill
mv SKILL.md AGENTS.md
```

Open in Codex and say `kickoff`.

The mentor asks for your resume, target role, and timeline — then builds your profile, assesses your starting point, and gives you a prioritized action plan. Everything saves automatically to `mentoring_state.md`.

---

## What It Does

### Resume & Career Positioning

| Feature | What You Get |
|---------|-------------|
| **Resume Optimization** | Audit every bullet for delivery proof, thinking visibility, and skill signal. Rewrite with impact-first framing. JD-targeted versions for specific applications. |
| **Career Narrative** | Build a coherent arc connecting every role. Transition bridges for "why did you leave?". Recurring themes. Elevator pitches at 15s / 30s / 60s / 90s. |
| **STAR-T Storybank** | STAR + Thinking depth: every story captures the hard part, alternatives considered, why this approach, and lessons learned. Includes earned secrets and rapid-retrieval drills. |

### Interview Preparation & Practice

| Feature | What You Get |
|---------|-------------|
| **5-Dimension Scoring** | Substance · Structure · Relevance · Credibility · Differentiation — calibrated to your seniority level, with root cause diagnosis. |
| **8-Stage Drill System** | Constraint ladders → pushback → pivot → gap handling → role-specific → panel → stress → technical. Gated progression — you advance when you're ready. |
| **Full Mock Interviews** | 4-6 question simulations in behavioral, system design, case study, panel, and technical+behavioral formats. Includes the **interviewer's inner monologue**. |
| **Transcript Analysis** | Paste from Otter, Zoom, Grain, Meet, Teams — auto-detected format, per-question scoring, triage-based coaching path. |

### Tracking & Adaptation

| Feature | What You Get |
|---------|-------------|
| **Adaptive Mentoring** | Decision tree triages your bottleneck and branches to the right drill. Not the same path for everyone. |
| **Session Continuity** | Persistent `mentoring_state.md` tracks storybank, scores, patterns, drill progression, and interview loops across sessions. |
| **Self-Calibration** | Tracks the gap between your self-assessment and actual scores. Knows if you're an over-rater or under-rater. |
| **8-Language Support** | Full mentoring in English · 中文 · 日本語 · 한국어 · Español · Français · Filipino · Bahasa Indonesia |

---

## Commands

14 commands covering the full interview lifecycle:

| Category | Command | What It Does |
|----------|---------|-------------|
| **Setup** | `kickoff` | Initialize profile, pick track, get personalized action plan |
| **Resume** | `resume` | Audit, rewrite, add thinking depth, JD-target your resume |
| **Narrative** | `narrative` | Build career arc, transition bridges, themes, elevator pitches |
| **Prep** | `prep [company]` | Company research, predicted questions, story mapping, cheat sheet |
| **Practice** | `practice` | 8-stage drill progression with scoring and gating |
| **Mock** | `mock [format]` | Full simulated interview with inner monologue debrief |
| **Stories** | `stories` | Build STAR-T storybank with earned secrets |
| **Analyze** | `analyze` | Score interview transcripts with format-aware parsing |
| **Debrief** | `debrief` | Same-day post-interview rapid capture |
| **Feedback** | `feedback` | Log recruiter feedback, outcomes, corrections |
| **Progress** | `progress` | Trend review, self-calibration, coaching effectiveness |
| **Negotiate** | `negotiate` | Post-offer negotiation with exact scripts |
| **Hype** | `hype` | Pre-interview confidence boost, 3x3 sheet, recovery scripts |
| **Help** | `help` | Context-aware command guide with recommended next step |

<details>
<summary><strong>Multi-language command aliases</strong></summary>

| Alias | Command |
|-------|---------|
| `准备` / `準備` | `prep` |
| `简历` / `履歴書` | `resume` |
| `叙事` / `ストーリー` | `narrative` |
| `练习` / `練習` | `practice` |
| `模拟` / `模擬` | `mock` |
| `故事` | `stories` |
| `分析` | `analyze` |
| `复盘` / `復盤` | `debrief` |
| `反馈` / `フィードバック` | `feedback` |
| `进度` / `進度` | `progress` |
| `谈判` / `交渉` | `negotiate` |
| `加油` | `hype` |
| `帮助` / `ヘルプ` | `help` |

</details>

---

## How It Works

### The Scoring System

Every answer is evaluated on 5 dimensions (1-5 scale):

```
Substance      ████░  Evidence quality — specifics, numbers, alternatives considered
Structure      ███░░  Narrative clarity — setup → conflict → resolution → impact
Relevance      █████  Question fit — every sentence serves the answer
Credibility    ████░  Believability — proof points, realistic constraints
Differentiation ██░░░  Uniqueness — earned secrets, defensible POVs
```

Scores map to a **Hire Signal**: Strong Hire · Hire · Mixed · No Hire — calibrated to your seniority band (Early Career / Mid / Senior / Executive).

### The STAR-T Framework

Traditional STAR captures what you did. **STAR-T** captures how you think:

```
S — Situation    What was the environment and pressure?
T — Task         What was on YOUR plate?
A — Action       What did YOU do? (specific steps and decisions)
R — Result       Quantified outcome + ripple effects

T — Thinking     ← This is what sets you apart
    ├── Hard Part:     The real challenge (not the obvious one)
    ├── Alternatives:  What else you considered
    ├── Why This:      Your reasoning for the chosen path
    ├── Risk:          What could go wrong
    └── Lesson:        What you'd do differently now
```

### The 8-Stage Drill Progression

```
Stage 1  ▸ Ladder      Tell the same story at 30s, 60s, 90s, 3min
Stage 2  ▸ Pushback    Handle skepticism and "so what?" pressure
Stage 3  ▸ Pivot       Redirect when questions don't match your prep
Stage 4  ▸ Gap         Handle "I don't have an example" gracefully
Stage 5  ▸ Role        Face role-specific specialist scrutiny
Stage 6  ▸ Panel       Navigate multiple interviewer personas
Stage 7  ▸ Stress      Perform under maximum pressure
Stage 8  ▸ Technical   Think out loud, articulate tradeoffs
```

Each stage has a **gating threshold** — you advance when your scores prove readiness.

---

## Workflow Examples

**Getting started:**
```
> kickoff
```
Share your resume → get profile snapshot → receive time-aware action plan.

**Optimizing your resume:**
```
> resume audit          # Score every bullet for impact, thinking, and skill signal
> resume thinking       # Add decision-making depth to key bullets
> resume target Google  # Tailor for a specific JD
```

**Building your narrative:**
```
> narrative build       # Career arc: timeline → growth → thesis
> narrative bridge      # "Why did you leave X for Y?" bridges
> narrative thread      # Extract recurring career themes
> narrative pitch       # 15s / 30s / 60s / 90s elevator pitches
```

**Preparing for an interview:**
```
> prep Google           # Company research + predicted questions + cheat sheet
> practice              # Drill progression (8 stages)
> mock behavioral Google  # Full 4-6 question simulation
> hype                  # Pre-interview confidence boost
```

**After an interview:**
```
> debrief               # Same-day rapid capture
> analyze               # Paste transcript → per-question scoring
> feedback              # Log recruiter feedback or outcome
```

**When you get an offer:**
```
> negotiate             # Offer analysis + strategy + scripts
```

---

## Two Tracks

| | Quick Prep | Full System |
|---|---|---|
| **Best for** | Interview in < 2 weeks | Multi-week job search |
| **Focus** | Prep brief → focused practice → hype | Full lifecycle coaching |
| **Commands** | `prep` → `practice` → `hype` | All 14 commands |
| **Storybank** | Gap check only | Full build + retrieval drills |
| **Tracking** | Minimal | Scores, trends, calibration, outcomes |

Choose during `kickoff`. Switch anytime.

---

## Supported Languages

| | Language | Status |
|---|----------|--------|
| 🇺🇸 | English | Full support |
| 🇨🇳 | 中文（简体） | Full support |
| 🇯🇵 | 日本語 | Full support |
| 🇰🇷 | 한국어 | Full support |
| 🇪🇸 | Español | Full support |
| 🇫🇷 | Français | Full support |
| 🇵🇭 | Filipino | Full support |
| 🇮🇩 | Bahasa Indonesia | Full support |

The mentor auto-detects your language from your first message. Command names stay in English (or use aliases above), but all coaching output is in your language.

---

## Repository Structure

```
interview-mentor-skill/
├── SKILL.md                     # Core skill — rename to CLAUDE.md to activate
├── README.md                    # This file
├── LICENSE                      # MIT License
└── references/
    ├── commands/                # Per-command workflows (14 files)
    │   ├── kickoff.md           # Profile setup + action plan
    │   ├── resume.md            # Resume audit, rewrite, thinking depth
    │   ├── narrative.md         # Career arc, bridges, themes, pitches
    │   ├── prep.md              # Company + role prep brief
    │   ├── practice.md          # 8-stage drill system
    │   ├── mock.md              # Full mock interview simulations
    │   ├── stories.md           # STAR-T storybank management
    │   ├── analyze.md           # Transcript analysis + scoring
    │   ├── debrief.md           # Post-interview rapid capture
    │   ├── feedback.md          # External input capture
    │   ├── progress.md          # Trend review + calibration
    │   ├── negotiate.md         # Offer negotiation coaching
    │   ├── hype.md              # Pre-interview confidence
    │   └── help.md              # Context-aware command guide
    ├── cross-cutting.md         # Gap-handling, signal-reading, cultural awareness
    ├── rubrics-detailed.md      # 5-dimension scoring anchors + root causes
    ├── differentiation.md       # Earned secrets + spiky POVs
    ├── storybank-guide.md       # Story management + retrieval drills
    └── examples.md              # Worked examples with scoring
```

---

## Tips for Best Results

1. **Share a real resume** — not a summary. The more detail, the better the analysis.
2. **Include the full JD** for `prep` — and the interview format if you know it.
3. **Use real transcripts** for `analyze` — the system auto-detects format.
4. **Build your storybank early** with `stories` — aim for 8+ stories covering core competencies.
5. **Run `progress` weekly** — it tracks self-assessment accuracy, not just scores.
6. **Use `debrief` same day** — capture signals while they're fresh.
7. **Run `mock` before big interviews** — individual drills build skills; mocks test the full arc.
8. **Log every outcome** with `feedback` — the system learns from your real experiences.

---

## Contributing

We welcome contributions! Open an issue or PR with:

- Repro steps (what you did)
- Current behavior (what happened)
- Expected behavior (what should happen)
- Suggested fix (optional)

---

## Credits

Created by [Junhao Xue](https://github.com/JunhaoXue) & [Claude](https://claude.ai).

## License

[MIT](LICENSE) — use it, fork it, make it yours.
