## Omri Galor

Economics at Brown. Four years in **Model Risk at Deutsche Bank** deciding what a model
actually establishes and where it breaks — then venture investing, then co-founding
[Reprium](https://github.com/omrigalor/reprium), then a year of building things end to end.

The thread through all of it: **I care more about whether a number can be defended than
whether it looks good.** Most of what is below ships with its own limitations written down.

---

### Selected work

**[Battery MRI](https://github.com/omrigalor/battery-mri)** — Bayesian optimal experiment design
Instead of measuring a battery and analysing the result, it *designs the measurement*. PyBaMM
predicts two competing degradation hypotheses, a bounded optimizer searches current waveforms
for maximum expected information gain, and synthetic measurements update a Bayesian posterior —
then the next probe is designed against that posterior.
`PyBaMM · SciPy differential evolution · Gauss–Hermite quadrature · FastAPI · React`

**[Journey of Humanity Simulation](https://github.com/omrigalor/journey-of-humanity-simulation)** — Unified Growth Theory, simulated
300,000 years of economic history as a running mechanism rather than an illustration: the
Malthusian trap as an emergent property of the technology–population loop, the quantity–quality
tradeoff, demographic transition, and regional divergence from deep-rooted factors.
`C++ economic core · deterministic counterfactuals · classroom instrumentation`

**[Cardiac Flow Visualization](https://github.com/omrigalor/cardiac-flow-visualization)** — procedural medical anatomy
Right-heart anatomy generated from a public reference atlas, tricuspid leaflet motion on a real
cardiac timeline, regurgitant flow, and a controlled anatomical orbit — rendered deterministically
from Python with no manual modelling, and self-validating before it renders.
`Blender · Python · computational geometry · CC BY 4.0 atlas geometry`

**[GTM Target Scoring](https://github.com/omrigalor/gtm-target-scoring)** — account propensity at scale
Ranks companies on ~165 public signals with full provenance, so any rank traces back to the
sentence that produced it. Fit and timing are scored separately and combined multiplicatively,
because a company that fails badly on one dimension should not hide behind the others.
Validated with conformal prediction: **it ranks reliably and cannot certify any individual
account** — so it orders a queue, it never makes the call.

**[SignalForce](https://github.com/omrigalor/signalforce)** — bounded company research
Two-stage research then strict structured synthesis, with every finding tied to a retrievable
source. Distinguishes *incomplete coverage* from *verified absence*. Keys never touch the browser.

**[Diligence IQ](https://github.com/omrigalor/diligence-iq)** — AI diligence workspace for VC, PE and IB
**[LLM Compliance Pipeline](https://github.com/omrigalor/llm-compliance-data-pipeline)** — generates, judges, dedups and blind-evaluates a QA training set from policy documents
**[AI Agent Portfolio](https://github.com/omrigalor/ai-agent-portfolio)** — production-style agents for recruiting, intake, claims denial-prevention and reimbursement
**[Reprium](https://github.com/omrigalor/reprium)** — relationship-longevity engine calibrated on 3.9M couples (US Patent 11,847,293 B2)

---

### How I build

**Provenance over output.** Every signal in the scoring system keeps the sentence it came from.
When someone asks why a company ranks where it does, there is an answer rather than a shrug.

**Calibration is the deliverable.** Conformal prediction told me the account model ranks but
cannot certify. A bootstrap said a top-fifty position holds about forty percent of the time —
far above chance, nowhere near stable. Both facts are in the README rather than omitted.

**Adversarial by default.** A second independent model re-reads the raw material and argues with
the first. They agree closely about a third of the time, and I record the disagreement as an
uncertainty flag instead of averaging it away, because averaging invents precision.

**Limits stated before they are found.** Battery MRI says plainly that two fixed hypotheses make
EIG monotonic in separation, so updating the prior need not change the optimal waveform. The
cardiac pipeline says it is illustrative and not CFD, FEA or hemodynamics.

---

[omrigalor.com](https://omrigalor.com) · New York
