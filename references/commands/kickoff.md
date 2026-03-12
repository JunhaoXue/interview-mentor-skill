# kickoff — Setup Workflow

### Step 1: Coaching Configuration

Collect (one question at a time):

1. Track choice: `Quick Prep` or `Full System`
2. Target role(s)
3. Feedback directness (1-5, default 3)
4. Interview timeline
5. Biggest concern
6. **Interview history**: "Have you been interviewing already? How many interviews have you done for this type of role, and how have they gone?"
   - **First-time interviewer**: Needs fundamentals — storybank building, basic structure, confidence. Start with practice ladder.
   - **Active but not advancing**: Needs diagnosis. "Where are you getting stuck — first rounds, final rounds, or not hearing back?" First-round failures → Relevance/Structure. Final-round failures → Differentiation/Credibility.
   - **Experienced but rusty**: Needs refreshing, not rebuilding. Focus on updating stories and sharpening differentiation.

### Step 2: Candidate Context

Required:
- Resume text or upload summary

Strongly recommended:
- 2-3 target companies
- 3-5 initial stories

### Step 2.5: Resume Analysis

Analyze for coaching-relevant signals:

1. **Positioning strengths**: The 2-3 signals a hiring manager sees in 30 seconds
2. **Likely concerns**: Career gaps, short tenures, domain switches, seniority mismatches, missing keywords
3. **Career narrative gaps**: Transitions that need a story ready
4. **Story seeds**: Resume bullets with likely rich stories behind them

### Step 2.6: Career Transition Detection

Check whether target role represents a career transition:
- Function change (engineering → product)
- Domain shift (B2C → B2B)
- IC ↔ management switch
- Industry pivot
- Career restart

When detected, flag downstream impacts: stories need bridge narratives, concerns shift, positioning needs reframing.

### Step 2.7: Target Reality Check

Fire only when clear mismatches are visible:
- Seniority gap of 2+ levels
- Zero domain experience for domain-specific role
- Function switch without obvious bridge
- Missing hard skill requirements

When triggered, surface directly without gatekeeping: "I want to flag [gap]. This doesn't mean you shouldn't go for it — but we should build a strategy for addressing it."

### Step 3: Initialize Mentoring State

Write `mentoring_state.md` with:
- Profile populated from Steps 1-2
- Resume Analysis from Step 2.5
- Empty storybank (or populated if initial stories provided)
- Empty score history, outcome log, drill progression at Stage 1
- Empty Interview Intelligence section
- Session log with kickoff entry
- Coaching Notes with observations from kickoff

### Time-Aware Coaching

- **≤48 hours**: Triage mode. Skip storybank building. `prep` → `hype` → done.
- **1-2 weeks**: Focused mode. `prep` + one targeted `practice` drill.
- **3+ weeks**: Full system. Build storybank, run progression drills, develop differentiation.

### Output Schema

```markdown
## Kickoff Summary
- Track:
- Target Role(s):
- Seniority band:
- Timeline:
- Interview history:
- Feedback Directness:
- Time-aware mode: [triage / focused / full]

## Profile Snapshot
- Positioning strengths:
- Likely interviewer concerns:
- Career narrative gaps:
- Story seeds:

## Interview Readiness Assessment
- Current readiness:
- Biggest risk going in:
- Biggest asset going in:

## Target Reality Check (only if flagged)
- Gap identified:
- Recommendation:

## First Plan
### Immediate (this session)
1. [action + command]

### This week
2. [action + command]
3. [action + command]

### Before first interview
4. [action + command]

**Recommended next**: `[command]` — [reason]. **Alternatives**: `stories`, `practice ladder`, `help`
```
