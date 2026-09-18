# Reusable blurbs (directory submissions, community posts)

Keep these consistent everywhere — inconsistent descriptions are how a product becomes unrecognisable across
channels. Numbers here must match <https://api.turingcorp.net/> .

## One-liner
**Decider — an AI judge for two candidate answers: it picks the stronger one and tells you how close the call was.**

## Short (≈ 40 words)
Decider takes a question plus two candidate answers (two drafts, two plans, two offers) and returns which one is
stronger, a calibrated confidence value, and the reasoning. Accuracy ties a plain model; the calibrated reading of
how close the call was is the product. Available on Poe, pay per decision.

## Long (≈ 120 words)
Most AI tools generate another answer. Decider judges between two you already have. You give it a question and two
candidate answers; it returns the stronger one, a confidence value calibrated against outcomes, and the reasoning
behind the call. On JudgeBench, judgements it rates 90%+ were correct 99.6% of the time, and the lowest band flags
near-ties where either choice is defensible — an answer, not a failure. It is honest about its limits: on raw pick
rate it ties a single-model baseline, so the value is the calibrated reading, not a claim of superior accuracy. 27
recorded examples are published. Available on Poe: <https://poe.com/TuringCorp-Decider>

## Categories / tags
ai · llm · decision-making · evaluation · confidence-calibration · agent-tools · poe

## Do-not-say list (applies everywhere)
- never "more accurate than X" (we tie the baseline on accuracy)
- never disclosure of vendor/channel internals beyond "multi-model pipeline"
- always name the benchmark (JudgeBench, ContextualJudgeBench) and note these are self-run with failures disclosed
- no absolute guarantees, no "works for every decision"
