# Worked Examples

Calibrated examples showing scoring in action.

---

## Example 1: Behavioral Answer — Mid-Career PM

**Question**: "Tell me about a time you had to make a difficult prioritization decision."

### Weak Answer (Substance: 2, Structure: 2, Relevance: 3, Credibility: 2, Differentiation: 1)

"So we had a lot of features to build and not enough engineers. I used the RICE framework to prioritize. We ended up shipping the most impactful features first and it worked out well. The team was happy with the process."

**Why these scores:**
- Substance 2: No specifics — which features? What was the constraint? How many engineers?
- Structure 2: No narrative arc — just a flat summary
- Relevance 3: Addresses the question but lacks depth
- Credibility 2: "It worked out well" — how? No metrics
- Differentiation 1: RICE framework mention is textbook. Any PM could say this

### Strong Answer (Substance: 4, Structure: 5, Relevance: 5, Credibility: 4, Differentiation: 4)

"In Q3 last year, my team had 4 engineers and 12 feature requests from 3 different stakeholders — sales, customer success, and our CEO. The CEO wanted a dashboard for board reporting. Sales wanted API integrations that 3 enterprise prospects had requested. CS wanted bug fixes that were driving churn.

I spent a day mapping each request to revenue impact. The API integrations mapped to $2.1M in pipeline. The bug fixes mapped to $400K in at-risk renewals. The CEO dashboard mapped to... nothing measurable.

I went to the CEO and said: 'I'd like to defer the dashboard by 6 weeks. Here's why.' I showed the revenue math. He pushed back — the board meeting was in 8 weeks. I proposed a compromise: a lightweight version using existing Metabase charts, shipped in 3 days instead of 6 weeks of custom work.

We shipped API integrations first. Two of the three prospects converted — $1.4M closed. The Metabase dashboard worked fine for the board meeting. The lesson I took away: the most political feature is rarely the most valuable one, and the best way to say no to your CEO is to show them the math, not argue the principle."

**Why these scores:**
- Substance 4: Specific numbers ($2.1M pipeline, $1.4M closed, 4 engineers, 12 requests). Missing: what happened with the bug fixes?
- Structure 5: Clean arc — setup (constraint), conflict (CEO pushback), resolution (compromise), impact (results + lesson)
- Relevance 5: Every sentence serves the prioritization question
- Credibility 4: Real numbers, realistic constraints, CEO interaction rings true. Would be 5 with third-party validation
- Differentiation 4: "The most political feature is rarely the most valuable one" — this is an earned secret. Specific to this person's experience

---

## Example 2: System Design Communication — Senior Engineer

**Question**: "Design a notification system for a social media platform."

### Weak Communication (Process Visibility: 2, Structure: 2)

"Okay so I'd use a message queue, probably Kafka, and then have workers that process notifications and send them via push, email, and SMS. We'd need a database to store notification preferences. I'd use Redis for rate limiting."

**Why weak:**
- Jumped straight to solution without scoping
- No structure — just listed technologies
- No tradeoff discussion
- Interviewer can't follow the reasoning

### Strong Communication (Process Visibility: 5, Structure: 4)

"Before I dive in, let me scope this. When you say notification system — are we talking about in-app notifications, push, email, SMS, or all of the above? And what scale are we designing for — millions of users, or billions?

[After scoping] Great. I'll structure my approach in three parts: first the high-level architecture, then the delivery pipeline, then I'll address scale and failure modes.

For the high-level architecture, I see three main components: an event ingestion layer, a preference/routing engine, and delivery channels. Let me draw this out...

The key tradeoff I want to call out early: we could do synchronous delivery for simplicity, but at this scale that's a non-starter. So I'm going with an async pipeline using a message queue. The tradeoff is latency — notifications won't be instant, but we gain reliability and the ability to handle traffic spikes without dropping messages.

One thing I'm not sure about is whether we need exactly-once delivery semantics. That's significantly harder to implement. My instinct is at-least-once with client-side deduplication is good enough for most notification types — but I'd want to validate that with the product team for things like payment notifications where duplicates would be confusing."

**Why strong:**
- Scoped before solving
- Outlined structure upfront
- Named tradeoffs explicitly
- Acknowledged uncertainty honestly

---

## Example 3: Triage Decision

**Candidate scores across 3 sessions:**

| Session | Sub | Str | Rel | Cred | Diff |
|---------|-----|-----|-----|------|------|
| Mock 1 | 3.2 | 2.5 | 3.8 | 3.0 | 2.0 |
| Practice | 3.5 | 2.8 | 3.5 | 3.2 | 2.2 |
| Mock 2 | 3.0 | 2.3 | 4.0 | 2.8 | 2.5 |

**Triage analysis:**
- Structure consistently lowest (2.3-2.8) → primary bottleneck
- Differentiation consistently low (2.0-2.5) → secondary bottleneck
- Relevance strong (3.5-4.0) → not an issue
- Pattern: candidate knows WHAT to say but not HOW to structure it

**Root cause**: Likely narrative hoarding — answers run long, structure collapses under detail weight. Evidence: Structure drops from practice (2.8) to mock (2.3), suggesting anxiety amplifies the hoarding.

**Prescribed path**:
1. `practice ladder` — constraint drills force structure by limiting time
2. After Structure ≥ 3: `stories improve` — extract earned secrets to boost Differentiation
3. Parallel: address performance anxiety component via Psychological Readiness

---

## Example 4: Self-Assessment Delta

**Mock result:**
- Candidate self-assessed: "I think that was a Hire. Maybe a Strong Hire on Q2."
- Mentor scored: Mixed (3 questions at 3, 1 at 2, 1 at 4)

**Delta**: Over-rater. Candidate rated themselves ~0.8 points higher on average.

**Coaching response:**
"You rated yourself higher than I did on 4 out of 5 questions. That's not unusual — most people are over-raters early on. The risk is that you'll feel confident going into interviews when there's still real work to do. Let's look at where the gap is widest — Q3, where you gave yourself a 4 on Structure and I scored it a 2. Here's what I noticed..."

---

## Example 5: Earned Secret Extraction

**Raw story**: "I led the migration from monolith to microservices. It took 18 months and we had zero downtime."

**Extraction dialogue:**

Mentor: "What surprised you most about this migration?"

Candidate: "Honestly, the technical part was straightforward. What nearly killed us was the team dynamics. Every time we split a service, we had to decide which team owned it, and that meant org chart changes. Half the resistance to the migration was really resistance to reorgs."

Mentor: "That's your earned secret. Most people think microservice migrations are technical challenges. You know they're organizational ones. Let's build the story around that."

**Earned secret**: "The hardest part of a microservice migration isn't the code — it's the org chart. Every service boundary is a team boundary, and every team boundary is a political negotiation."

**Differentiation impact**: Jumps from 2 (generic "led a migration") to 4 (specific organizational insight that reframes the problem).
