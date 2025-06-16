# checkpoints/README.md

## 🧭 Checkpoints – Usage Guide

This folder contains mandatory checkpoint files that document and enforce validation gates. Each file corresponds to a core stage in the system. You cannot progress to the next phase without completing and scoring the current checkpoint.

---

## 📌 Purpose

Checkpoints:

- Enforce discipline
- Capture evidence
- Prevent false signals
- Align execution across async or distributed teams

---

## ✅ How to Use

1. **Clone the correct checkpoint file** from this folder.
2. **Fill out all fields** honestly, with evidence links.
3. **Score the stage** based on internal criteria (see guardrails).
4. **Include checkpoint proof** in any README, mock, or ticket related to the next phase.

---

## 🧱 Template Structure

Each checkpoint file includes:

```markdown
# Checkpoint: [Stage Name]

- Date completed:
- Summary of evidence:
- Score:
- Link to supporting docs:
```

---

## 🚦 Checkpoint Files

| File              | Stage Enforced           |
| ----------------- | ------------------------ |
| `interviews.md`   | ≥3 interviews complete   |
| `persona.md`      | Persona scored ≥14       |
| `wedge.md`        | Wedge loop ≥15 & repeat  |
| `monetization.md` | Pricing or revenue proof |
| `system.md`       | Codified growth + ops    |

Each must be updated and committed before proceeding. They act as gates.

---

## ⛔ Enforcement

> No build, no outreach, and no funding loops without a passing checkpoint file.

Checkpoint contents must be referenced like:

```markdown
✅ Build Check: wedge.md → SCORE 16  
✅ Revenue Signal: strong quote from user X
```

---

## 🧬 Custom Checkpoints

You may add new ones if a stage demands more rigor:

- `delegation.md`
- `support-readiness.md`
- `handoff.md`

Keep them in this folder and maintain the standard structure.

---

## 📂 Location

All checkpoints live in `/checkpoints/` and are tracked like code.

Use them as forced moments of discipline before expanding execution.
