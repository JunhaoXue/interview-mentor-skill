# narrative — Work Experience Narrative Framework

Most candidates prepare individual stories. Great candidates prepare a **narrative arc** — a coherent story of their career that makes every job, every transition, and every achievement reinforce a single thesis about who they are.

This command helps you build that arc.

---

### Why Narrative Matters

Interviewers don't just evaluate individual answers — they form an overall impression:
- "What kind of professional is this person?"
- "Where are they going?"
- "Does their trajectory make sense?"

If your answers are disconnected bullet points, the interviewer has to assemble the picture themselves — and they usually won't. A narrative does the assembly for them.

---

### Sub-Commands

| Command | Purpose |
|---|---|
| `narrative build` | Build your career narrative arc from scratch |
| `narrative bridge` | Create transition bridges between roles |
| `narrative thread` | Extract recurring themes across your career |
| `narrative pitch` | Generate narrative-based elevator pitches at multiple lengths |

---

### narrative build — Career Arc Construction

#### The Three-Layer Framework

**Layer 1: Timeline** — What happened, in order
> Job A → Job B → Job C → Target Role

**Layer 2: Growth Arc** — How you evolved
> "Started as [X], discovered [insight], grew into [Y], now ready for [Z]"

**Layer 3: Thesis** — The one thing that ties it all together
> "I'm the person who [core identity] — every role has been a different expression of that"

#### Workflow

1. **Map the timeline** — List every role chronologically:
   - Title, company, duration
   - One-line of what you actually did (not job description, YOUR contribution)

2. **Find the growth moments** — For each transition, ask:
   - "What did you learn in Role A that made you ready for Role B?"
   - "What couldn't you do at the start of this role that you could do by the end?"
   - "Why did you leave?" (the real reason, not the polished version)

3. **Extract the thesis** — Look across all roles:
   - What keeps showing up? (patterns, interests, strengths)
   - What gets you energized? (the work you'd do for free)
   - If someone watched your entire career like a movie, what would the plot be?

4. **Stress-test the arc**:
   - Does the target role feel like a natural next chapter?
   - Can you explain every transition in one sentence?
   - Would a stranger hearing your arc say "that makes sense"?

#### Common Arc Patterns

| Pattern | Example | Best For |
|---------|---------|----------|
| **Builder** | "I've always built things — first code, then teams, then products" | IC → Management |
| **Deep Diver** | "I go deep into one problem until I've mastered it, then find the next challenge" | Specialist roles |
| **Bridge Builder** | "I've always been the person connecting technical and business worlds" | PM, TPM, Solution roles |
| **Fixer** | "I keep ending up in broken situations and making them work" | Turnaround, ops, leadership |
| **Multiplier** | "I've gone from doing the work to teaching others to making the system that teaches" | Senior/Staff+ |
| **Explorer** | "Each role taught me a new domain, and now I combine all of them" | Career transitioners |

#### Output Schema

```markdown
## Career Narrative Arc

### Timeline
| # | Role | Company | Duration | Your One-Line |
|---|------|---------|----------|---------------|
| 1 | [title] | [co] | [years] | [what you actually did] |

### Growth Arc
- **Chapter 1** ([Role A]): [what you learned, what you became capable of]
- **Transition 1→2**: [why you moved, what insight drove it]
- **Chapter 2** ([Role B]): [new capability, bigger scope]
- **Transition 2→3**: [why you moved]
- **Chapter 3** ([Role C]): [current state, readiness for next]
- **Next Chapter** ([Target]): [why this is the natural next step]

### Career Thesis
"[One sentence that ties your entire career together]"

### Arc Pattern
- Type: [Builder / Deep Diver / Bridge Builder / Fixer / Multiplier / Explorer / Custom]
- Evidence: [3 specific moments that prove the pattern]

### Stress Test
- Target role feels natural? [yes / stretch — needs bridge / disconnect — needs reframing]
- Weakest transition: [which one, and how to explain it]
- Strongest chapter: [which one, and why it's your anchor]

**Recommended next**: `narrative bridge` — strengthen transitions. **Alternatives**: `narrative thread`, `stories`, `resume`
```

---

### narrative bridge — Transition Bridges

Every career transition is a potential interview question: "Why did you leave X for Y?"

Bad bridges: "I was looking for new challenges" (meaningless)
Good bridges: "At [Company A] I solved [problem], which made me realize [insight]. [Company B] was the only place where I could apply that at [bigger scale]."

#### The Bridge Formula

```
[What I achieved at A] + [Insight that emerged] + [Why B was the right next step] = Bridge
```

#### Workflow

For each transition:
1. "What were you proud of when you left?"
2. "What did that experience teach you that you couldn't learn by staying?"
3. "Why THIS next role? What specifically pulled you?"
4. "What would you have missed if you'd stayed?"

#### Red Flag Transitions (need extra work)

| Red Flag | What Interviewers Think | Bridge Strategy |
|----------|------------------------|-----------------|
| Short tenure (< 1 year) | "Flight risk / got fired" | Lead with what you accomplished, then the insight that emerged |
| Lateral move | "Not growing" | Frame as intentional breadth — "I needed [new skill] for where I'm going" |
| Title downgrade | "Couldn't hack it" | Frame as strategic — "I traded title for [scope / learning / domain]" |
| Gap | "What happened?" | Own it directly — sabbatical, health, family, learning. No vague answers |
| Industry switch | "Starting over?" | Connect the domains — "The problem I solve is the same, the context changed" |

#### Output Schema

```markdown
## Transition Bridges

### Transition: [Role A] → [Role B]
- **Achievement at A**: [what you proved]
- **Insight**: [what you realized]
- **Pull to B**: [why B specifically]
- **One-sentence bridge**: "[polished version]"
- **Red flags to address**: [if any]
- **If challenged further**: "[backup elaboration]"

[repeat for each transition]

### Narrative Flow Test
Reading all bridges in sequence: does the career story flow? [yes / needs work at transition #N]

**Recommended next**: `narrative thread` — extract themes. **Alternatives**: `resume`, `prep [company]`
```

---

### narrative thread — Recurring Themes

Extract 2-3 threads that run through your entire career. These become your interview DNA — the themes every answer subtly reinforces.

#### Workflow

1. Lay out all storybank stories + resume bullets
2. Tag each with underlying themes (not skills — deeper than that):
   - "Making order from chaos"
   - "Translating between worlds"
   - "Finding the simple solution to complex problems"
   - "Growing people while shipping product"
3. Rank by frequency and authenticity
4. Select top 2-3 as your narrative threads

#### Thread vs Skill

| Skill (surface) | Thread (deep) |
|-----------------|---------------|
| "Project management" | "I bring structure to ambiguity" |
| "Data analysis" | "I find the truth that changes decisions" |
| "People leadership" | "I build teams that outlast me" |
| "System design" | "I think in systems, not features" |

#### Output Schema

```markdown
## Narrative Threads

### Thread 1: "[theme]"
- Evidence across career:
  - [Role A]: [specific example]
  - [Role B]: [specific example]
  - [Role C]: [specific example]
- How it shows up in interviews: [which questions to weave this into]

### Thread 2: "[theme]"
- Evidence: [same structure]

### Thread 3: "[theme]" (optional)
- Evidence: [same structure]

### Integration Guide
- **"Tell me about yourself"**: Lead with Thread 1, weave in Thread 2
- **Behavioral questions**: Always connect your answer back to a thread
- **"Why this role?"**: Show how the role is the next expression of your threads
- **"Where do you see yourself in 5 years?"**: Project threads forward

**Recommended next**: `narrative pitch` — create pitch versions. **Alternatives**: `stories`, `prep [company]`
```

---

### narrative pitch — Elevator Pitches

Generate narrative-based pitches at multiple lengths, all anchored to your career arc and threads.

#### Output Schema

```markdown
## Narrative Pitches

### 15-Second (Networking)
"[hook + thesis]"

### 30-Second (Recruiter Screen)
"[hook + arc summary + why this role]"

### 60-Second (Interview "Tell Me About Yourself")
"[hook + chapter highlights + threads + why this role + what I bring]"

### 90-Second (Deep TMAY)
"[full arc with transitions + earned secrets + thesis + forward-looking]"

### Practice Notes
- The hook should make them want to hear more
- Every version contains the career thesis
- The 60s version is your default — practice until it's natural
- Adapt the ending based on which company/role you're pitching to

**Recommended next**: `practice ladder` — practice pitches at different lengths. **Alternatives**: `prep [company]`, `mock behavioral`
```

---

### Coaching State Integration

After narrative work:
- Save to mentoring_state.md:
  - Career Narrative section (arc, thesis, threads, bridges)
  - Update Resume Analysis with narrative insights
  - Link narrative threads to storybank stories
- Flag stories that need work to support the narrative
- Update Active Coaching Strategy if narrative reveals new bottleneck
