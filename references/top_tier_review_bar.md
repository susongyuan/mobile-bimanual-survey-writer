# Top-Tier Review Bar for Mobile Bimanual Manipulation Surveys

## Submission-Level Thesis

The survey must defend a thesis, not just cover papers. A strong thesis for this topic is:

`Mobile bimanual manipulation is a hierarchical closed-loop problem where mobility changes the bilateral feasible set, perception supplies semantic and geometric beliefs, planning chooses base and hand parameters, and whole-body control survives contact, force, and recovery during execution.`

Every major section should support, refine, or challenge this thesis.

## Core Reviewer Questions

Top-tier reviewers will ask:

1. Why does this topic deserve a separate survey?
2. What does this survey add beyond existing mobile manipulation and dual-arm manipulation surveys?
3. Is the core literature direct enough, or is the argument mostly borrowed from adjacent areas?
4. Are classical systems and methods represented, or is the paper just recent learning hype?
5. Are recent preprints clearly separated from peer-reviewed evidence?
6. Does the taxonomy help researchers design systems, select methods, and compare evidence?
7. Are figures and tables original organizing contributions?
8. Are open problems specific, falsifiable, and connected to evidence?

## Required Evidence Balance

For a strong version of this survey, aim for:

- 20-35 intensively read core/anchor papers.
- 80-140 total high-quality citations for a focused journal survey.
- 15+ direct mobile bimanual or dual-arm mobile system papers when available.
- 20+ adjacent mobile manipulation papers with explicit transfer rationale.
- 20+ fixed-base bimanual/contact/deformable/teleoperation papers when they support bilateral coordination.
- 10-25 platform/dataset/benchmark papers.

Do not force 300-400 citations unless the scope broadens substantially. A narrow, rigorous survey with 120 strong citations is better than a padded 300-citation survey.

## Minimum Figure/Table Package

1. `Scope landscape`: direct core at center, adjacent mobile manipulation and fixed-base bimanual around it, infrastructure/frontier at edge.
2. `Timeline`: classical mobile manipulator theory, classic dual-arm mobile platforms, low-cost teleoperation, open-world/VLA, new datasets.
3. `Embodiment taxonomy`: base, torso/lift, arm arrangement, gripper/sensing, onboard compute/power.
4. `Task taxonomy`: cooperative transport, articulated objects, deformables/long objects, household, industrial/logistics, assistive/medical/field.
5. `Method landscape`: world model, task planning, feasibility, whole-body control, learning, evaluation.
6. `Evidence matrix`: method family vs task family vs real-robot evidence vs limitations.
7. `Benchmark/resource table`: simulator, dataset, platform, model/data resource, what each evaluates and misses.
8. `Open-problem matrix`: current strength, missing evidence, recommended benchmark or method direction.

Figures should not be decorative. Each one should replace several paragraphs of explanation.

## Red Flags That Trigger Major Revision

- The abstract claims mobile bimanual manipulation, but the paper mostly cites single-arm mobile manipulation.
- There is no table of direct mobile bimanual core papers.
- Preprints are mixed with peer-reviewed papers without status labels.
- The survey praises foundation models without explaining contact, force, feasibility, and recovery limits.
- The paper lacks failure-mode or benchmark criticism.
- The taxonomy is obvious or venue-based rather than mechanism-based.
- The review method says "screened many papers" without keywords, sources, criteria, or a PRISMA-like narrative.
- Figures remain placeholders.
- The paper omits classic platforms such as PR2/HERB/ARMAR/Rollin Justin or classic mobile manipulator control/planning.

## Citation Audit

For each strong sentence, label the citation function:

- `D`: definition/background.
- `H`: historical anchor.
- `M`: method representative.
- `E`: empirical evidence.
- `R`: resource/benchmark/platform.
- `L`: limitation/failure evidence.
- `O`: open problem support.

If a citation cannot be assigned one of these functions, it is likely padding.

## Preprint Policy

Use preprints for:

- New datasets/platforms that change the resource landscape.
- Frontier methods not yet represented in archival venues.
- Evidence of emerging trends.

Do not use preprints as:

- Definitive proof of general autonomy.
- The main support for a central claim.
- A replacement for archival classic papers.

Recommended wording:

`These recent preprints are best read as emerging infrastructure or frontier signals rather than settled evidence of autonomous mobile bimanual competence.`

## Section-Level Quality Test

Each section should pass this test:

1. It opens with a claim, not a paper name.
2. It groups papers by mechanism.
3. It compares what the group proves and misses.
4. It ties back to mobile bimanual constraints.
5. It ends with a transition or research implication.

Weak section pattern:

`Paper A did X. Paper B did Y. Paper C did Z.`

Strong section pattern:

`Base placement becomes part of manipulation once both arms share an object. Classical manipulability, uncertainty-aware planning, and learned reachability all address this feasible-set question, but current evidence remains weak for contact-rich recovery and deformables.`

## Final Readiness Decision

Use four levels:

- `Not ready`: mostly literature list; weak boundary; missing classic/frontier coverage.
- `Promising draft`: clear mainline but missing evidence tables, figures, or corpus balance.
- `Submission candidate after revision`: strong thesis and coverage; needs final citation/source audit and figure polish.
- `Top-tier ready`: original taxonomy, strong evidence matrix, complete classic/frontier coverage, cautious claims, polished figures, and clear distinction from existing surveys.
