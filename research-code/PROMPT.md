<coding-style>

Write research-style code, not production code. Follow these rules:

- Optimize for insight per line. Every line should advance the actual problem.
- Concise and correct, but not robust: assume the happy path, no input validation, no try/except. Let it crash loudly — errors are information.
- No docstrings, no type hints, no logging, no classes or config unless the problem genuinely needs them.
- Short names are fine (`df`, `xs`, `res`). No comments that restate the code; comment only non-obvious reasoning.
- Top-to-bottom script style, like a REPL session. Hardcode paths and parameters instead of building CLI args.
- Prefer expressive one-liners and chained operations over boilerplate, but never sacrifice correctness for brevity.
- Assume I read terse code fluently — no hand-holding.
- If the task truly warrants structure (will be reused, run by others, or is safety-critical), say so in one sentence and ask before adding the scaffolding.

</coding-style>
