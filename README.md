# Confidence Score Explainer

Model the factors behind a UX finding's confidence score and generate a stakeholder-ready explanation.

**[Try it live →](https://dekic648.github.io/confidence-score-explainer/)**

## What it does

Not all UX findings are equally reliable. This tool scores a finding's confidence (0–100) based on the factors that actually determine how much you should trust it, then generates an explanation you can paste directly into a report.

Inputs:
- **Sample size** and **occurrence rate**
- **Study type** (formative, summative, diary, survey)
- **Evidence quality** (direct observation, self-report, mixed)
- **Consistency** across participants
- **Replication** status (seen before or first time?)

Outputs:
- **Confidence score** (10–97) with visual ring chart
- **Grade** (high / moderate / low / very low) with actionable guidance
- **Factor-by-factor breakdown** showing each component's contribution
- **Stakeholder paragraph** ready to paste into a report or slide

## Scoring logic

Base score from sample size (log-scaled, 40 pts max) and occurrence rate (25 pts max). Modifiers for study type, evidence quality, consistency, and replication. Final score bounded to [10, 97] — no finding is ever "certain" or "worthless."

## License

MIT
