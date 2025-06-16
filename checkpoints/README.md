# checkpoints/README.md

## ✅ Checkpoints Overview – Operator Validation System

This folder holds mandatory stage completion checklists. Every phase of the validation system has a gate. No stage can proceed without a corresponding checkpoint file that proves it has been passed.

---

### ⛳ Required Checkpoint Files

Each of the following must be filled out and committed before advancing:

- `interviews.md` – 3+ interviews, 1 scored ≥7
- `persona.md` – 1+ persona scored ≥14
- `wedge.md` – 1 wedge loop run with score ≥15
- `monetization.md` – payment, strong quote, or validated price point
- `systems.md` – growth + delivery documented and delegated

---

### 🧾 Checkpoint File Format

Each file follows this structure:

```markdown
# Checkpoint: [Stage Name]

- **Date completed:** [YYYY-MM-DD]
- **Summary of evidence:** [Brief bulletproof notes on signal]
- **Score:** [Numerical score if applicable]
- **Link to supporting docs:** [URL or relative repo path]
```

---

### 🔒 Enforced Use

No code, mocks, or specs may proceed unless checkpoint files are:

- Present
- Scored
- Referenced in the corresponding `/growth-loops/` or `/playbooks/` doc

Example in a test loop file:

```markdown
✅ Checkpoint Met: `../checkpoints/persona.md` → SCORE: 15
```

---

### 📂 Suggested Files

You may also include optional check-ins for:

- `re-interviews.md` – periodic rescoring of key personas
- `delegation.md` – delegation tracker snapshot
- `loop-history.md` – cross-loop pattern trends

These are not enforced, but useful for decision audits and operator handoffs.

---

Keep this folder tightly managed. It represents the heartbeat of your validation integrity.
