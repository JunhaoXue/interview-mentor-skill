# debrief — Post-Interview Rapid Capture

Use same day after a real interview while details are fresh. Works with or without a transcript.

### Workflow

1. **Rapid capture** — Ask one at a time:
   - "What questions did they ask? List as many as you remember."
   - "For each question, what story did you tell? How do you think it landed?"
   - "Any moments where the interviewer seemed especially interested or disengaged?"
   - "Anything unexpected — questions you didn't prep for, format surprises?"
   - "Overall gut feeling: Strong Hire, Hire, Mixed, No Hire?"

2. **Signal reconstruction** — From the candidate's recall, identify:
   - Positive signals (follow-ups, note-taking, genuine curiosity)
   - Negative signals (quick pivots, redirections, clock-checking)
   - Ambiguous signals (silence, neutral responses)

3. **Story tracking** — Update storybank:
   - Mark stories as "Last Used: [date]" and increment Use Count
   - Flag stories that didn't land well for `stories improve`
   - Note new story candidates from unexpected questions

4. **Coaching state update** — Record in Interview Loops:
   - Round completed with date
   - Questions asked (to Interview Intelligence Question Bank, marked "recall-only")
   - Stories used per round
   - Interviewer signals observed

### Output Schema

```markdown
## Debrief: [Company] — [Round] — [Date]

### Questions Recalled
1. [question] → Story: [S### or improvised] → Landing: [strong / okay / weak]
2. ...

### Interviewer Signals
- Positive: [moments of interest]
- Negative: [moments of disengagement]
- Unexpected: [surprises]

### Self-Assessment
- Overall: [Strong Hire / Hire / Mixed / No Hire]
- Best moment:
- Weakest moment:

### Storybank Updates
- Used: [S### list with dates]
- Needs improvement: [S### that didn't land]
- New candidates: [experiences from unexpected questions]

### Next Steps
- Outcome expected by: [date if known]
- Follow-up needed: [yes/no]

**Recommended next**: `analyze` — paste transcript for detailed scoring. **Alternatives**: `feedback` (when you hear back), `prep [next company]`
```
