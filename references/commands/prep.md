# prep — Company + Role Prep Brief

### Prerequisites
- Company name (required)
- Role/seniority (required)
- Job description (strongly recommended)
- Interviewer LinkedIn URLs (optional — for per-interviewer intelligence)

### Workflow

1. **Company Research** — Search for company information using web search. Apply Evidence Sourcing Standard (✓ Verified / ~ General Knowledge / ? Unknown).
2. **Format Discovery** — Ask: "Do you know the interview format? (behavioral, system design, case study, panel, technical+behavioral mix)". If unknown, infer from company/role norms.
3. **Role-Fit Assessment** — Evaluate across 5 dimensions (Requirement Coverage, Seniority Alignment, Domain Relevance, Competency Overlap, Trajectory Coherence). Produce verdict: Strong Fit / Investable Stretch / Long-Shot Stretch / Weak Fit.
4. **Competency Extraction** — From JD, extract top competencies with confidence labels.
5. **Story Mapping** — If storybank exists, map stories to predicted questions using 4-level fit scoring (Strong Fit / Workable / Stretch / Gap).
6. **Concern Anticipation** — Generate likely interviewer concerns + counter strategies.
7. **Question Prediction** — Generate 7-10 predicted questions based on JD, role, company culture.
8. **Interviewer Intelligence** — If LinkedIn URLs provided, research each interviewer for focus areas, rapport hooks, story recommendations.

### Technical Format Coaching Boundaries

For system design, case study, or technical+behavioral mix formats, state upfront:
"I'll coach how you communicate your thinking — structuring, reasoning, articulating tradeoffs. I won't evaluate the technical correctness of your solution. For that, practice with a domain peer."

### Output Schema

```markdown
## Prep Brief: [Company] — [Role]

### Interview Format
- Type: [behavioral / system design / case study / panel / technical-mix]
- Duration: [if known]
- Coaching boundaries: [if technical format]

### Company Snapshot
- Stage/size:
- Culture signals: [with evidence tags ✓/~/? ]
- What they optimize for:

### Role-Fit Assessment
- Verdict: [Strong Fit / Investable Stretch / Long-Shot Stretch / Weak Fit]
- Strengths:
- Gaps (frameable):
- Gaps (structural):

### Interviewer Intelligence (if available)
#### [Interviewer Name]
- Background:
- Likely focus areas:
- Rapport hooks:
- Story recommendations:

### Top Competencies
1. [competency] — Confidence: [High/Medium/Low]
2. [competency] — Confidence: [High/Medium/Low]
3. [competency] — Confidence: [High/Medium/Low]

### Predicted Questions (7-10)
1. [question] → Story: [S### or GAP]
2. ...

### Likely Concerns + Counters
| Concern | Counter Strategy |
|---------|-----------------|

### Your Best Positioning
- Lead with:
- Differentiate on:

### Questions To Ask Them
1.
2.
3.

### Day-Of Cheat Sheet
- 3 concerns + counters
- 3 questions to ask
- Opening positioning (30 seconds)
- Recovery script: "That wasn't my best answer. Let me give this next one full attention."

**Recommended next**: `practice` — [reason]. **Alternatives**: `mock [format]`, `hype`, `stories`
```

### Coaching State Integration

After prep:
- Add/update Interview Loops entry for this company
- Save round formats, fit verdict, concerns, predicted questions
- If storybank gaps found, flag for `stories`
