# feedback — Capture External Input

### Input Types

| Type | Trigger | What to Capture |
|---|---|---|
| **Recruiter feedback** | "The recruiter said..." | Verbatim feedback, linked dimension, company |
| **Outcome** | "I got rejected / advanced / got an offer" | Update Outcome Log, trigger calibration check |
| **Correction** | "Actually, I think your score was wrong because..." | Evaluate, adjust if warranted |
| **Memory** | "I just remembered — they also asked..." | Route to Question Bank / Storybank / Interview Loops |
| **Meta-feedback** | "This coaching isn't working for me because..." | Record in Coaching Notes, adjust approach |

### Workflow

1. Classify input type
2. Route to appropriate section of mentoring_state.md
3. Cross-reference with existing data where useful
4. Suggest next action

### Outcome Processing

When candidate reports an outcome:
- Update Outcome Log (Result: advanced / rejected / pending / offer / withdrawn)
- Update Question Bank Outcome column for that company's questions
- If 3+ outcomes exist → trigger calibration check:
  - Compare practice/mock scores with real outcomes
  - Detect scoring drift (coach scoring too high or low vs reality)
  - Update Calibration State

### Rejection Processing

When rejected:
- "This is useful data. Let's extract what we can."
- Cross-reference with practice/mock scores for that company
- Identify dimension most likely responsible
- Update Active Coaching Strategy if pattern emerges
- At Level 5: structured leverage extraction (what can we learn and apply?)

### Output Schema

```markdown
## Feedback Captured

### Type: [recruiter / outcome / correction / memory / meta]
### Details: [what was captured]
### State Updated: [which sections of mentoring_state.md changed]

### Implications
- [what this means for coaching strategy]

**Recommended next**: `[command]` — [reason]. **Alternatives**: `[command]`, `[command]`
```
