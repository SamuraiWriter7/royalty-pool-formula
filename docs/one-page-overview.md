# One-Page Overview

## What this repository is

This repository defines a machine-readable foundation for **trace-based royalty allocation**.

It describes how value can be:

- specified
- calculated
- explained
- visualized
- recorded

The core flow is:

**permission → trace → resonance → allocation → recirculation → audit**

The aim is not to reward raw activity, but to define how value can flow back through **permitted**, **traceable**, and **auditable** contribution structures.

---

## Core components

### 1. Royalty Pool Formula

Defines how a distributable royalty pool is calculated and proportionally allocated.

Main role:

- turn contribution scores into normalized shares
- preserve permission, origin traceability, and agency attribution
- support internal accounting units such as QCoin

Key files:

- `schema/royalty-pool-formula-v0.1.schema.json`
- `examples/royalty-pool-formula-v0.1.sample.yaml`

---

### 2. ARA Engine

The **Autonomous Royalty Allocator** is the execution engine.

Main role:

- evaluate permission
- compute multi-layer similarity
- apply confidence, decay, and anomaly controls
- generate allocations, holds, and explanations
- emit commit-ready ledger events

Key file:

- `spec/ara-engine-v0.1.yaml`

---

### 3. Cultural Lineage Map

A graph-based view of how questions, works, structures, traces, and allocations relate.

Main role:

- show lineage and derivation
- show where value flowed
- show what was recirculated upstream
- support reviewer understanding and dispute analysis

Key file:

- `spec/cultural-lineage-map-v0.1.yaml`

---

### 4. Trace Ledger Architecture

The audit layer that records committed outputs in an append-only, tamper-evident form.

Main role:

- store committed events
- preserve recalculation history
- preserve dispute history
- verify payload integrity and hash continuity
- separate operational event flow from immutable audit records

Key file:

- `spec/trace-ledger-architecture-v0.1.yaml`

---

## How the pieces connect

```text
Trace Input
   ↓
Royalty Pool Formula
   ↓
ARA Engine
   ├─→ Cultural Lineage Map
   └─→ Trace Ledger Architecture

permission
   ↓
trace capture
   ↓
resonance scoring
   ↓
allocation
   ↓
recirculation
   ↓
audit commit

README.md
LICENSE-KAZENE-ROYALTY-CORE
CITATION.cff
docs/
schema/
examples/
spec/
.github/workflows/

.
├─ README.md
├─ LICENSE-KAZENE-ROYALTY-CORE
├─ CITATION.cff
├─ docs/
│  └─ one-page-overview.md
├─ schema/
│  └─ royalty-pool-formula-v0.1.schema.json
├─ examples/
│  └─ royalty-pool-formula-v0.1.sample.yaml
├─ spec/
│  ├─ ara-engine-v0.1.yaml
│  ├─ cultural-lineage-map-v0.1.yaml
│  └─ trace-ledger-architecture-v0.1.yaml
└─ .github/
   └─ workflows/
      └─ validate-specs.yml

Reading order

Recommended reading order:

README.md
examples/royalty-pool-formula-v0.1.sample.yaml
schema/royalty-pool-formula-v0.1.schema.json
spec/ara-engine-v0.1.yaml
spec/cultural-lineage-map-v0.1.yaml
spec/trace-ledger-architecture-v0.1.yaml
Short reading paths
For specification readers

README → sample YAML → schema JSON → ARA spec

For architecture readers

README → ARA spec → lineage map spec → ledger spec

For audit / governance readers

README → ledger spec → lineage map spec → license

Design principles

This repository is based on the following principles:

Permission first
No valid allocation without valid permission context.
Trace before reward
Value should not be allocated without trace-linked reasoning.
Origin traceability
Upstream origins should remain visible.
Agency attribution
The acting or represented subject should remain attributable.
Auditability
Allocation decisions should be reviewable, replayable, and tamper-evident.
Internal accounting
The current scope uses internal accounting units rather than speculative tokenization.
Extensibility
Formula, engine, visualization, and ledger layers should remain versionable and replaceable.
Current scope

This repository currently defines:

machine-readable formula structure
human-readable execution architecture
lineage visualization structure
append-only audit architecture
validation workflow
citation metadata
a custom core-preservation license

This repository does not yet define:

external payment rails
token markets
public blockchain deployment
legal settlement enforcement
production UI implementation
Validation

The repository includes:

a JSON Schema for the formula document
a sample YAML file expected to pass validation
a GitHub Actions workflow for automatic checking

Main validation files:

schema/royalty-pool-formula-v0.1.schema.json
examples/royalty-pool-formula-v0.1.sample.yaml
.github/workflows/validate-specs.yml
License and citation
License

This repository is distributed under the terms described in LICENSE-KAZENE-ROYALTY-CORE.

In short, the license is designed to allow reading, study, implementation, modification, and commercial use, while preserving the core requirements of:

origin visibility
trace preservation
agency attribution
compatibility honesty
value recirculation capability
Citation

If you use this specification, please cite it using the metadata in CITATION.cff.

In one line

This repository describes how trace-aware value can be calculated, explained, visualized, and recorded.
