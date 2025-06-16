# filter.md – /personas/

This file defines how personas are scored, tiered, and qualified for go-to-market motion. Every interview passes through this model before advancing to wedge tests or growth loops.

---

## 🎯 Persona Scoring Criteria

Score each criterion from 0–2:

| Criteria               | 0 = No Signal          | 1 = Partial Signal        | 2 = High Signal                                |
| ---------------------- | ---------------------- | ------------------------- | ---------------------------------------------- |
| **Pain Clarity**       | Vague / abstract       | Recognized but not urgent | Urgent, clear, and quantified                  |
| **Buyer Authority**    | No budget control      | Influencer only           | Final decision-maker / owns budget             |
| **Repeatability**      | Edge case / one-off    | Mid-tier use case         | Frequent, broad, or recurring across verticals |
| **Current Workaround** | None or unclear        | Partial workaround        | Painful, manual, or expensive workaround       |
| **Willingness to Act** | Passive, no next steps | Interested but slow       | Proactive, wants a solution now                |

**Total score: X/10**

---

## 🎯 Persona Tiers and Required Actions

| Tier   | Score | Meaning                | Action                              |
| ------ | ----- | ---------------------- | ----------------------------------- |
| Tier 1 | 9–10  | Direct ICP fit         | Launch wedge experiment immediately |
| Tier 2 | 7–8   | Promising lead         | Run follow-up loop + revalidate     |
| Tier 3 | 5–6   | Weak fit / soft signal | Park in `/suggestions/`             |
| Tier 4 | <5    | No fit                 | Archive                             |

---

## 🧪 Quantifying Interviews

After each interview, create a markdown file in `/interviews/YYYY-MM-DD-[name].md` using the template below:

```markdown
# Interview Summary – YYYY-MM-DD

## Contact

- Name:
- Title:
- Company:
- Segment:

## Pain Summary

> One paragraph summary in their own words

## Criteria Scoring

| Criteria           | Score (0–2) | Notes |
| ------------------ | ----------- | ----- |
| Pain Clarity       |             |       |
| Buyer Authority    |             |       |
| Repeatability      |             |       |
| Current Workaround |             |       |
| Willingness to Act |             |       |

**Total Score: X/10**  
**Tier: 1 / 2 / 3 / 4**

## Next Steps

- [ ] Add to wedge queue
- [ ] Enrich and loop back in
- [ ] Archive or score suggestions
```

### 🧠 System Notes

This scoring model must be applied before any tests or outreach sequences.

If a persona is not a Tier 1 or Tier 2, it cannot enter /growth-loops/.

This file is audited regularly to reduce false positives and founder bias.
