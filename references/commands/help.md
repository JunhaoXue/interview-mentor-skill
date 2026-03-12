# help — Context-Aware Command Guide

### Workflow

1. Read mentoring_state.md to understand current context
2. Show full command list with current relevance
3. Highlight the recommended next command based on coaching state

### Output Schema

```markdown
## Interview Mentor — Command Guide

### Getting Started
| Command | What It Does | Your Status |
|---|---|---|
| `kickoff` | Set up your profile and coaching plan | [✓ done / needed] |

### Interview Prep
| Command | What It Does | Your Status |
|---|---|---|
| `prep [company]` | Build a prep brief for a specific company | [companies prepped] |
| `hype` | Pre-interview confidence boost | [use before interviews] |

### Practice & Simulation
| Command | What It Does | Your Status |
|---|---|---|
| `practice` | Drill practice (8 stages) | Stage [N] |
| `mock [format]` | Full simulated interview | [mocks completed] |
| `stories` | Build and manage your storybank | [N] stories |

### Analysis & Tracking
| Command | What It Does | Your Status |
|---|---|---|
| `analyze` | Score an interview transcript | [transcripts analyzed] |
| `debrief` | Rapid capture after an interview | [use same day] |
| `feedback` | Log recruiter feedback or outcomes | [pending outcomes] |
| `progress` | Review trends and calibration | [sessions since last review] |

### Offer Stage
| Command | What It Does | Your Status |
|---|---|---|
| `negotiate` | Post-offer negotiation coaching | [when you have an offer] |

### Command Aliases
You can also use these shortcuts:
- 中文: 准备/练习/模拟/故事/分析/复盘/反馈/进度/谈判/加油/帮助
- 日本語: フィードバック/ヘルプ/交渉

---

**Right now, your highest-leverage move is**: `[command]` — [reason based on coaching state]
```

### Recommendation Logic

Check in this order:
1. Pending outcomes in Outcome Log → "Any news from [companies]?"
2. Interview within 48h → `hype`
3. Storybank empty → `stories`
4. Debrief captured but no analysis → `analyze`
5. Research done but no prep → `prep [company]`
6. 3+ sessions without progress review → `progress`
7. Active prep but no practice → `practice`
8. Otherwise → most relevant command based on Active Coaching Strategy
