# Loophole

Adversarial stress-tester for AI agent permission frameworks.

Feed it your governance rules. It generates edge-case scenarios designed to break them — scope creep, context flips, cascade risks, ambiguity exploits, missing rules, and temporal attacks.

## What it does

Loophole ships with a full permission inventory (80+ rules) and 24 adversarial scenario templates across 6 attack vectors:

- **Context Flip** — valid action becomes dangerous when the context shifts
- **Scope Creep** — small permissions that chain into large ones
- **Cascade Risk** — one failure triggers a domino of downstream failures
- **Ambiguity Exploit** — vague rules that two reasonable people would interpret differently
- **Missing Rule** — actions that fall through every existing gate
- **Temporal Context** — permissions that expire, rotate, or depend on timing

For each scenario, a three-judge panel evaluates whether your framework **holds**, is **ambiguous**, or **breaks**.

## How to use

1. Open `index.html` in a browser (zero dependencies, fully self-contained)
2. Review the embedded permission inventory or paste your own
3. Run scenarios one at a time or in batch
4. Judge each scenario: holds / ambiguous / breaks
5. Track your framework's resilience score in the stats bar
6. Export results as JSON for documentation

## Who it's for

- AI agent developers testing their CLAUDE.md / system prompt governance
- Security teams auditing LLM tool-use policies
- Anyone building autonomous agents who wants to find the gaps before users do

## Live demo

[loophole-ecru.vercel.app](https://loophole-ecru.vercel.app)

## License

MIT
