# Royalty Pool Formula v0.1

Machine-readable specification for royalty allocation from permission-aware trace events.  
Built with JSON Schema, YAML examples, and GitHub Actions validation.  
Designed for auditable permission → trace → resonance → allocation workflows.

---

## Overview

`Royalty Pool Formula v0.1` is a machine-readable foundation for **trace-based royalty allocation**.

This repository defines how value can be:

- specified
- calculated
- explained
- visualized
- recorded

The core flow is:

**permission → trace → resonance → allocation → recirculation → audit**

The goal is not to reward raw activity, but to define how value can flow back through **permitted**, **traceable**, and **auditable** contribution structures.

For a compact architectural summary, see [`docs/one-page-overview.md`](docs/one-page-overview.md).

---

## Core Flow

This repository is organized around the following logic:

1. **Permission**  
   Confirm whether a use is permitted, restricted, or prohibited.

2. **Trace**  
   Record relevant trace-linked events in a structured form.

3. **Resonance**  
   Compute contribution scores from similarity, confidence, decay, and policy-aware factors.

4. **Allocation**  
   Normalize contribution scores into proportional royalty shares.

5. **Recirculation**  
   Optionally return part of downstream value to upstream structures or origins.

6. **Audit**  
   Record committed outputs in an append-only, tamper-evident form.

---

## Repository Structure

```text
.
├─ README.md
├─ LICENSE
├─ CITATION.cff
├─ docs/
│  └─ one-page-overview.md
├─ schema/
│  └─ royalty-pool-formula-v0.1.schema.json
├─ examples/
│  └─ royalty-pool-formula-v0.1.sample.yaml
├─ spec/
│  ├─ trace-vector-profile-v0.1.yaml
│  ├─ ara-engine-v0.1.yaml
│  ├─ cultural-lineage-map-v0.1.yaml
│  └─ trace-ledger-architecture-v0.1.yaml
└─ .github/
   └─ workflows/
      └─ validate-specs.yml

## Start Here

This repository can be read from two directions:

- **from formula to system**
- **from system to audit**

For most readers, the recommended reading order is:

### 1. Read this README
Start with the overview, repository structure, and design principles to understand the scope of the repository.

### 2. Open the sample file
Read:

- `examples/royalty-pool-formula-v0.1.sample.yaml`

This is the fastest way to understand the intended document shape.

### 3. Check the validation schema
Open:

- `schema/royalty-pool-formula-v0.1.schema.json`

This defines the machine-readable contract for the formula document.

### 4. Read the trace representation layer
Open:

- `spec/trace-vector-profile-v0.1.yaml`

This defines how traces are represented as a stable multi-vector profile across:

- behavior
- semantic
- structural

It is the bridge between trace capture and ARA scoring.

### 5. Read the execution layer
Open:

- `spec/ara-engine-v0.1.yaml`

This shows how the system computes:

- scoring
- allocation
- hold decisions
- recirculation
- explanation
- ledger events

### 6. Read the visualization layer
Open:

- `spec/cultural-lineage-map-v0.1.yaml`

This shows how lineage, structure reuse, and value flow are visualized.

### 7. Read the audit layer
Open:

- `spec/trace-ledger-architecture-v0.1.yaml`

This shows how committed outputs are stored in an append-only, tamper-evident form.

### 8. Read the one-page summary
Open:

- `docs/one-page-overview.md`

This gives a compact architectural summary.

### 9. Run validation locally
Use the schema validation command described below to confirm that the example passes.

### 10. Review CI behavior
Open:

- `.github/workflows/validate-specs.yml`

This shows how validation is enforced automatically.

### Recommended reading paths

#### For specification readers
README → sample YAML → schema JSON → trace vector profile → ARA spec

#### For architecture readers
README → trace vector profile → ARA spec → lineage map spec → ledger spec

#### For audit / governance readers
README → ledger spec → lineage map spec → license

### In one sentence

This repository defines how trace-aware royalty allocation can be **specified, vectorized, executed, visualized, and audited**.

Directory overview
docs/

Compact high-level documentation.

one-page-overview.md
A one-page architectural summary of the repository.
schema/

Machine-readable validation schemas.

royalty-pool-formula-v0.1.schema.json
JSON Schema for validating the Royalty Pool Formula document structure.
examples/

Human-readable sample specifications.

royalty-pool-formula-v0.1.sample.yaml
A minimal sample document conforming to the schema.
spec/

Core human-readable specifications for execution, visualization, and audit.

ara-engine-v0.1.yaml
Autonomous Royalty Allocator engine specification
cultural-lineage-map-v0.1.yaml
Cultural lineage visualization and graph structure specification
trace-ledger-architecture-v0.1.yaml
Trace ledger architecture for auditability, replayability, and tamper-evident history
.github/workflows/

Continuous Integration workflows.

validate-specs.yml
Automatically validates the schema and example files on push and pull request.
Start Here

This repository can be read from two directions:

from formula to system
from system to audit

For most readers, the recommended reading order is:

1. Read this README

Start with the overview, repository structure, and design principles to understand the scope of the repository.

2. Open the sample file

Read:

examples/royalty-pool-formula-v0.1.sample.yaml

This is the fastest way to understand the intended document shape.

3. Check the validation schema

Open:

schema/royalty-pool-formula-v0.1.schema.json

This defines the machine-readable contract for the formula document.

4. Read the three core specifications

Open these in order:

spec/ara-engine-v0.1.yaml
spec/cultural-lineage-map-v0.1.yaml
spec/trace-ledger-architecture-v0.1.yaml

This sequence shows how the system works:

ARA computes allocation
Cultural Lineage Map visualizes lineage and value flow
Trace Ledger Architecture records committed results for auditability
5. Read the one-page summary

Open:

docs/one-page-overview.md

This gives a compact architectural summary.

6. Run validation locally

Use the schema validation command described below to confirm that the example passes.

7. Review CI behavior

Open:

.github/workflows/validate-specs.yml

This shows how validation is enforced automatically.

Recommended reading paths
For specification readers

README → sample YAML → schema JSON → ARA spec

For architecture readers

README → ARA spec → lineage map spec → ledger spec

For audit / governance readers

README → ledger spec → lineage map spec → license

In one sentence

This repository defines how trace-aware royalty allocation can be specified, executed, visualized, and audited.

Specification Set

This repository currently contains four major specification layers.

1. Royalty Pool Formula

Defines how a distributable royalty pool is calculated and proportionally allocated.

Main role:

turn contribution scores into normalized shares
preserve permission, origin traceability, and agency attribution
support internal accounting units such as QCoin

Key files:

schema/royalty-pool-formula-v0.1.schema.json
examples/royalty-pool-formula-v0.1.sample.yaml
2. ARA Engine

The Autonomous Royalty Allocator is the execution engine.

Main role:

evaluate permission
compute multi-layer similarity
apply confidence, decay, and anomaly controls
generate allocations, holds, and explanations
emit commit-ready ledger events

Key file:

spec/ara-engine-v0.1.yaml
3. Cultural Lineage Map

A graph-based view of how questions, works, structures, traces, and allocations relate.

Main role:

show lineage and derivation
show where value flowed
show what was recirculated upstream
support reviewer understanding and dispute analysis

Key file:

spec/cultural-lineage-map-v0.1.yaml
4. Trace Ledger Architecture

The audit layer that records committed outputs in an append-only, tamper-evident form.

Main role:

store committed events
preserve recalculation history
preserve dispute history
verify payload integrity and hash continuity
separate operational event flow from immutable audit records

Key file:

spec/trace-ledger-architecture-v0.1.yaml
How the pieces connect
Trace Input
   ↓
Royalty Pool Formula
   ↓
ARA Engine
   ├─→ Cultural Lineage Map
   └─→ Trace Ledger Architecture

Or more explicitly:

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
Schema Usage

This repository provides a machine-readable schema and a sample YAML document for the Royalty Pool Formula specification.

Files
schema/royalty-pool-formula-v0.1.schema.json
examples/royalty-pool-formula-v0.1.sample.yaml
.github/workflows/validate-specs.yml
What this does
schema/royalty-pool-formula-v0.1.schema.json
JSON Schema that defines the document structure for Royalty Pool Formula v0.1
examples/royalty-pool-formula-v0.1.sample.yaml
A minimal sample document expected to pass schema validation
.github/workflows/validate-specs.yml
GitHub Actions workflow that automatically validates the sample YAML
Local validation
1. Install dependencies
python -m pip install --upgrade pip
python -m pip install jsonschema PyYAML
2. Validate the sample YAML against the schema
python - <<'PY'
import json
import yaml
from jsonschema import Draft202012Validator

schema_path = "schema/royalty-pool-formula-v0.1.schema.json"
sample_path = "examples/royalty-pool-formula-v0.1.sample.yaml"

with open(schema_path, "r", encoding="utf-8") as f:
    schema = json.load(f)

with open(sample_path, "r", encoding="utf-8") as f:
    sample = yaml.safe_load(f)

validator = Draft202012Validator(schema)
errors = sorted(validator.iter_errors(sample), key=lambda e: e.path)

if errors:
    for err in errors:
        path = ".".join(str(x) for x in err.path)
        print(f"[ERROR] path={path or '<root>'}")
        print(err.message)
        print("-" * 80)
    raise SystemExit(1)

print("Validation passed: royalty-pool-formula-v0.1.sample.yaml")
PY
Expected result
Validation passed: royalty-pool-formula-v0.1.sample.yaml
Validation scope

This schema validates the structural integrity of the specification, including:

top-level required sections
variable definition objects
formula expression containers
similarity weight defaults
policy rule structure
extension blocks
sample input/output structure
Notes
The schema validates document structure, not mathematical correctness.
Formula strings in expression fields are treated as human-readable symbolic expressions.
YAML is used for readability, while JSON Schema is used for deterministic validation.
The GitHub Actions workflow runs the same validation logic automatically on push, pull request, and manual dispatch.
Design Layers

This repository is organized into four layers:

Formula layer
The royalty calculation logic and structural validation rules
Execution layer
The ARA engine that computes scores, allocations, holds, and recirculation
Visualization layer
The Cultural Lineage Map that makes trace, structure, and value flow visible
Audit layer
The Trace Ledger Architecture that records committed results in an append-only, tamper-evident form
Why this structure

This layout separates concerns clearly:

schema/ defines formal validation
examples/ shows minimal valid usage
spec/ defines the higher-level architecture
.github/workflows/ enforces consistency in CI

It is designed to stay readable for humans while remaining extensible for machine-verifiable workflows.

Design Principles

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
Formula Philosophy

This specification is not intended to be a generic engagement score.

It is designed to preserve:

permission-aware use
trace-based allocation
origin traceability
agency attribution
value recirculation
auditability
internal accounting discipline

In other words, the aim is not merely to reward activity, but to formalize how value can flow back through permitted and traceable contribution structures.

One-Page Overview

A compact summary is available here:

docs/one-page-overview.md

That document is recommended for readers who want:

a short architectural summary
the main flow in one page
a quick map of the repository
a faster entry point before reading each spec
Status

Current status: Draft (v0.1.0)

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
Recommended Workflow
Edit the schema in schema/
Update or add examples in examples/
Update core specs in spec/ if architecture changes
Run local validation
Commit changes
Confirm GitHub Actions passes
Update docs/one-page-overview.md when architectural scope changes
Future Expansion

A natural future layout may look like this:

.
├─ docs/
│  ├─ one-page-overview.md
│  └─ architecture-notes.md
├─ schema/
│  ├─ royalty-pool-formula-v0.1.schema.json
│  ├─ royalty-pool-formula-v0.2.schema.json
│  └─ allocation-report-v0.1.schema.json
├─ examples/
│  ├─ royalty-pool-formula-v0.1.sample.yaml
│  ├─ royalty-pool-formula-v0.1.sample.json
│  ├─ allocation-report-v0.1.sample.yaml
│  └─ ledger-event-v0.1.sample.yaml
├─ spec/
│  ├─ ara-engine-v0.1.yaml
│  ├─ cultural-lineage-map-v0.1.yaml
│  ├─ trace-ledger-architecture-v0.1.yaml
│  └─ dispute-review-v0.1.yaml
└─ .github/
   └─ workflows/
      └─ validate-specs.yml

Potential future additions:

semantic version evolution
JSON example support
stricter schema constraints
allocation report schemas
ledger event schemas
dispute review specs
graph export specs
interoperability profiles
signed verification receipts
License

This repository is distributed under the terms described in LICENSE-KAZENE-ROYALTY-CORE.

Please review the license carefully before reuse, modification, redistribution, or compatibility claims.

In short, the license is designed to allow reading, study, implementation, modification, and commercial use, while preserving the core requirements of:

origin visibility
trace preservation
agency attribution
compatibility honesty
value recirculation capability
Citation

If you use this specification, please cite it using the metadata in CITATION.cff
.

Suggested citation source:

CITATION.cff

The repository includes citation metadata for:

title
abstract
version
authorship
keywords
repository URL
Contributing

Contributions may include:

schema refinements
additional examples
validation improvements
documentation cleanup
architectural clarifications
future version drafting

When contributing:

preserve structural clarity
preserve version traceability
avoid silent breaking changes
keep examples and specs aligned
update documentation when behavior changes

A dedicated CONTRIBUTING.md can be added as the repository expands.

Start Summary

If you only open three files, open these first:

examples/royalty-pool-formula-v0.1.sample.yaml
spec/ara-engine-v0.1.yaml
spec/trace-ledger-architecture-v0.1.yaml

That path gives the fastest understanding of:

what the formula looks like
how allocation is executed
how committed results are recorded
In One Line

This repository describes how trace-aware value can be calculated, explained, visualized, and recorded.
