# DIKWP RefractoRehab OS

High-myopia + astigmatism + presbyopia vision rehabilitation planning system.

This project is an offline, GitHub-ready, non-prescriptive clinical education and rehabilitation planning tool. It helps patients, optometrists, ophthalmologists, and vision rehabilitation teams organize visual task needs, high-myopia safety surveillance, optical-option questions, low-vision adaptations, and clinician handoff notes.

## What it is

- DIKWP vision ledger for refractive triad cases.
- High-myopia risk and overdue surveillance organizer.
- Non-prescriptive optical stack comparison.
- Vision rehabilitation and screen/reading environment planner.
- Red-flag education card.
- Clinician handoff draft.
- AI request guard that blocks prescription, diagnosis, surgery decision, and emergency-triage replacement requests.

## What it is not

It is not a prescription tool, diagnostic tool, surgical recommendation tool, emergency triage substitute, or medical device.

## Quick start

```bash
pip install -e .
refractorehab analyze examples/sample_refractive_rehab_case.json --out outputs/demo
refractorehab guard "write my glasses prescription"
refractorehab static-audit src --out outputs/demo/static_boundary_audit_report.json
```

Open `index.html` for a standalone browser demo.

## DIKWP framing

The system compiles each case into C=(D,I,K,W,P,R): data, information, knowledge, wisdom, purpose, reliability. It follows DIKWP-Mesh 4.0: incomplete, imprecise, inconsistent input is expected; local noise does not automatically kill the conclusion; high-risk symptoms and action boundaries remain hard stops.
