---
name: mobile-bimanual-survey-writer
description: Literature-review and survey-writing workflow for mobile bimanual manipulation, dual-arm mobile manipulation, whole-body mobile manipulation, robotic teleoperation, imitation learning, planning/control, embodied-AI mobile manipulation, and adjacent fixed-base bimanual manipulation. Use when screening papers, reading PDFs, updating survey Excel files, classifying intensive/skimming papers, drafting taxonomy sections, building evidence tables, auditing citations, or reviewing a robotics survey from a top-tier reviewer perspective.
---

# Mobile Bimanual Survey Writer

## Core Stance

Treat the user's survey as an argumentative robotics survey, not a bibliography dump. Keep the main boundary:

`mobile bimanual manipulation / dual-arm mobile manipulation`

Use adjacent literature only when it transfers to one of these layers: embodiment, world modeling, task/skill selection, motion feasibility, whole-body control, teleoperation/imitation learning, data/benchmarking, or evaluation/recovery.

Aim for a top-tier review standard: every included paper must either define the field, support a taxonomy, provide representative evidence, expose a failure mode, or motivate an open problem. Do not add papers just to increase the citation count.

## Top-Tier Quality Bar

A survey output is not top-tier ready unless it has:

- A defensible scope distinct from existing mobile manipulation, fixed-base bimanual, foundation-model manipulation, and assistive-robot surveys.
- A core corpus of direct mobile bimanual papers plus adjacent work whose transfer rationale is explicit.
- A taxonomy that is useful to future researchers, not only a list of topics.
- Evidence tables that connect paper groups to claims, tasks, platforms, metrics, and limitations.
- Clear separation between peer-reviewed evidence, preprints, datasets, platforms, and demos.
- Real figures/tables with intellectual content: timeline, method landscape, embodiment/task taxonomy, resource table, evidence matrix, and open-problem matrix.
- Reviewer-grade limitations: what the field can do, what it cannot yet prove, and where current evaluation is weak.

## Paper Triage

Classify every paper into one of five roles:

1. `Core`: mobile base + two arms/bimanual manipulation are central.
2. `Mobile Support`: mobile manipulation, whole-body mobile control, VLA/LLM mobile manipulation, or mobile benchmarks, but not bimanual.
3. `Bimanual Support`: fixed-base dual-arm/bimanual manipulation, deformables, contact-rich manipulation, force/tactile, or bimanual teleoperation.
4. `Infrastructure`: dataset, platform, simulator, benchmark, open-source hardware, or teleoperation/data pipeline.
5. `Exclude/Weak`: generic embodied AI, generic manipulation, or weak venue/application paper with no transferable insight.

Prefer top-tier/archival venues: `T-RO`, `IJRR`, `Science Robotics`, `RA-L`, `ICRA`, `IROS`, `RSS`, `CoRL`, `ICLR`, `NeurIPS`, `CVPR` when directly relevant, `Annual Review`, `JFR`, `RAS`, `T-Mech`, `T-ASE`. Use preprints only as emerging infrastructure or frontier signals, and label them explicitly.

When paper status, venue, or latest frontier coverage may have changed, verify with web sources before making a strong claim. Prefer primary sources: publisher pages, conference proceedings, arXiv, official project pages, author pages, DBLP, Semantic Scholar/OpenAlex only as secondary cross-checks.

## Reading Template

For each paper, produce this compact note:

```text
Paper role:
Problem solved:
System architecture:
Core method:
Experimental setup:
Main results:
Strengths:
Limitations:
What this paper proves:
What this paper does not prove:
Best survey section to cite it in:
Exact survey claim it can support:
Relationship to prior and later work:
Intensive/skimming recommendation:
```

Keep the answer evaluative. Do not restate the abstract. Identify what the paper proves, what it does not prove, and which survey claim it can support.

## Evidence Matrix

When comparing papers, prefer a matrix with these fields:

`Paper | Role | Platform | Mobile? | Bimanual? | Real robot? | Task family | Method layer | Data source | Metrics | Main evidence | Main limitation | Citation use`

Use this matrix to decide whether a section is over-dependent on adjacent single-arm mobile manipulation or fixed-base bimanual work.

## Survey Mainline

Use this default mainline unless the user changes direction:

1. Why mobile bimanual manipulation deserves a separate survey.
2. Historical roots: classical mobile manipulators + fixed-base bimanual manipulation.
3. Embodiment/platform taxonomy: differential/holonomic/legged base, torso/lift, symmetric/wide-baseline arms, end-effectors, sensing.
4. Task taxonomy: cooperative transport, articulated objects, deformables/long objects, household service, industrial/logistics, assistive/medical/field tasks.
5. Motion and feasibility: base placement, reachability, manipulability, TAMP, uncertainty.
6. Whole-body control: QP/MPC, nonholonomic constraints, closed-chain constraints, internal force, compliance.
7. Perception/world models: scene memory, open-vocabulary maps, articulated models, active viewpoint selection.
8. Learning/data: teleoperation, imitation learning, co-training, human demonstrations, data generation, RL/self-improvement.
9. Foundation models/VLA: semantic grounding and task selection, but not a direct replacement for contact execution.
10. Platforms/benchmarks/evaluation: datasets, simulators, real-world protocols, recovery, contact quality, human intervention.
11. Open problems: semantics-contact gap, recovery, deformables, tactile/force sensing, morphology-aware transfer, benchmark standardization.

## Excel Updates

When modifying the user's survey Excel:

- Preserve the original file unless the user explicitly asks to overwrite it; create a dated copy.
- Add a dedicated audit/addition sheet for new papers.
- Keep columns compatible with the user's existing sheets: year, title, venue, paper type, topic, relevance, reading recommendation, overview, contribution, writing insight, recommended chapter, terms, URL, citation.
- Highlight newly added rows.
- Deduplicate by normalized title across all sheets.
- Separate `Peer-reviewed` from `Preprint / not peer-reviewed yet`.

## Reviewer Audit

When asked whether a survey is top-tier ready, check:

- Is the boundary clear enough to avoid becoming generic mobile manipulation?
- Does the paper justify why mobile bimanual is not merely mobile + dual-arm?
- Is the inner corpus large enough, or is the argument mostly adjacent literature?
- Are classic platforms and methods included: PR2, HERB/HERB 2.0, ARMAR, Rollin Justin, ALOHA/Mobile ALOHA, classical mobile manipulator control/planning?
- Are frontier items handled carefully: Mobile ALOHA, HoMMI, MoMaGen, BiGym, YOR, AhaRobot, RoboMIND, Mobi-pi, MoManipVLA, BUMBLE, MOSART, SafeMimic?
- Are figures real taxonomy/evidence contributions rather than decoration?
- Are preprints labeled as frontier signals, not settled evidence?
- Does every strong claim have concrete supporting citations?
- Are open problems specific enough to guide research?

Use a direct reviewer tone:

1. `Summary judgment`
2. `Accept-like strengths`
3. `Major concerns`
4. `Minor concerns`
5. `Must-fix before submission`
6. `Concrete revision plan`
7. `Residual risk after revision`

Be skeptical of claims like "general", "robust", "whole-body", "foundation model", "real-world", and "benchmark" unless the experiments and citations justify them.

## Ten-Pass Audit

For high-stakes survey drafts, audit in this order:

1. Scope and title.
2. Novelty versus existing surveys.
3. Core/adjacent citation balance.
4. Classic platform and theory coverage.
5. Frontier coverage and preprint labeling.
6. Taxonomy usefulness.
7. Evidence behind strong claims.
8. Figure/table contribution.
9. Evaluation and benchmark criticism.
10. Writing coherence and reviewer objections.

## Use References

Load `references/survey_workflow.md` when the user asks for detailed process, section planning, reading workflow, paper-screening standards, or reviewer checklists.

Load `references/top_tier_review_bar.md` when the user asks for publication readiness, top-tier/top-conference quality, reviewer-style judgment, or multiple-round audit.
