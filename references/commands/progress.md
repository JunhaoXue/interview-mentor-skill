# progress — Trend Review & Self-Calibration

### Minimum Data Thresholds

| Data Available | What You Can Show |
|---|---|
| 1 session | Basic: last session summary, current drill stage |
| 2-3 sessions | Emerging: direction per dimension, early patterns |
| 4+ sessions | Full: trends, self-calibration accuracy, coaching effectiveness |
| 3+ real outcomes | Calibration: practice-to-outcome correlation, scoring drift |

### Workflow

1. **Score Trends** — Chart direction per dimension over time (improving / stagnant / declining)
2. **Self-Calibration** — Compare candidate's self-assessments vs mentor scores. Pattern: over-rater, under-rater, or well-calibrated.
3. **Coaching Effectiveness** — Is the current strategy working? Check Active Coaching Strategy + recent scores.
4. **Outcome Correlation** — If 3+ real outcomes: do practice scores predict real results?
5. **Scoring Calibration** — Detect drift between mentor scores and real-world outcomes.
6. **Archival Check** — If Score History > 15 rows, run archival. If Interview Intelligence exceeds thresholds, archive.

### Meta-Check Integration

If session count (from Session Log) is a multiple of 3, include a meta-check:
"Is this feedback landing? Are we working on the right things? What's not clicking?"

Record response in Coaching Notes.

### Output Schema

```markdown
## Progress Review — [Date]

### Score Trends
| Dimension | Baseline | Current | Direction |
|-----------|----------|---------|-----------|
| Substance | __ | __ | [↑/→/↓] |
| Structure | __ | __ | [↑/→/↓] |
| Relevance | __ | __ | [↑/→/↓] |
| Credibility | __ | __ | [↑/→/↓] |
| Differentiation | __ | __ | [↑/→/↓] |

### Self-Calibration
- Tendency: [over-rater / under-rater / well-calibrated]
- Average delta: [number]
- Pattern: [description]

### Drill Progression
- Current stage: [N]
- Gates passed: [list]
- Next gate: [what's needed]

### Coaching Strategy Assessment
- Current approach: [what we're doing]
- Working? [yes — evidence / no — evidence / unclear]
- Recommendation: [continue / adjust / pivot]

### Outcome Correlation (if 3+ outcomes)
- Practice score range for advances: [range]
- Practice score range for rejections: [range]
- Scoring drift: [none / coach scoring high / coach scoring low]

### Key Insight
[The single most important thing to know about this candidate's trajectory]

### What's Changed Since Last Review
[Specific improvements and remaining gaps]

**Recommended next**: `[command]` — [reason]. **Alternatives**: `practice [drill]`, `mock [format]`, `stories improve`
```
