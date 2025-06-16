# Operator Validation System – Template Repository

This is a structured validation framework for technical operators, startup builders, or fractional CTOs who want to turn raw insight into executable growth systems.

> ⚠️ This is a **template repo**, not a live system. Clone or fork this to run with real data.

---

## 🔧 What This System Does

- Validate or kill product ideas rapidly
- Score and filter customer personas with confidence
- Run high-signal growth loops
- Document execution and team playbooks
- Define off-ramp conditions for founder/operator exit

---

## 🗂 Folder Structure

| Folder                 | Purpose                                                 |
| ---------------------- | ------------------------------------------------------- |
| `/growth-loops/`       | Run structured validation tests on ideas                |
| `/interviews/`         | Capture, score, and process customer insights           |
| `/personas/`           | Score personas and update ICP hypotheses                |
| `/playbooks/`          | Define execution rhythm, hiring, and systems of insight |
| `/off-ramp/`           | Exit planning and operator offboarding                  |
| `/suggestions/`        | Collect and filter raw ideas                            |
| `/wedge/`              | Go-to-market hypotheses and first-win use cases         |
| `patterns.md`          | Synthesized feedback across interviews and loops        |
| `kill-zone.md`         | Kill logic, pivot thresholds, and risk boundaries       |
| `revenue-sightings.md` | Monetization signal log                                 |

---

## 🚦 Workflow: From Insight to Exit

1. **Interview** → Add to `/interviews/`
2. **Score Persona** → `/personas/`
3. **Run Test Loop** → `/growth-loops/`
4. **Capture Signal** → `patterns.md`
5. **Codify Systems** → `/playbooks/`
6. **Exit Planning** → `/off-ramp/`

You build only when loops show pull, revenue signs emerge, and operations scale beyond the founder.

---

## 🧠 System Map

| Layer             | Purpose                                                     |
| ----------------- | ----------------------------------------------------------- |
| Insight Engine    | Raw insight → signal scoring (`/interviews/`, `/personas/`) |
| Validation Engine | Test wedge + persona loops (`/growth-loops/`)               |
| Pattern Engine    | Synthesis of feedback and objections (`patterns.md`)        |
| Execution System  | Scaling through systems and delegation (`/playbooks/`)      |
| Exit Track        | Founder's off-ramp and org durability (`/off-ramp/`)        |

---

## ✅ Build or Kill Criteria

| Milestone                | Condition                                 |
| ------------------------ | ----------------------------------------- |
| Valid Persona            | Score ≥ 14                                |
| Valid Wedge              | Converts repeatedly in loop tests         |
| Revenue Signal           | Confirmed pricing insight or payments     |
| Founder Replacement Path | Systems documented, delegated, stable     |
| Exit Ready               | Off-ramp criteria complete, team executes |

---

## 🚀 Deploy Options

### 1. Markdown-First Repo

Use Git for async tracking, commits, and ops memory.

```
git clone https://github.com/your-org/operator-validation-system.git
```

---

### 2. Notion Workspace Export

Use this structure when importing into Notion:

| Folder / File        | Suggested Notion Table    |
| -------------------- | ------------------------- |
| /interviews/         | Interview Notes           |
| /growth-loops/       | Validation Experiments    |
| /personas/           | Persona Scorecards        |
| /suggestions/        | Feature / Product Backlog |
| revenue-sightings.md | Monetization Signals      |
| /off-ramp/           | SOPs and Delegation Maps  |

---

### 3. Static Docs Site

Use Docusaurus to share this system as a public reference.

```
npx create-docusaurus@latest validation-docs classic
cd validation-docs
cp ../README.md ./docs/index.md
npm run start
```

---

## 🛠️ Automation Suggestions

This repo assumes manual markdown updates for now. To reduce friction:

- Use GitHub Actions or Notion API to auto-update `outcomes.md` from persona, loop, and revenue files.
- Use `checkpoints/` directory as status indicators; an automation could scan for these before merging product code.
- Weekly workflows (cadence.md) can be run via calendar reminders, Notion timeline, or GitHub Issues.

## 📌 Final Notes

- Do not build until repeatable traction is proven.
- This system protects operator time and validates truth over opinion.
- The repo exists to reduce waste, surface pull, and scale deliberately.
