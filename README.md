# Decider — a calibrated second opinion on two candidate answers

**Paste a question and two candidate answers. Get back which one is stronger, how close the call was, and the
reasoning.** Decider is an AI judge built for the moment when you have two drafts, two plans or two offers and
cannot tell which is better.

- **Use it on Poe**: <https://poe.com/TuringCorp-Decider> (pay per decision, no subscription)
- **What it is, how it is measured, what it costs**: <https://api.turingcorp.net/platform/poe>
- **27 recorded examples, browsable**: <https://api.turingcorp.net/platform/poe/examples>
- **For agents and crawlers**: <https://api.turingcorp.net/platform/llms.txt> · <https://api.turingcorp.net/platform/poe.md>

## Why a judge, not another generator

Ask a model to pick between two answers and you get an opinion. The useful part is not the pick — it is knowing
**how close the call was**. Decider returns a confidence value that is calibrated against outcomes:

| Confidence reported | Observed accuracy (JudgeBench) |
|---|---|
| ≥ 90% | **99.6%** |
| 80–90% | 94.0% |
| 70–80% | 84.1% |
| < 70% | 67.7% |

A high band is permission to commit and move on. A low band is equally useful: it says the two options really are
close, so take the one you already preferred instead of re-reading both again.

**Honest framing**: on raw pick rate Decider ties a plain single-model baseline (≈92.5% vs 92.7% on JudgeBench).
We do not claim to be more accurate. What a single pass cannot give you is the calibrated reading of your own
uncertainty — that is the product. Full tables, including the runs that failed, are published at
<https://api.turingcorp.net/>.

## Try it before paying

The app ships free **recorded runs**: open it, tap a domain chip and read a real decision end to end — the
question, both answers, the pick, the confidence and the full reasoning. Nothing is charged for those. The same
27 cases are browsable as static pages at <https://api.turingcorp.net/platform/poe/examples>.

## Pricing

List **$0.50** per decision; launch offer **$0.25**. One decision = one A/B pair, charged through Poe in compute
points. No subscription, no minimum.

## What this repository is

The public launch kit for the Decider channel: how we describe it, and the material we use when submitting it to
directories and communities (`launch/`). It is not the product source and contains no user data — every example
referenced here was authored by us and recorded from real runs.

Contact: iAsk@turingcorp.net
