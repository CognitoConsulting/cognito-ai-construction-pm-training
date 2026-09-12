# Cognito Consulting AI Construction Project Management Training Factory

This repository is the project control system for building an AI Construction Project Management Training Factory for Cognito Consulting. It is currently prepared for Phase 1 only: defining the governance, research questions, fictional project concept direction, data schema, document taxonomy, planted-issue methodology, source/reference categories, training architecture, and quality gates.

No fictional project data, training slides, full curriculum, or fabricated research findings should be created at this stage.

## Repository Structure
- `00_CONTROL/`: governing specification, machine-readable state, task queue, agent configuration, roles, quality rules, and changelog.
- `01_RESEARCH/`: research planning, questions, and source/reference category maps.
- `02_PROJECT/`: project concept, schema, taxonomy, methodology, and training architecture drafts.
- `03_SOURCE_DOCUMENTS/`: supplied or collected source documents.
- `04_CURATED_CONTENT/`: reviewed and reusable curated content.
- `05_EXERCISES/`: exercise designs and scenario materials.
- `06_PROMPTS/`: reusable prompt libraries.
- `07_WORKFLOWS/`: AI workflow procedures and job aids.
- `08_REVIEWS/`: validation notes, review reports, and approval records.
- `09_TRAINER/`: trainer-only guides, answer keys, facilitation notes, and hidden issue maps.
- `10_PARTICIPANT/`: participant-facing materials only.
- `11_PRESENTATION/`: presentation plans and slide assets.
- `12_FINAL/`: approved final deliverables.
- `99_ARCHIVE/`: superseded or retired artifacts.

## Agent Operating Rules
Agents must read `00_CONTROL/MASTER_SPEC.md`, `00_CONTROL/PROJECT_STATE.json`, `00_CONTROL/TASK_QUEUE.json`, `00_CONTROL/AGENT_CONFIG.yaml`, `00_CONTROL/AGENT_ROLES.md`, and `00_CONTROL/QUALITY_RULES.md` before beginning controlled work.

Agents should work only on tasks whose dependencies are satisfied, save outputs to the paths listed in the task queue, and update state only when an actual checkpoint, blocker, error, or approval exists. Model selection should use the tier names in `AGENT_CONFIG.yaml` rather than hardcoded model names.

## Restarting After Failure
To restart after failure:

1. Read `00_CONTROL/PROJECT_STATE.json`.
2. Review any entries in `blocked_tasks` and `errors`.
3. Check `00_CONTROL/TASK_QUEUE.json` for the affected task and dependencies.
4. Resume from the most recent saved or approved artifact.
5. Record the recovery checkpoint before continuing.

## State and Approved Artifacts
Project state is stored in `00_CONTROL/PROJECT_STATE.json`. Phase 1 work is queued in `00_CONTROL/TASK_QUEUE.json`.

Approved artifacts must be listed in `PROJECT_STATE.json` before downstream tasks treat them as authoritative. Final approved deliverables belong in `12_FINAL/`; trainer-only approved materials belong in `09_TRAINER/`; participant-facing approved materials belong in `10_PARTICIPANT/`.
