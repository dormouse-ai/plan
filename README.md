# dormouse — plan

Three documents, and that is the point.

| file | what it answers |
|---|---|
| [PLAN.md](PLAN.md) | what we build, in what order, and what "done" means |
| [ARCHITECTURE_V1.md](ARCHITECTURE_V1.md) | the stack, each slot with the measurement that chose it, and the attention/cache arithmetic for a 1M context |
| [NEGATIVE_RESULTS.md](NEGATIVE_RESULTS.md) | the rule: a losing arm is a hypothesis about a bug, not a verdict — eight checks before anything is switched off |

Code lives in [dormouse](https://github.com/dormouse-ai/dormouse) and
[dormouse-core](https://github.com/dormouse-ai/dormouse-core); the landing page and
documentation in [site](https://github.com/dormouse-ai/site).

## The one-line version

1.00 B stored / 46 M active, hybrid attention (3 KDA : 1 CSA) for a 1M context,
MoE for capacity, MoA for expressivity, ternary weights from step 0 — on one 16 GB
card, ~250 MB as a file.
