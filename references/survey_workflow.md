# Mobile Bimanual Survey Workflow

## Boundary Definitions

Use these definitions consistently:

- `mobile bimanual manipulation`: a mobile platform with two coordinated arms/hands performing physical manipulation where mobility and bimanual coordination both affect success.
- `dual-arm mobile manipulator`: hardware/platform term for a mobile robot carrying two arms.
- `mobile manipulation`: support category when the paper has mobility and manipulation but not bimanual coordination.
- `fixed-base bimanual manipulation`: support category when the paper has two-arm coordination but no mobile base.

Avoid letting the survey become a generic embodied-AI or generic manipulation survey.

## Evidence Levels

Use this evidence hierarchy:

1. Real robot + mobile + bimanual + peer-reviewed.
2. Real robot + mobile manipulation + strong transfer to bimanual feasibility/control/evaluation.
3. Real robot + fixed-base bimanual + strong transfer to bilateral contact, deformables, teleoperation, force, tactile, or learning.
4. Sim/benchmark/platform/preprint that changes infrastructure but is not yet strong evidence of autonomy.
5. Weak application papers only if they reveal a distinct failure model or evaluation practice.

## Reading Order

For a new paper:

1. Read title, abstract, figures, task videos if available.
2. Identify role: core/mobile support/bimanual support/infrastructure/exclude.
3. Read method only enough to determine architecture and key assumptions.
4. Read experiments for robot platform, task difficulty, sample size, metrics, success rates, baselines, ablations, and failure cases.
5. Read limitations and conclusion.
6. Write the 10-field reading note.

Do not fully derive equations unless the paper is a core planning/control paper and the survey section depends on those equations.

## Citation Use

Do not cite papers as decoration. Attach every citation to one of these functions:

- Definition/background.
- Historical anchor.
- Method representative.
- Empirical evidence.
- Benchmark/resource.
- Limitation/failure evidence.
- Open problem support.

One strong paragraph usually needs 2-5 representative citations, not every paper in the subfield.

## Section Drafting Pattern

For each survey subsection, use this pattern:

1. Claim sentence: state the technical point.
2. Historical or conceptual context.
3. Representative papers grouped by mechanism, not one-by-one summaries.
4. Evaluation of what the group proves.
5. Boundary: what remains unsolved or not supported.
6. Transition to the next subsection.

Example claim forms:

- `Base motion is not a navigation prelude; it changes the bilateral feasible set.`
- `Foundation models currently reshape semantic task selection more than contact execution.`
- `Teleoperation is data infrastructure, not merely supervision.`
- `Recovery should be measured as a first-class capability rather than hidden in rollout success.`

## Recommended Figures and Tables

Minimum figures/tables for a strong survey:

- Literature landscape: core, mobile-support, bimanual-support, infrastructure.
- Timeline: classical mobile manipulator -> classic mobile dual-arm platforms -> ALOHA/Mobile ALOHA -> human-demo/data-generation/frontier systems.
- Embodiment and task taxonomy.
- Method landscape across layers: world model, task planning, feasibility, control, learning.
- Evidence matrix: method family vs task family vs evidence strength.
- Benchmark/resource table.
- Open problems matrix.

## Must-Fix Flags

Flag these as major risks:

- The title says mobile bimanual, but most cited papers are single-arm mobile manipulation.
- Preprints are treated as definitive evidence.
- The survey lists papers without a taxonomy or argument.
- Figures are placeholders or decorative.
- Classic platforms/methods are missing.
- No failure/evaluation discussion.
- No distinction between semantic grounding and physical contact feasibility.
- No clear relation to existing surveys.

## Core Anchor Paper Families

Classic mobile manipulation/control:
Seraji 1998, Yamamoto/Yun 1999, Bayle 2001, Oriolo 2005, Fruchard 2006, Yang elastic roadmaps, Pilania planning under uncertainty.

Classic mobile dual-arm/platform systems:
PR2, HERB/HERB 2.0, ARMAR, Rollin Justin, AILA/KIT-style systems, Centauro/BIT-DMR where relevant.

Bimanual manipulation support:
Smith dual-arm survey, bimanual grasp planning, shared control, compliant bimanual control, deformable bimanual manipulation, contact-rich imitation.

Learning/data frontier:
ALOHA, Mobile ALOHA, HoMMI, MoMaGen, BiGym, RoboMIND, YOR, AhaRobot, ALOHA 2.

Mobile manipulation/frontier support:
HomeRobot, OK-Robot, DynaMem, BUMBLE, Mobi-pi, MoManipVLA, MOSART, SafeMimic, LLM-GROP, GPT-4V mobile manipulation.
