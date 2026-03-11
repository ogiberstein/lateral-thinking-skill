---
name: lateral-thinking
description: Adjacent discovery engine for cross-domain, divergent thinking. Surfaces non-obvious connections, hidden mechanism chains, and cross-field analogies that standard analysis misses. Use this skill whenever the user says "what are we missing", "go deeper", "think harder", "think laterally", "cross-domain", wants to break out of a local optimum, needs non-obvious insights, or is stuck on a problem where incremental improvements feel insufficient. Also trigger when the user asks for brainstorming that goes beyond surface-level ideas, wants to apply concepts from one field to solve problems in another, or needs creative problem-solving on any topic — engineering, business, science, design, strategy, writing, or anything else.
---

# Lateral Thinking

> **Credit:** Inspired by the [AI Lateral Thinking Research Generator](https://github.com/jconorgrogan/Ai-lateral-thinking-research-generator) by [jconorgrogan](https://github.com/jconorgrogan).

## Purpose

Standard analysis finds what's known. This skill finds what's *connectable but not yet connected*. It's the difference between "what does the literature say about X" and "what mechanism from adjacent fields explains WHY this happens and what structural change would break the pattern."

Apply this to any domain: engineering, business strategy, product design, scientific research, writing, education, health, policy — anywhere the user is stuck or wants deeper insight.

## When to Activate

- After an approach fails and the obvious fixes feel insufficient
- When incremental improvements won't change the fundamental dynamics
- When the user says "what are we missing?", "go deeper", "think harder"
- When you need to break out of the local optimum of current thinking
- When a problem has been well-studied within its own field but nobody has looked outside it

## Core Principle: Ring Model

Standard knowledge is Ring 0. Start at Ring 2.

- **Ring 0-1 (SKIP PAST):** Direct evidence, known solutions, what's already been tried, what a web search returns, what a domain expert would say first. Assume the user already knows this.
- **Ring 2 (START HERE):** Component decomposition. If mechanism M drives the problem, what regulates M that nobody in this field is looking at? What upstream or parallel systems interact?
- **Ring 3 (THE POINT):** Cross-domain analogies. The same mechanism exists in a completely different field. Adjacent literature that practitioners in the target domain would never read.

## What You're Looking For

1. **Hidden chains:** A → B is known. B → C is known. But A → C hasn't been connected in this context.
2. **Mechanism transfer:** Strategy X works in domain Y. The same underlying mechanism exists in the user's domain but hasn't been applied.
3. **Structural neighbors:** The obvious problem is P. But P cross-talks with Q, and Q has interventions nobody's considered here.
4. **Overlooked modulators:** Upstream factors, feedback loops, environmental details, timing effects, behavioral patterns that shift the system in ways not being tracked.
5. **Inversion:** Instead of "how do we achieve X", ask "what would make X inevitable?" or "who benefits when we fail, and can we become them?" or "what if we wanted the opposite outcome — what does that reveal?"

## Workflow

### Step 1: State the Problem Skeleton

Reduce the user's situation to its mechanical core. Strip away jargon and domain-specific framing — describe the raw dynamics.

Example (product): "We build features. Users try them once. They don't return. We build more features."
Example (health): "Intervention reduces symptom. Symptom returns when intervention stops. Increasing intervention has diminishing returns."
Example (engineering): "System handles normal load. Spike arrives. Recovery takes longer than the spike. Next spike arrives before recovery completes."

### Step 2: Decompose Into Primitives

Break the mechanism into fundamental components:
- **Information flow** — who knows what, when? What signals are being missed or misread?
- **Timing & sequencing** — what order of events creates or destroys value?
- **Incentive structure** — who gets rewarded for what behavior? Where are incentives misaligned?
- **Structural constraints** — what's physically, mathematically, or organizationally impossible?
- **Feedback loops** — what reinforces or dampens the current dynamics?
- **Resource flows** — where does energy, attention, money, or effort actually go vs. where it's intended to go?

### Step 3: Ring 2 — Component-Level Discovery

For each primitive, ask:
- What regulates this that we're not watching?
- What happens if we change this component's sign (e.g., instead of preventing X, deliberately cause X)?
- What's the dual/inverse of this component?
- What adjacent system interacts with this component that nobody in this field monitors?

### Step 4: Ring 3 — Cross-Domain Raid

Search for analogies across fields distant from the user's domain. The further the source field, the more valuable the insight (if the mechanism genuinely transfers). Draw from whichever fields are most relevant, such as:

- **Biology & ecology** (predator-prey dynamics, evolutionary stable strategies, immune systems, ecological niches, symbiosis)
- **Physics & engineering** (resonance, phase transitions, feedback control, thermodynamics, signal processing)
- **Economics & game theory** (Nash equilibria, mechanism design, auction theory, principal-agent problems, market microstructure)
- **Information theory** (signal vs. noise, compression, entropy, channel capacity, error correction)
- **Military strategy** (Boyd's OODA loop, asymmetric warfare, logistics, flanking, attrition vs. maneuver)
- **Network science** (power laws, small worlds, cascading failures, preferential attachment, resilience)
- **Psychology & behavioral science** (cognitive biases, habit formation, social proof, loss aversion, attention economics)
- **Urban planning & architecture** (desire paths, zoning effects, traffic flow, emergent vs. planned order)
- **Medicine & pharmacology** (dose-response curves, side effects as primary effects, homeostasis, resistance)
- **Mathematics** (optimization landscapes, saddle points, dimensionality reduction, symmetry breaking)

For each analogy: what's the mechanism? Does it transfer? What would the user's domain version look like?

### Step 5: Synthesize Hypotheses

For each non-obvious connection discovered:

**Non-obvious connection:** [The link that isn't in standard sources for this domain]

**Mechanism chain:** A → B → C (specify which links are established vs. inferred)

**Why this isn't already known/tried:** [Domain boundary? Different terminology? Recent development in the source field?]

**Adjacent evidence:** [Where this mechanism IS studied, even if not in the user's domain]

**What would test it:** [Specific experiment, prototype, analysis, data check, or action the user could take]

**Estimated impact:** [Order of magnitude — how much could this move the needle?]

### Step 6: Rank and Recommend

Prioritize by: **mechanistic plausibility** × **domain distance** × **testability**

Penalize:
- Anything that appears in standard guides for the user's domain
- Anything that's already been tried or is obvious to practitioners
- Vague "more research needed" without a specific thread to pull
- Ideas that require resources wildly beyond the user's reach
- Surface-level analogies where only the metaphor transfers, not the mechanism

## Output Format

```markdown
## Lateral Thinking: [Problem Statement]

### Mechanism Skeleton
[2-3 sentences: the mechanical core of the problem, stripped of jargon]

### Ring 2: Component Discoveries
[3-5 non-obvious observations about the problem's components]

### Ring 3: Cross-Domain Hypotheses

#### Hypothesis 1: [Name]
- **Source field:**
- **Non-obvious connection:**
- **Mechanism chain:**
- **Why not already known:**
- **Adjacent evidence:**
- **Test:**
- **Estimated impact:**

[Repeat for 3-7 hypotheses]

### Cross-Domain Pointers
[Specific papers, fields, concepts, or literatures to raid for more]

### Recommended Actions
[Ranked list: what to try first, what to investigate, what to discard]
```

## Guardrails

- Never output Ring 0-1 content. If you're stating something that appears in a standard guide for the user's field, you've gone too shallow.
- Every hypothesis must have a testable prediction or actionable next step. "Interesting but untestable" = worthless.
- Cross-domain analogies must specify the MECHANISM that transfers, not just surface similarity. "It's like evolution" is not an insight. "Selection pressure on X creates the same fitness landscape trap as Y, and the escape route in biology was Z" is an insight.
- This is NOT research or literature review. This is divergent thinking followed by convergent ranking. Prioritize novelty of connection over depth of evidence.
- Adapt the cross-domain sources to the user's problem. Don't force-fit every field — pick the 3-5 most mechanistically relevant distant fields for each problem.
