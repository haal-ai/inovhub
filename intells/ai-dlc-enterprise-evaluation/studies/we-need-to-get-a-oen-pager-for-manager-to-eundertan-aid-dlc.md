# AI-DLC One-Pager for Management

Intell: AI-DLC Enterprise Evaluation — Measuring AI-Driven Development Efficiency
Type: study
Created: 2026-03-15T00:00:00.000Z

---

# AI-DLC: One-Pager for Management

**Study:** What Is AI-DLC and Should We Try It?
**Intell:** AI-DLC Enterprise Evaluation — Measuring AI-Driven Development Efficiency
**Phase:** Assess · **Status:** Being Assessed · **Expected Impact:** Under Evaluation

---

## Summary

AWS's AI-DLC (AI-Driven Development Life Cycle) is a software delivery methodology that positions AI not as a tool bolted onto existing workflows, but as a **central collaborator** across every phase of development. Rather than adding GitHub Copilot or Claude Code to current sprints and calling it "AI-assisted," AI-DLC proposes redesigning the entire lifecycle around AI — introducing new rituals, new cadence units, and a human-in-the-loop model throughout. The core claim is straightforward but significant: **transformative productivity gains from AI cannot be achieved by keeping the old process intact.** This one-pager explains what the methodology entails, what early signals indicate, and how we could run a low-risk trial.

---

## Problem Space

Most enterprise teams today find themselves in the same position: they have added AI coding assistants (Copilot, Claude Code, Amazon Q) to their existing SDLC and are seeing *some* gains — faster boilerplate generation, quicker lookups, lighter code review preparation. But the underlying process remains unchanged. Teams still run two-week sprints, still write epics, and still hold the same planning and refinement ceremonies.

AWS's argument is that this approach is fundamentally limited. Traditional SDLC rituals were designed around **human cognitive constraints and communication overhead** — the time required to gather requirements, write specifications, align teams, and build incrementally. AI removes or compresses many of those constraints. Retaining the old scaffolding means we are driving a faster car on a road with outdated speed limits.

The gap AI-DLC targets: **the space between "AI helps me write code faster" and "AI changes how we build software altogether."**

---

## What AI-DLC Actually Is

AI-DLC is an open-source methodology (MIT-0 licence) published by AWS Labs, with workflow templates available on GitHub (`awslabs/aidlc-workflows`, 700+ stars). It restructures development into three phases:

| Phase | What Happens | AI Role |
|---|---|---|
| **Inception** | Requirements are gathered and specified | AI co-authors via *Mob Elaboration* |
| **Construction** | Architecture designed, code written | AI-driven implementation via *Mob Construction* |
| **Operations** | Deployment, monitoring, iteration | Continuous AI-assisted oversight |

### Key Terminology

- **Bolts** — replace sprints. Instead of two-week cycles, work is broken into short, AI-executable bursts measured in hours or days. The rationale is that AI can compress implementation time sufficiently to make longer cycles unnecessary.
- **Units of Work** — replace epics. These are larger scopes of intent that AI helps decompose into bolts automatically.
- **Mob Elaboration** — a structured session where humans and AI collaboratively produce a specification. Think of it as a requirements workshop where AI is an active participant — drafting, questioning, and refining — rather than simply a note-taker.
- **Mob Construction** — the implementation equivalent: humans set direction and review while AI executes and proposes solutions. Human-in-the-loop approval gates are built into the flow.

AI-DLC is **agent-agnostic** — it supports Kiro (AWS's AI IDE), Amazon Q Developer, Cursor, Claude Code, and GitHub Copilot. Adopting it would not require changing our current tooling.

---

## Real-World Signals

AI-DLC is new — AWS launched it in 2025 — so large-scale independent case studies are not yet available. Here is what can be observed:

| Signal | Detail |
|---|---|
| **GitHub traction** | 700+ stars on `awslabs/aidlc-workflows` shortly after launch — notable for a methodology repository rather than a product |
| **AWS backing** | Positioned as a first-party AWS methodology, not a community experiment; closely tied to Amazon Q Developer's enterprise push |
| **Kiro IDE alignment** | AWS launched Kiro (an AI-native IDE) in 2025 with AI-DLC rituals built in — indicating a commitment to infrastructure, not just a whitepaper |
| **Analyst interest** | The "bolt AI onto SDLC vs. redesign for AI" debate has become mainstream — similar thinking appears in Gartner's 2025 software engineering notes and GitHub's internal research on Copilot ROI ceilings |
| **Honest caveat** | No peer-reviewed enterprise benchmarks exist yet. Early adopters are predominantly AWS partners and startups, not regulated enterprise environments |

**Bottom line on maturity:** This is early-stage but credible. It is not vaporware — real tooling, open-source artefacts, and a clear intellectual foundation exist. However, enterprise-grade validation remains limited.

---

## How We Could Try It — A Low-Risk Trial Path

Full organisational commitment is not required. A contained trial can generate meaningful signal within one quarter:

### Phase 1 — Observe (Weeks 1–2)
- Assign one engineer or tech lead to complete AWS's AI-DLC self-paced material and review the GitHub workflow templates.
- Map AI-DLC's constructs (bolts, units of work, Mob Elaboration) against our current sprint/epic/refinement model. Identify where the friction points would arise.
- **Output:** A one-page gap analysis — what changes and what remains the same.

### Phase 2 — Pilot Bolt (Weeks 3–6)
- Select one small, well-scoped feature from the backlog — ideally something with clear requirements and no hard regulatory dependencies.
- Run it as a single **bolt** using Mob Elaboration for the specification and Mob Construction for implementation, using our existing tools (Claude Code or Copilot).
- Track: time from specification to PR, number of review cycles, and developer experience (qualitative).
- **Output:** Bolt retrospective comparing effort and quality against a comparable recent sprint item.

### Phase 3 — Evaluate (Weeks 7–8)
- Review findings with the team and engineering leadership.
- Decision gate: expand to a full sprint-equivalent trial, postpone for six months, or deprioritise.
- **Output:** Recommendation memo with supporting evidence.

### What This Costs
| Item | Estimate |
|---|---|
| Engineer time (Phase 1–2) | ~3–5 days across 6 weeks |
| Tooling | £0 — uses existing AI tools |
| Risk | Low — one isolated feature, no process change for the rest of the team |

---

## Key Risks to Flag

| Risk | Why It Matters | Mitigation |
|---|---|---|
| **Governance friction** | Bolts assume fast iteration; our change management and audit requirements may conflict | Scope the pilot to a non-regulated area first |
| **Team disruption** | New rituals require learning investment; teams mid-delivery should not be interrupted | Run the pilot with volunteers only |
| **Methodology immaturity** | No enterprise benchmarks yet — investment could yield findings that it does not scale | Time-box the trial; set clear success criteria upfront |
| **AWS lock-in perception** | AI-DLC is AWS-originated; teams may assume it requires AWS tooling | Clarify that it is tool-agnostic and MIT-0 licensed |

---

## Recommendation

> **Trial — time-boxed, low-commitment pilot on one feature.**

We are already bearing the cost of AI tools. The question is whether we are capturing their full value. AI-DLC's core argument is intellectually sound and supported by sufficient tooling to warrant a structured evaluation. A 6–8 week pilot costs very little and will either validate the approach or provide concrete evidence to move on. **We should not adopt wholesale without evidence, but equally we should not disregard a methodology that directly challenges the ROI ceiling of our current AI-assisted approach.**

---

*Prepared from intell: AI-DLC Enterprise Evaluation | Phase: Assess | Status: Being Assessed*
*Sources: AWS Labs GitHub (`awslabs/aidlc-workflows`), AWS AI-DLC methodology documentation, intell record.*
