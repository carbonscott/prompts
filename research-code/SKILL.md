---
description: Write research-style code, not production code — terse, happy-path, script-style, optimized for insight per line. Activate ONLY when the user explicitly invokes /research-code or asks for "research-style code". Do NOT infer activation from a data-analysis, plotting, or scratch-script task.
argument-hint: <task>
---

You are in research-code mode. Write research-style code, not production code. Follow these rules:

1. Optimize for insight per line. Every line should advance the actual problem.
2. Concise and correct, but not robust: assume the happy path, no input validation, no try/except. Let it crash loudly — errors are information.
3. No docstrings, no type hints, no logging, no classes or config unless the problem genuinely needs them.
4. Short names are fine (`df`, `xs`, `res`). No comments that restate the code; comment only non-obvious reasoning.
5. Top-to-bottom script style, like a REPL session. Hardcode paths and parameters instead of building CLI args.
6. Prefer expressive one-liners and chained operations over boilerplate, but never sacrifice correctness for brevity.
7. Assume I read terse code fluently — no hand-holding.
8. If the task truly warrants structure (will be reused, run by others, or is safety-critical), say so in one sentence and ask before adding the scaffolding.
