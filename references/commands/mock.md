# mock — Full Simulated Interview

A complete simulated interview (4-6 questions) with holistic feedback on the full arc.

### Setup

1. Ask for format: behavioral, system-design, case-study, panel, technical-mix
2. Ask for company/role context (or use existing prep data)
3. **Calibrate difficulty** to candidate's progression stage
4. **Calibrate tone** to target company:
   - Large tech: structured, high bar on metrics, rubric-based
   - Startups: conversational, adaptability and scrappiness
   - Consulting/finance: case-study oriented, precision, polish
5. Set interviewer persona based on format

### Execution

1. Deliver questions one at a time. Wait for each response.
2. **Do NOT give feedback between questions** — simulate real interview.
3. Vary difficulty: start moderate, escalate, include one curveball.
4. Include at least one question targeting a known story gap.
5. Pull from saved concerns data if available.
6. **Adapt mid-mock like a real interviewer**:
   - Strong answer → go deeper with follow-up
   - Weak answer → move on or redirect subtly
   - Surprising/contradictory → follow up
7. Track: story diversity, energy trajectory, answer length, time management.

### Panel Simulation

Use named personas with distinct voices:

> **[Sarah — Skeptic]**: "I'm not sure that metric tells the full story. How did you isolate your team's impact?"
>
> **[James — Ally]**: "That's interesting. Can you walk us through the timeline?"
>
> **[Director Lin — Silent Observer]**: *[takes notes]*

### System Design / Case Study Simulation

**State coaching boundary**: "I'll evaluate your communication process — how you scope, structure, reason, and articulate tradeoffs. I won't evaluate technical correctness."

1. Present open-ended problem statement
2. Observe clarification phase silently
3. Probe tradeoffs: "Why this over X?", "What breaks at 10x scale?"
4. Test adaptability: "What if [constraint] changed?"

**Track**: Clarification behavior, approach structure, reasoning narration, tradeoff articulation, adaptability, time management, uncertainty handling.

### Technical + Behavioral Mix Simulation

1. Structure mock to match described format (default: alternating)
2. Include deliberate mode switches mid-question
3. Vary transitions (clean breaks vs seamless pivots)

**Track**: Mode-switching speed, register appropriateness, integration quality, energy trajectory, which mode is stronger.

### Post-Mock Self-Assessment

**Before showing any scores**, ask:
- "How do you think that went? Strong Hire, Hire, Mixed, or No Hire?"
- "Which answer was strongest? Weakest?"
- "Anything you'd do differently?"

### Redo Mechanism

Offer one redo for the weakest answer: "Your answer to Q[N] had the most room for improvement. Want to try that one again?"

### Post-Mock Debrief Schema

```markdown
## Mock Interview Debrief: [Format] — [Company/Role]

## Overall Impression
- Hire Signal: Strong Hire / Hire / Mixed / No Hire
- One-sentence summary:

## Arc Analysis
- Energy trajectory: Started [level] → Ended [level]
- Story diversity: __ unique stories across __ questions
- Pacing: [rushed / well-timed / dragged]

## Per-Question Scorecard

### Q1
- Scores: Sub __ / Str __ / Rel __ / Cred __ / Diff __
- Strongest moment:
- Missed opportunity:

[repeat for each question]

## Holistic Patterns
- Repeated crutch phrases:
- Topics avoided:
- Questions causing hesitation:
- Best moment of the interview:
- Worst moment and recovery quality:

## Signal Reading Notes
- Questions where follow-up indicated interest (+):
- Questions where interviewer moved on quickly (-):

## Interviewer's Inner Monologue
[Key moments from the interviewer's real-time perspective — what they were thinking and evaluating. Include both positive and negative reactions. Ground in candidate's actual words.]

## Format-Specific Notes (if applicable)
[System design: process visibility, clarification behavior, tradeoff articulation]
[Technical mix: mode-switching fluidity, integration quality, stronger mode]

## Top 3 Changes for Next Mock
1.
2.
3.

**Recommended next**: `[command]` — [reason]. **Alternatives**: `mock [format]`, `practice [drill]`, `analyze`
```

### Interviewer's Inner Monologue — How To Write It

- Ground every beat in candidate's actual words
- Include both positive and negative reactions
- Show pivot points where overall impression shifted
- Connect to signal-reading
- Calibrate tone to mock format (startup CEO ≠ FAANG bar raiser)

### Coaching State Integration

After mock:
1. Add scores to Score History (Type: mock, include Hire Signal)
2. Record self-assessment delta
3. Update Active Coaching Strategy if new patterns emerge
