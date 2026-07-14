# Program Bootstrap workbook schema

Use this schema when creating or validating `Program-Bootstrap-Workbook.xlsx`.

## Global rules

- Make every tab editable and usable in Excel and Google Sheets.
- Hide gridlines, freeze useful headers, enable filters, and use restrained semantic colors.
- Use real spreadsheet dates with `yyyy-mm-dd` formatting.
- Use `Unknown` for expected values that evidence does not establish.
- Use `Not defined` when a measurement or target does not exist.
- Keep source names short but auditable; add section, slide, or page when available.
- Use only these confidence values: `High`, `Medium`, `Low`.
- Use only these evidence states: `Confirmed`, `Reported`, `Inferred`, `Unknown`, `Conflicting`.

## 01 PID

Create a draft Project Initiation Document with these sections:

1. Document control
2. Initiation recommendation
3. Background and rationale
4. Mandate
5. Intended outcomes and success
6. Scope and constraints
7. Outputs and deliverables summary
8. Workstreams and execution approach
9. Milestones and timeline
10. Governance and decision rights
11. Measures of success
12. Program controls summary
13. Open decisions and critical gaps
14. Recommended first actions
15. Approval

Include these document-control fields:

- Program name
- Version
- Date created
- Evidence cutoff date
- Prepared by
- Status
- Overall confidence

Use one of these initiation recommendations:

- `Ready to initiate`
- `Ready with stated assumptions`
- `Not ready — critical decisions required`

Keep approval fields blank unless an authorized human supplies them.

## 02 Workstream Map

Create a compact PID companion table with exactly these columns:

| Column | Rule |
|---|---|
| Workstream | One row for each identified workstream |
| Deliverables | The related deliverable name; include its stable ID when available |
| Measure | The extracted measurement, KPI, or key result; use `Not defined` when absent |

Keep this tab deliberately simple. Do not add ownership, dates, provenance, confidence, or status columns; those details belong in the supporting tabs.

## 03 Deliverables

Required columns:

| Column | Rule |
|---|---|
| ID | Stable identifier such as `DEL-001` |
| Deliverable | Named output or `Unknown` |
| Intended outcome | Why the output matters |
| Workstream | Related workstream or `Unknown` |
| Owner | Evidence-backed owner or `Unknown` |
| Milestone / due date | Real date when available |
| Acceptance criteria | Evidence-backed completion condition or `Unknown` |
| Status | `Not started`, `In progress`, `Blocked`, `Complete`, or `Unknown` |
| Source | File and location |
| Evidence state | Required controlled value |
| Confidence | `High`, `Medium`, or `Low` |

## 04 Workstreams & Measures

Required columns:

| Column | Rule |
|---|---|
| Workstream | Stable name or `Unknown` |
| Objective / outcome | Required explanation of intended result |
| Lead | Evidence-backed lead or `Unknown` |
| Deliverables | IDs from the Deliverables tab |
| Milestones | Known milestone names or dates |
| Measure type | `OKR`, `KPI`, `Metric`, `SLA`, or `Not defined` |
| Measurement / key result | Extracted measure or `Not defined` |
| Baseline | Typed value when available; otherwise `Unknown` |
| Target | Typed value when available; otherwise `Not defined` |
| Current | Typed value when available; otherwise `Unknown` |
| Dependencies | Related teams, systems, decisions, or deliverables |
| Source | File and location |
| Evidence state | Required controlled value |
| Confidence | `High`, `Medium`, or `Low` |

Do not generate an OKR merely to fill a row. Preserve existing OKRs exactly enough to retain meaning. Flag absent or weak measures for later OKR Builder work.

## 05 RAID

Required columns:

| Column | Rule |
|---|---|
| ID | Stable identifier such as `RAID-001` |
| Type | `Risk`, `Assumption`, `Issue`, or `Dependency` |
| Description | Clear statement of the item |
| Workstream | Related workstream or `Program-wide` |
| Owner | Evidence-backed owner or `Unknown` |
| Probability | `High`, `Medium`, `Low`, or `N/A` |
| Impact | `High`, `Medium`, `Low`, or `N/A` |
| Priority | `Critical`, `High`, `Medium`, or `Low` |
| Mitigation / action | Existing or recommended response; label recommendations |
| Due date | Real date when available |
| Status | `Open`, `Monitoring`, `Mitigating`, `Blocked`, `Closed`, or `Unknown` |
| Source | File and location |
| Evidence state | Required controlled value |
| Confidence | `High`, `Medium`, or `Low` |

## 06 Evidence & Gaps

Create a `Source inventory` table with:

- Source
- Source date
- Apparent purpose
- Apparent authority
- Freshness
- Relevant content
- Limitations

Create a `Critical gaps` table with:

- Gap ID
- Gap or conflict
- Why it matters
- Impacted workstream
- Priority
- Recommended resolver
- Status
- Related sources

Create an `Evidence legend` showing the five evidence states and their meanings.
