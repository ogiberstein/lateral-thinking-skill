# Lateral Thinking Skill for Claude Code

An adjacent discovery engine for cross-domain, divergent thinking. Surfaces non-obvious connections, hidden mechanism chains, and cross-field analogies that standard analysis misses.

> Inspired by the [AI Lateral Thinking Research Generator](https://github.com/jconorgrogan/Ai-lateral-thinking-research-generator) by [jconorgrogan](https://github.com/jconorgrogan).

## What It Does

Standard analysis finds what's known. This skill finds what's *connectable but not yet connected* — mechanism transfers across distant fields, hidden causal chains, and structural analogies that practitioners in a single domain would never encounter.

It works on any domain: engineering, business strategy, product design, scientific research, writing, education, health, policy, and more.

### The Ring Model

- **Ring 0-1 (skipped):** Known solutions, standard advice, what a domain expert says first.
- **Ring 2 (start here):** Component decomposition — what regulates the problem that nobody is watching?
- **Ring 3 (the point):** Cross-domain raid — the same mechanism exists in a completely different field.

### Trigger Phrases

- "What are we missing?"
- "Go deeper" / "Think harder"
- "Think laterally" / "Cross-domain"
- Any situation where incremental improvements feel insufficient

## Installation

### Claude Code

Copy the skill file to your Claude Code skills directory:

```bash
cp lateral-thinking.md ~/.claude/skills/lateral-thinking.md
```

### As a `.skill` File

If you have the `.skill` archive, extract and copy:

```bash
unzip lateral-thinking.skill -d /tmp/lt
cp /tmp/lt/lateral-thinking/SKILL.md ~/.claude/skills/lateral-thinking.md
```

## Usage

Once installed, the skill activates automatically when you use trigger phrases in Claude Code, or you can invoke it directly:

```
/lateral-thinking
```

## Output Format

The skill produces structured output with:

1. **Mechanism Skeleton** — the raw dynamics of the problem, stripped of jargon
2. **Ring 2: Component Discoveries** — non-obvious observations about the problem's primitives
3. **Ring 3: Cross-Domain Hypotheses** — ranked by mechanistic plausibility × domain distance × testability
4. **Cross-Domain Pointers** — specific fields and concepts to explore further
5. **Recommended Actions** — what to try first, investigate, or discard

## License

MIT
