# The Cantica Method - CSIM (Cantica Sequential Inference Method)

**Methodology statement · CSIM v2.0 · August 2026**

Cantica observes the Fin-Tech industry continuously and answers commissioned
questions from the record it builds. This document sets out the method: how
the record is constructed, how a question is resolved against it, what governs
the strength of each claim, and what a client can verify.

To commission a custom Fin-Tech intelligence report: https://www.thebrightminded.com/custom-fin-tech-intelligence-reports-cantica/
To discover more about Cantica's bespoke Fin-Tech reports and intelligence: https://www.thebrightminded.com/cantica/data/
To discover more about how the Fin-Tech publication The Bright Minded uses Cantica for its own business: https://www.thebrightminded.com/cantica/

---

## The record

Cantica reads the Fin-Tech industry every day and writes each public event it
observes into a permanent record — funding, licensing, regulatory action,
enforcement, partnership, product launch, acquisition.

Each entry carries the event, the actor, the jurisdiction, the amounts where
disclosed, the date of the event, the date Cantica observed it, and the
source. Entries are written once. The record is append-only: it grows by
addition and is never rewritten.

### Classification at observation

Each event is classified as it enters the record, under a lens that carries a
version number. The classification establishes the actor, the action, the
object of the action, the jurisdiction, the category, and what any amount
refers to. Once written, it is fixed.

Two consequences follow, and both govern what the method can do.

**Figures are reproducible.** A quantity computed under a given lens version
returns that same quantity whenever it is recomputed under that version.
Cantica stands behind a figure for as long as the report containing it is in
use.

**The record holds the state of knowledge at each date.** Every
classification was made from the record as it stood on the day of observation.
What entered the record, how an actor was resolved, what counted as a single
development, what an amount referred to — each was determined at that moment.
Cantica can therefore compute what a market looked like on a past date, as it
was visible on that date, and report what followed from it.

### Editorial and computational layers

The Bright Minded publishes editorial analysis. Cantica computes data. The two
occupy separate layers of the system.

Editorial fields — the verdict on an event, its reasoning, its implication —
are written at ingest and serve the published editorial layer. The computation
layer loads factual fields only, and the editorial fields are not addressable
from it. This is enforced in code.

Every Cantica figure is computed from the factual record.

---

## Resolving a question

A commissioned question is resolved into three things: the part of the record
it concerns, the kind of answer it requires, and the objective the client is
weighing. Scope is derived from the question by a defined procedure and
recorded, so the boundary of every figure is established before any
computation begins.

Questions resolve into seven stages. Each answers a distinct kind of question,
and each draws on more of the record than the stage below it.

| | Stage | The question it answers |
|---|---|---|
| **1** | State | What is the case |
| **2** | Motion | What is changing, and at what rate |
| **3** | Structure | How the parts relate, and where concentration sits |
| **4** | Divergence | Where a market departs from its own established pattern, and where stated positions depart from observed behaviour |
| **5** | Precedent | What followed, in the record, from configurations comparable to this one |
| **6** | Projection | What follows next, and within what range |
| **7** | Decision | Which course holds across that range |

Each report states the stage it reached. The evidence establishing that a
market is behaving unexpectedly is a different quantity from the evidence
establishing what happens next, and the stage identifies which of the two the
report carries.

---

## The strength of a claim

Every figure in a Cantica report carries one of four marks, stating what the
reader is entitled to conclude from it.

| Mark | What it means |
|---|---|
| **Observed** | This happened. Named, dated, sourced events, provided with the report. |
| **Measured** | A quantity computed over a stated population, disclosed with the figure. |
| **Inferred** | A pattern the evidence supports at a strength that cleared a fixed threshold. |
| **Projected** | A forward statement, given as a range, resting on evidence that cleared the standard beneath it. |

Thresholds are fixed in advance of any commission. A mark carries the same
meaning in every report Cantica issues.

### Admissibility

Two independent conditions govern publication of a claim.

The **gate** establishes that the record supports this class of method for the
scope in question: sufficient history, sufficient coverage, sufficient
distinct observations. The **test** establishes that the individual claim
clears its own bar: strength of evidence, distinct actors behind it, distinct
sources behind it.

Admissibility is a property of the pipeline rather than a review
applied at the end.

---

## Properties of a continuously observed record

A record assembled by continuous observation of a live industry has six
properties that determine how it must be computed. Cantica accounts for each,
and every report reflects them.

**Coverage and market growth are separated.** As Cantica's observation widens,
counts rise across the record. Baselines are coverage-aware and segment
measures are expressed as shares of recorded activity, so a reported
acceleration is a property of the market.

**Volume is counted in developments.** A single announcement is reported
across wires, outlets and languages over several days. Cantica identifies
developments across languages at the point of ingest, so a count reflects the
number of things that happened.

**Every scope is measured at equal statistical power.** The measurement window
is derived from the density of the scope in question. A dense market and a
sparse one are each measured at the resolution their evidence supports, and a
finding's strength reflects the evidence carrying it.

**Expectations are built per scope from that scope's history.** Regulators,
exchanges and competitors act in response to one another, and conditions shift
at deadlines, enforcement actions and market entries. Cantica derives each
expectation from the scope's own record across those shifts.

**Small samples are computed exactly.** A scoped question may hold a few dozen
developments. Cantica computes these quantities exactly, so a finding carries
the same meaning in a narrow market as in a crowded one.

**The standard is enforced by the system.** Gates and tests are applied before
any decision about a report's contents. They hold under deadline, and they
hold identically across every commission.

---

## Verification

Every figure in a commissioned report is delivered with the evidence beneath
it:

```
Figure(
    value       = 2.67e9,
    label       = "disclosed capital",
    events      = [dated, sourced, checkable],
    method_id   = "CSIM-M014",
    method_ver  = "1.2.0",
    lens_ver    = "1.0.0",
    scope_id    = "CSIM-F-2026-0043",
    mark        = "Measured",
    computed_at = "2026-08-09",
)
```

A client confirms that each event exists, is correctly dated, is correctly
sourced, and states what the report attributes to it. The scope is disclosed
alongside: what the figure was computed over, what fell outside it, and the
dates it covers.

Method and lens identifiers are stable across reports and versions, so a
figure issued in one commission can be placed against a figure issued in
another. The events and the scope are disclosed. The computation is
proprietary to Cantica.

---

## Delivery

A commission answers one question and is delivered as a document together with
the data beneath it: the datasets computed for the commission, and the events
supporting every figure.

Scope is fixed before the data is drawn.

---

## Corrections, versions, independence

**Corrections.** The record is permanent and published figures are subject to
correction. Where a figure is found to be wrong, Cantica issues a correction
naming the figure, the reports it appeared in, the corrected value and the
cause. Corrections supersede rather than overwrite, so the original remains
identifiable to anyone who acted on it.

**Versions.** Method version and lens version are carried on every figure.
Figures computed under matching versions are directly comparable, and Cantica
states the relationship where versions differ. This document is versioned on
the same principle. This is v2.0.

**Independence.** Cantica is funded by the clients who commission reports. It
accepts no payment, equity or other consideration from any company in
connection with coverage, inclusion, or a finding.

---

Findings may be cited with attribution to The Bright Minded — Cantica.
Not financial, legal, or investment advice.

*Cantica™ — a proprietary intelligence system of The Bright Minded™.
© 2026 Rosalia Mazza.*
