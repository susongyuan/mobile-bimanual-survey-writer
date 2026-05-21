# Mobile Bimanual Survey Writer

A Codex skill for writing and reviewing high-quality robotics survey papers on mobile bimanual manipulation, dual-arm mobile manipulation, whole-body mobile manipulation, teleoperation, robot learning, planning/control, and adjacent embodied-AI manipulation.

The skill is designed for literature screening, paper reading notes, Excel-based survey curation, taxonomy design, evidence-matrix construction, and top-tier reviewer-style audits.

## What It Helps With

- Classifying papers as core mobile bimanual work, mobile-manipulation support, bimanual support, infrastructure, or weak/excluded.
- Extracting structured paper notes: problem, architecture, method, experiments, strengths, limitations, citation use, and relation to prior/later work.
- Maintaining a survey mainline around embodiment, bilateral constraints, mobile feasibility, whole-body control, world models, teleoperation/imitation learning, foundation models, benchmarks, and recovery.
- Auditing whether a survey is ready for top-tier robotics venues and journals.
- Building publication-grade figures and tables such as task taxonomy, method landscape, timeline, evidence matrix, resource table, and open-problem matrix.

## Skill Files

- `SKILL.md`: Main trigger description and compact workflow.
- `references/survey_workflow.md`: Detailed paper-reading and section-writing workflow.
- `references/top_tier_review_bar.md`: Top-tier reviewer checklist and publication readiness bar.
- `agents/openai.yaml`: UI metadata for Codex skill discovery.

## Installation

Copy this folder into your Codex skills directory:

```powershell
Copy-Item -Recurse . "$env:USERPROFILE\.codex\skills\mobile-bimanual-survey-writer"
```

Then invoke it by asking Codex to use `mobile-bimanual-survey-writer` for survey writing, paper screening, or reviewer-style audit tasks.

## License

MIT License. See `LICENSE`.
