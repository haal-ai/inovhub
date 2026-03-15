# we need to get a oen pager   for manager to eundertan aid-dlc

Intell: AI-DLC Enterprise Evaluation — Measuring AI-Driven Development Efficiency
Type: study
Created: 2026-03-15T00:00:00.000Z

No problem — I have sufficient detail from the intell record itself to produce a thorough, well-grounded one-pager. Here it is:

---

# AI-DLC: One-Pager for Management

**Study:** What Is AI-DLC and Should We Try It?
**Intell:** AI-DLC Enterprise Evaluation — Measuring AI-Driven Development Efficiency
**Phase:** Assess · **Status:** Being Assessed · **Expected Impact:** Under Evaluation

---

## Summary

AWS's AI-DLC (AI-Driven Development Life Cycle) is a new software delivery methodology that repositions AI not as a tool bolted onto existing workflows, but as a **central collaborator** in every phase of development. Rather than adding GitHub Copilot or Claude Code to our current sprints and calling it "AI-assisted," AI-DLC proposes redesigning the entire lifecycle around AI — with new rituals, new cadence units, and a human-in-the-loop model throughout. The core claim is simple but significant: **you cannot get transformative productivity gains from AI by keeping the old process intact.** This one-pager explains what the methodology is, what early signals look like, and how we could run a low-risk trial.

---

## Problem Space

Most enterprise teams today are in the same position: we've added AI coding assistants (Copilot, Claude Code, Amazon Q) to our existing SDLC, and we're seeing *some* gains — faster boilerplate, quicker lookups, lighter code review prep. But the process itself hasn't changed. We still run two-week sprints. We still write epics. We still hold the same planning and refinement ceremonies.

AWS's argument is that this is the wrong approach. Traditional SDLC rituals were designed around **human cognitive limits and communication overhead** — the time it takes to gather requirements, write specs, align teams, and build incrementally. AI removes or compresses many of those constraints. Keeping the old scaffolding in place means we're driving a faster car on a road with 1970s speed limits.

The gap AI-DLC targets: **the space between "AI helps me write code faster" and "AI changes how we build software altogether."**

---

## What AI-DLC Actually Is

AI-DLC is an open-source methodology (MIT-0 licence) published by AWS Labs, with workflow templates on GitHub (`awslabs/aidlc-workflows`, 700+ stars). It restructures development into three phases:

| Phase | What Happens | AI Role |
|---|---|---|
| **Inception** | Requirements are gathered and specified | AI co-author via *Mob Elaboration* |
| **Construction** | Architecture designed, code written | AI-driven implementation via *Mob Construction* |
| **Operations** | Deployment, monitoring, iteration | Continuous AI-assisted oversight |

### Key Terminology to Know

- **Bolts** — replace sprints. Instead of two-week cycles, work is broken into short, AI-executable bursts measured in hours or days. The idea is that AI can compress implementation time enough to make longer cycles unnecessary.
- **Units of Work** — replace epics. Larger scopes of intent that AI helps decompose into bolts automatically.
- **Mob Elaboration** — a structured session where humans and AI collaboratively produce a specification. Think of it as a requirements workshop where the AI is an active participant drafting, questioning, and refining — not just a note-taker.
- **Mob Construction** — the implementation equivalent: humans set direction and review, AI executes and proposes. Human-in-the-loop approval gates are built into the flow.

AI-DLC is **agent-agnostic** — it supports Kiro (AWS's new AI IDE), Amazon Q Developer, Cursor, Claude Code, and GitHub Copilot. We would not need to change our tooling to trial it.

---

## Real-World Signals

AI-DLC is new — AWS launched it in 2025 — so large-scale independent case studies are not yet available. What we can observe:

| Signal | Detail |
|---|---|
| **GitHub traction** | 700+ stars on `awslabs/aidlc-workflows` shortly after launch — meaningful for a methodology repo, not a product |
| **AWS backing** | Positioned as a first-party AWS methodology, not a community experiment; associated with Amazon Q Developer's enterprise push |
| **Kiro IDE alignment** | AWS launched Kiro (an AI-native IDE) in 2025 with AI-DLC rituals built in — suggesting AWS is committing infrastructure, not just a whitepaper |
| **Analyst interest** | The "bolt AI onto SDLC vs. redesign for AI" debate is now mainstream — similar thinking appears in Gartner's 2025 software engineering notes and GitHub's internal research on Copilot ROI ceilings |
| **Honest caveat** | No peer-reviewed enterprise benchmarks yet. Early adopters are mostly AWS partners and startups, not regulated enterprise environments |

**Bottom line on maturity:** This is early-stage but credible. It is not vaporware — it has real tooling, open-source artefacts, and a clear intellectual foundation. But enterprise-grade validation is still thin.

---

## How We Could Try It — A Low-Risk Trial Path

We do not need to commit the whole organisation. A contained trial can generate real signal within one quarter:

### Phase 1 — Observe (Weeks 1–2)
- Assign one engineer or tech lead to complete AWS's AI-DLC self-paced material and review the GitHub workflow templates.
- Map AI-DLC's constructs (bolts, units of work, Mob Elaboration) against our current sprint/epic/refinement model. Identify where the friction points would be.
- **Output:** A one-page gap analysis — what changes, what stays the same.

### Phase 2 — Pilot Bolt (Weeks 3–6)
- Select one small, well-scoped feature from the backlog — ideally something with clear requirements and no hard regulatory dependencies.
- Run it as a single **bolt** using Mob Elaboration for spec and Mob Construction for implementation, using tools we already have (Claude Code or Copilot).
- Track: time from spec to PR, number of review cycles, developer experience (qualitative).
- **Output:** Bolt retrospective comparing effort and quality against a comparable recent sprint item.

### Phase 3 — Evaluate (Week 7–8)
- Review findings with the team and engineering leadership.
- Decision gate: expand to a full sprint-equivalent trial, park for 6 months, or deprioritise.
- **Output:** Recommendation memo with evidence.

### What This Costs
| Item | Estimate |
|---|---|
| Engineer time (Phase 1–2) | ~3–5 days across 6 weeks |
| Tooling | £0 — uses existing AI tools |
| Risk | Low — one isolated feature, no process change for rest of team |

---

## Key Risks to Flag

| Risk | Why It Matters | Mitigation |
|---|---|---|
| **Governance friction** | Bolts assume fast iteration; our change management and audit requirements may conflict | Scope the pilot to a non-regulated area first |
| **Team disruption** | New rituals require learning investment; teams mid-delivery shouldn't be interrupted | Run pilot with volunteers only |
| **Methodology immaturity** | No enterprise benchmarks yet — we could invest and find it doesn't scale | Time-box the trial; set clear success criteria upfront |
| **AWS lock-in perception** | AI-DLC is AWS-originated; teams may assume it requires AWS tooling | Clarify it is tool-agnostic and MIT-0 licensed |

---

## Recommendation

> **Trial — time-boxed, low-commitment pilot on one feature.**

We are already paying the cost of AI tools. The question is whether we're capturing their full value. AI-DLC's core argument is intellectually sound and backed by enough tooling to be worth a structured look. A 6–8 week pilot costs us very little and will either validate the approach or give us concrete evidence to move on. **We should not adopt wholesale without evidence, but we also should not ignore a methodology that directly challenges the ROI ceiling of our current AI-assisted approach.**

---

*Prepared from intell: AI-DLC Enterprise Evaluation | Phase: Assess | Status: Being Assessed*
*Sources: AWS Labs GitHub (`awslabs/aidlc-workflows`), AWS AI-DLC methodology documentation, intell record.*
