# stories — Storybank Management

### Sub-Commands

| Command | Purpose |
|---|---|
| `stories add` | Add a new story to the storybank |
| `stories improve [ID]` | Strengthen an existing story |
| `stories find gaps` | Identify competency gaps in storybank coverage |
| `stories list` | Show current storybank index |
| `stories retire [ID]` | Archive a story that's no longer useful |

### stories add — Workflow

1. Ask: "Tell me about a work experience you're proud of, or one that taught you something important."
2. Listen to the raw story.
3. Extract **STAR-T** structure (STAR + Thinking):
   - **Situation**: Context and stakes — what was the environment, what pressure existed?
   - **Task**: Your specific responsibility — what was on YOUR plate?
   - **Action**: What YOU did (not "we") — specific steps and decisions
   - **Result**: Quantified outcome + what changed + ripple effects
   - **Thinking**: The decision-making layer (NEW — critical for interview depth):
     - **The Hard Part**: What was the real challenge? (not the obvious one)
     - **Alternatives Considered**: What other approaches did you evaluate?
     - **Why This Approach**: What was your reasoning for the chosen path?
     - **What Could Go Wrong**: What risks did you weigh?
     - **Lesson Learned**: What would you do differently knowing what you know now?
4. Extract earned secret: "What do you know from this experience that most people in your role wouldn't know?"
5. Assign:
   - Primary Skill (the main competency this story demonstrates)
   - Secondary Skill (a bonus competency)
   - Thinking Depth rating (1-5): Can you clearly explain the WHY behind your decisions?
   - Strength rating (1-5, based on evidence quality and uniqueness)
   - Deploy for (one-line use case)
6. Write to storybank index + Story Details.

#### Thinking Depth Rating

| Score | Description |
|-------|-------------|
| 1 | "I did X" — no reasoning visible |
| 2 | "I chose X because it seemed right" — vague reasoning |
| 3 | "I chose X over Y because [reason]" — shows one alternative |
| 4 | "I evaluated X, Y, Z. Chose X because [specific tradeoff]. Risk was [R], mitigated by [M]" |
| 5 | Full decision chain: problem framing → hypothesis → options → tradeoff analysis → decision → validation → learning |

### stories improve — Workflow

1. Read the existing story from mentoring_state.md.
2. Identify weaknesses across ALL dimensions:
   - Missing quantification → push for numbers
   - Weak "I" vs "we" → clarify individual contribution
   - No earned secret → extract through reflection questions
   - Low differentiation → develop spiky POV
   - **Low thinking depth** → deep-dive extraction:
     - "What was the hardest part that's not obvious from the outside?"
     - "What alternatives did you seriously consider?"
     - "What would a senior interviewer challenge about your approach?"
     - "Walk me through the moment you decided on this direction — what data/intuition drove it?"
     - "What's the thing that almost went wrong?"
   - **No narrative connection** → link to career arc:
     - "How does this story connect to your broader career thesis?"
     - "What skill from a previous role made this possible?"
3. Coach improvements one at a time.
4. Update the story in mentoring_state.md.

### stories find gaps — Workflow

1. Map storybank against common competency questions for target role:
   - Leadership / influence
   - Conflict / disagreement
   - Failure / mistake
   - Ambiguity / prioritization
   - Technical challenge
   - Cross-functional collaboration
   - Customer/user focus
   - Innovation / creativity
2. For each gap, prescribe a gap-handling pattern:
   - Story exists, strength 3+ → No gap
   - Story exists, strength 2 → Adjacent Bridge
   - Story exists, strength 1 → Reframe to Strength / Growth Narrative
   - No story → Hypothetical with Self-Awareness
3. Recommend: "You have strong coverage for [X]. You need stories for [Y]. Want to add one now?"

### Earned Secret Extraction

Five reflection questions to extract earned secrets:

1. "What surprised you most about this experience?"
2. "What would you do differently now, and why?"
3. "What do you know from this that most people in your role don't know?"
4. "What's the counterintuitive thing about this situation?"
5. "If you were advising someone facing the same situation, what would you tell them that they wouldn't find in any book or course?"

### Rapid-Retrieval Drill (practice retrieval)

Requires 8+ stories. Protocol:

1. 10 rapid-fire questions, 10 seconds each
2. Candidate must name: Story ID + opening line
3. Score: speed, accuracy, coverage
4. Debrief: which competencies had no quick answer? Which caused hesitation?

### Narrative Identity

After 5+ stories, extract the 2-3 core themes across all stories. This becomes the candidate's narrative identity — the coherent thesis about who they are. Every answer should subtly reinforce this identity.

### Output Schema (stories add)

```markdown
## New Story: S[###] — [Title]

### STAR-T
- **Situation**: [context + stakes]
- **Task**: [your responsibility]
- **Action**: [what YOU did]
- **Result**: [quantified outcome]
- **Thinking**:
  - Hard Part: [the real challenge]
  - Alternatives: [what else you considered]
  - Why This: [your reasoning]
  - Risk: [what could go wrong]
  - Lesson: [what you'd do differently]

### Metadata
- Primary Skill: [competency]
- Secondary Skill: [competency]
- Earned Secret: [insight]
- Thinking Depth: [1-5]
- Strength: [1-5]
- Deploy for: [one-line use case]
- Narrative Thread: [which career theme this supports]

### Improvement Opportunities
- [what would make this story stronger]

### Interview Hooks
- If asked "tell me more": [which part to expand — usually the Thinking layer]
- If challenged "why not [alternative]?": [defense with evidence]

**Recommended next**: `stories add` — [if gaps exist]. **Alternatives**: `practice ladder`, `stories find gaps`
```

### Coaching State Integration

After stories changes:
- Update storybank index + Story Details in mentoring_state.md
- If narrative identity updated, note in Coaching Notes
