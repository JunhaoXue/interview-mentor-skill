# analyze — Transcript Analysis

### Input

Candidate pastes a raw interview transcript. The system handles:
- Auto-detection of format (Otter, Zoom, Grain, Google Meet, Teams, Tactiq, Granola, or generic)
- Normalization to a clean Q&A structure

### Workflow

1. **Format Detection**: Identify transcript source and normalize.
2. **Interview Type Classification**: behavioral, system design, panel, technical+behavioral mix, case study.
3. **Per-Unit Analysis**: Score each unit (Q&A pair for behavioral, phase for system design, exchange for panel).
4. **Self-Reflection**: Ask candidate to self-assess before showing scores.
5. **Triage Decision**: Based on patterns, branch to the right coaching path.
6. **Storybank Updates**: Identify stories used, flag new story candidates.

### Format-Specific Analysis

**Behavioral**: Parse Q&A pairs. Score each on 5 dimensions. Flag missed follow-up opportunities.

**System Design**: Parse into phases (scoping, approach, deep-dive, tradeoff, adaptation). Score communication quality, not technical correctness. Additional dimensions: Process Visibility, Scoping Quality.

**Panel**: Track cross-interviewer dynamics. Note which persona asked what, and how candidate adapted across different styles.

**Technical + Behavioral Mix**: Score each segment in its native mode. Assess mode-switching quality.

### Triage Decision Tree

After scoring, diagnose the primary bottleneck:

| Pattern | Diagnosis | Recommended Path |
|---------|-----------|-----------------|
| Substance < 3, others okay | Missing evidence/depth | `stories improve` + tension-mining |
| Structure < 3, others okay | Narrative disorganization | `practice ladder` (constraint drills) |
| Relevance < 3, others okay | Question misreading | Question-decoding drills |
| Credibility < 3, others okay | Believability gap | I/we audit + constraint practice |
| Differentiation < 3, others okay | Generic answers | Earned secret extraction |
| Multiple dims < 3 | Root cause likely | Check Root Cause Taxonomy |
| All dims ≥ 3, no 5s | Plateau | Differentiation push |
| Practice scores >> real scores | Performance anxiety | Psychological readiness |

### Output Schema

```markdown
## Transcript Analysis: [Company] — [Round]

### Format
- Detected: [source format]
- Interview type: [behavioral / system design / panel / mix]

### Per-Unit Scores

#### Q1 / P1 / E1: [question/phase summary]
- Sub: __ / Str: __ / Rel: __ / Cred: __ / Diff: __
- What worked:
- Gap:
- Interviewer was thinking: [1-2 sentences]

[repeat for each unit]

### Scorecard (averages)
- Substance: __
- Structure: __
- Relevance: __
- Credibility: __
- Differentiation: __
- **Hire Signal**: [Strong Hire / Hire / Mixed / No Hire]

### Self-Assessment Delta
- Candidate overall: __
- Mentor overall: __
- Calibration: [over / under / accurate]

### Triage Decision
- Primary bottleneck: [dimension]
- Root cause: [from taxonomy]
- Coaching path: [specific recommendation]

### What Is Working
1.
2.

### Top 3 Gaps To Close
1. [gap + specific fix]
2. [gap + specific fix]
3. [gap + specific fix]

### Storybank Changes
- Stories identified: [new candidates for storybank]
- Stories used: [S### IDs if storybank exists]

### Priority Move (Next 72 Hours)
[Single most impactful action]

**Recommended next**: `[command]` — [reason]. **Alternatives**: `practice [drill]`, `stories improve`, `mock [format]`
```

### Coaching State Integration

After analysis:
- Add scores to Score History (Type: interview)
- Update Active Coaching Strategy with triage decision
- Extract questions to Interview Intelligence Question Bank
- Update Effective/Ineffective Patterns if 3+ data points
- Check for cross-dimension root causes
