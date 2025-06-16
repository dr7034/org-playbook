# system-guardrails.md

## 🛡️ System Guardrails – Operator Validation Framework

A strict minimum bar for signal, repeatability, and system handoff. Ensures quality and prevents wasted cycles.

> 🧠 Decisions governed by /playbooks/operating-principles.md

---

### ✅ Build Conditions

You may proceed with product build **only if all are true**:

- [ ] At least one persona scored ≥14
- [ ] At least one wedge loop scored ≥15 and repeated
- [ ] Revenue signal is observed (conversion, pricing acceptance, or real payment)
- [ ] Loop has been run at least twice and documented
- [ ] Playbook exists for growth and delivery

---

### 🥮 Loop Scoring Method (15+ Criteria)

Each test loop is scored on a 0–5 scale across three axes:

| Axis         | Definition                                              |
| ------------ | ------------------------------------------------------- |
| **Signal**   | Clear pull, opt-in behavior, or intent to pay           |
| **Repeat**   | Action is repeatable across at least 2 personas or runs |
| **Velocity** | Time-to-outcome is <5 days from loop launch to insight  |

**Score = Signal + Repeat + Velocity** → Max: 15

A loop scoring ≥15 is considered strong. Loops under 12 should trigger a kill review.

**Examples of Valid Outcomes for Signal:**

- Call booked via landing page
- Waitlist signup submitted
- Verbal confirmation of need with timeline
- Form fill with project or budget data
- Unprompted request for more info or demo

---

### 🔁 Progression Gate (Enforced Step Flow)

You cannot proceed to the next phase until the prior stage is completed and scored. No skipping.

| Stage                   | Gate Condition                           |
| ----------------------- | ---------------------------------------- |
| **Interviews**          | ≥3 completed, ≥1 scored ≥7               |
| **Persona Fit**         | ≥1 persona scored ≥14                    |
| **Wedge Tests**         | ≥1 loop run + score ≥15                  |
| **Monetization**        | Validated price point or early payments  |
| **System Codification** | Growth + delivery documented + delegated |

Each gate must have its own README-level checkpoint file:
`/checkpoints/interviews.md`, `/checkpoints/persona.md`, etc.

Each checkpoint file must include:

```markdown
# Checkpoint: [Stage Name]

- Date completed:
- Summary of evidence:
- Score:
- Link to supporting docs:
```

---

### 🔄 Automation Guidance

Currently, checkpoint and outcomes files are manually updated. Suggested automation:

- GitHub Actions to validate checklist fields in `outcomes.md`
- Notion API scripts to update matching tables post-edit
- Optional: `checkpoints-sync.js` CLI to auto-generate summaries from source folder markdown

---

### 🧠 Mental Model Enforcement

The principles in `/playbooks/operating-principles.md` apply at every gate. Examples:

- **"Never build before signal"** → no code before Build Gate met
- **"Prioritize loops, not ideas"** → kill suggestions without loop backing
- **"Only trust behavior"** → persona and monetization gates require action, not opinion

---

### 🔒 No Build Without Gate File

Any product code, spec, or mock must include:

```markdown
✅ Build Check: Persona.md → PASSED  
✅ Loop Check: Wedge-Test-1.md → SCORE 16  
✅ Revenue Signal: $ paid / strong quote
```

---

### 🧨 Kill Triggers

If any of these occur, you _must_ archive or pivot:

- [ ] Loop runs 3x with <12 score and no traction
- [ ] Feedback across personas shows critical objection
- [ ] No clear monetization path emerges after 30 days
- [ ] Wedge test score drops >3 points across 2 reruns
- [ ] Delegation score falls below 60% after handoff
- [ ] Persona scoring softens (score <10 on re-interviews)

---

### 🧬 Shortcuts Allowed

Only when specifically noted:

- Early wedge tests can be UX mocks or manual tools
- Persona scoring can be provisional (with raw notes) if <3 interviews
- Suggestions can be skipped if loop ties directly to insight

---

### 📈 Off-Ramp Readiness (Fractional CTO Handoff)

This is the transition from Fractional CTO to durable team execution. It means the systems are now stable, learnable, and accountable **without your direct involvement**. This is _not_ a liquidity event. This is _build-ready handoff_.

You may exit your active role **only when**:

- [ ] Delegation tracker shows ≥80% coverage, ≥50% “Owned”
- [ ] All critical systems (growth loops, delivery, insights) are updating weekly without prompt
- [ ] Tech and product rhythm is codified in playbooks and visible to the team
- [ ] Revenue model is tested, pricing validated, and quoting predictable
- [ ] Weekly async status and monthly postmortem rhythms exist and are followed
- [ ] Escalation pathways are documented and team-assigned
