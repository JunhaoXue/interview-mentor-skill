# resume — Resume Optimization

Transform your resume from a task list into a proof-of-impact document. Three core principles:
1. **Prove you can deliver** — every bullet shows a skill AND a measurable result
2. **Show how you think** — embed decision-making and problem-solving into bullet points
3. **Tell a coherent story** — resume is a narrative, not a list of disconnected jobs

### Sub-Commands

| Command | Purpose |
|---|---|
| `resume audit` | Full resume review with scoring and priority fixes |
| `resume rewrite` | Rewrite bullets with impact-first framing |
| `resume target [company]` | Tailor resume for a specific JD |
| `resume thinking` | Add decision-making depth to key bullets |

---

### resume audit — Full Review

#### Workflow

1. **First Pass — Impact Scan** (30 seconds as a hiring manager)
   - Can I tell in 30 seconds what this person is good at?
   - Are there numbers? Are they meaningful?
   - Does this person sound like they delivered, or just participated?

2. **Bullet-by-Bullet Scoring** — Score each bullet on 3 dimensions:

   | Dimension | Score 1 | Score 3 | Score 5 |
   |-----------|---------|---------|---------|
   | **Delivery Proof** | "Managed a project" (no outcome) | "Led migration project, completed on time" (outcome but vague) | "Led monolith→microservices migration serving 2M users, reducing deploy time from 4h to 15min, zero downtime" (specific, quantified, scoped) |
   | **Thinking Visibility** | Just states what happened | Hints at a choice | Shows the problem → approach → why this approach → result chain |
   | **Skill Signal** | Generic responsibility | Clear skill but common framing | Unmistakable expertise — reader knows exactly what you're great at |

3. **Pattern Detection**
   - **"Responsible for" syndrome**: Bullets describe responsibilities, not achievements
   - **Number desert**: No quantification anywhere
   - **Context collapse**: Results without scope ("+50%" means nothing without baseline)
   - **Thinking gap**: No bullets show HOW you approached problems
   - **Narrative disconnect**: Jobs don't build on each other — reads like 3 different people

4. **Priority Fix List** — Rank fixes by impact:
   - P0: Missing numbers on strongest achievements (quick win, huge impact)
   - P1: "Responsible for" bullets → rewrite as achievements
   - P2: Add thinking depth to 2-3 key bullets
   - P3: Improve narrative flow between roles

#### Output Schema

```markdown
## Resume Audit

### 30-Second Hiring Manager Read
- First impression:
- Clearest strength:
- Biggest concern:
- Would I keep reading? [yes / maybe / no]

### Bullet Scoring
| # | Current Bullet | Delivery | Thinking | Skill Signal | Priority |
|---|---------------|----------|----------|-------------|----------|
| 1 | "..." | [1-5] | [1-5] | [1-5] | [P0-P3] |

### Patterns Detected
- [pattern name]: [evidence]

### Priority Fixes
1. **P0**: [specific fix + which bullet]
2. **P1**: [specific fix + which bullet]
3. **P2**: [specific fix + which bullet]

### Overall Assessment
- Delivery proof: [strong / moderate / weak]
- Thinking visibility: [strong / moderate / weak]
- Skill signal: [strong / moderate / weak]
- Narrative coherence: [strong / moderate / weak]

**Recommended next**: `resume rewrite` — start with P0 fixes. **Alternatives**: `resume thinking`, `stories`
```

---

### resume rewrite — Impact-First Bullets

#### The Rewrite Formula

Every bullet follows this structure:

```
[Action Verb] + [What You Did] + [How/Why (thinking)] + [Measurable Result] + [Scope/Context]
```

**Before**: "Responsible for the company's data pipeline"

**After**: "Redesigned data pipeline architecture (chose Kafka over RabbitMQ for 10x throughput headroom), reducing data latency from 45min to <2min for 3 downstream teams serving 500K daily users"

#### Rewrite Protocol

For each bullet:
1. **Extract the achievement**: What actually changed because of you?
2. **Find the number**: Revenue? Time saved? Users impacted? Error reduction? If no exact number, ask: "Can you approximate?"
3. **Surface the thinking**: Why did you choose this approach? What was the alternative?
4. **Add scope**: How big was this? How many users/dollars/systems?
5. **Verify the "I" test**: Is it clear this was YOUR contribution, not the team's?

#### Verb Upgrade Guide

| Weak | Strong | Why |
|------|--------|-----|
| Responsible for | Designed, Built, Led | Shows agency |
| Helped with | Drove, Spearheaded, Architected | Shows ownership |
| Worked on | Shipped, Delivered, Launched | Shows completion |
| Participated in | Initiated, Proposed, Championed | Shows initiative |
| Managed | Grew, Scaled, Transformed | Shows impact direction |

#### Output Schema

```markdown
## Resume Rewrite

### Bullet Rewrites (priority order)

#### Bullet #[N] — [Job Title @ Company]
- **Before**: "[original]"
- **After**: "[rewritten]"
- **What changed**: [delivery proof added / thinking visible / scope added]
- **Number sourced from**: [candidate provided / approximated / needs verification]

[repeat for each bullet]

### New Bullets to Add
- [achievement not currently on resume but should be, based on storybank or conversation]

### Bullets to Remove
- [bullet that adds no value or dilutes the narrative]

**Recommended next**: `resume thinking` — add decision depth. **Alternatives**: `resume target [company]`, `narrative`
```

---

### resume thinking — Decision-Making Depth

The goal: a hiring manager reads your resume and thinks "this person THINKS, not just executes."

#### The Thinking Layer

For 2-3 key bullets (your most impressive achievements), add a thinking layer:

**Level 1 — What you did** (most resumes stop here):
> "Built a recommendation engine"

**Level 2 — What you chose and why** (good resumes):
> "Built a collaborative filtering recommendation engine (chose over content-based approach after A/B testing showed 23% higher engagement)"

**Level 3 — The hard part and how you thought through it** (great resumes):
> "Built recommendation engine under cold-start constraints — designed hybrid approach combining collaborative filtering for returning users with popularity-based fallback for new users, solving the chicken-and-egg problem that blocked the previous 2 attempts"

#### Extraction Questions

For each key bullet, ask:
1. "What was the hardest part of this?" → This reveals the real challenge
2. "What alternatives did you consider?" → Shows decision-making breadth
3. "Why did you choose THIS approach?" → Shows judgment
4. "What did you try that didn't work first?" → Shows learning and persistence
5. "What would break if you'd made the wrong choice?" → Shows stakes awareness

#### Output Schema

```markdown
## Thinking-Enhanced Bullets

#### Bullet #[N]
- **Current**: "[bullet]"
- **Hard part identified**: [the real challenge]
- **Decision point**: [what you chose and what you rejected]
- **Enhanced**: "[rewritten with thinking visible]"

### Interview Bridge
For each enhanced bullet, prepare:
- **If interviewer asks "tell me more"**: [30-second expansion hitting the thinking process]
- **If interviewer asks "why that approach?"**: [defense of the decision with alternatives considered]
```

---

### resume target — JD-Targeted Optimization

#### Workflow

1. Parse JD for top competencies (with confidence labels)
2. Map resume bullets to JD requirements
3. Identify coverage gaps
4. Reorder/rewrite bullets to front-load JD-relevant achievements
5. Add keywords naturally (not keyword stuffing)

#### Output Schema

```markdown
## Targeted Resume: [Company] — [Role]

### JD Competency Map
| JD Requirement | Your Coverage | Resume Bullet # | Strength |
|---------------|--------------|-----------------|----------|
| [requirement] | [covered / partial / gap] | [#] | [1-5] |

### Recommended Changes
1. [reorder / rewrite / add specific bullet]
2. ...

### Keywords to Add
- [keyword] → natural placement: [which bullet]

### ATS Compatibility
- Format: [clean / needs fixes]
- Keyword density: [good / low — add these]
```

---

### Coaching State Integration

After resume work:
- Save Resume Optimization section to mentoring_state.md:
  - Date, depth, overall assessment
  - Delivery proof score, thinking visibility score, skill signal score
  - Narrative coherence score
  - Top fixes pending
  - JD-targeted status (if applicable)
- Update Story Seeds in Resume Analysis if new stories discovered
- Flag storybank gaps from resume bullets that need stories behind them
