# Quality Rules

## Source-of-Truth Hierarchy
`00_CONTROL/MASTER_SPEC.md` is the governing specification. `00_CONTROL/PROJECT_STATE.json` is the authoritative state record. `00_CONTROL/TASK_QUEUE.json` is the authoritative Phase 1 work queue. Approved artifacts listed in `PROJECT_STATE.json` outrank drafts in working folders.

## Hallucination Prevention
Agents must distinguish facts, assumptions, decisions, and placeholders. Research findings require traceable sources. Fictional project content must be labeled as fictional and generated only after dependencies allow it. Unknown items must remain unknown rather than being filled with plausible-sounding detail.

## Construction Realism
Construction scenarios, roles, documents, costs, schedules, risks, and workflows must be internally coherent and plausible for the approved project type. Subject matter that requires expertise must be reviewed before use in participant-facing materials.

## Data Consistency
Project entities must use the approved schema, stable identifiers, consistent names, and controlled statuses. Dates, costs, quantities, stakeholders, locations, and issue histories must not contradict each other across artifacts.

## Document Consistency
Documents must follow the approved taxonomy, naming rules, and version controls. Draft, reviewed, approved, participant-facing, trainer-only, and final materials must remain clearly separated.

## Participant and Answer-Key Separation
Participant materials must never include answer keys, planted-issue maps, scoring rubrics intended only for trainers, hidden issue labels, or facilitation notes. Trainer-only materials must be stored under `09_TRAINER/` unless a reviewed exception is recorded.

## Validation
Before approval, outputs must be checked for dependency compliance, file placement, syntax validity where applicable, source support, data consistency, document consistency, and audience fit. Review findings belong in `08_REVIEWS/`.

## Token and Context Minimization
Agents should use concise artifacts, structured handoffs, stable identifiers, and targeted file reads. Large source documents should be summarized into curated, traceable extracts rather than repeatedly copied into prompts.

## Checkpointing
Meaningful work must update `PROJECT_STATE.json` with checkpoint information, task status, blockers, errors, and approved artifacts as appropriate. No task may be marked complete without a corresponding saved output and review path.

## Failure Recovery
On failure, record the affected task, error summary, recovery recommendation, and last known good artifact. Blocked tasks must identify the missing dependency or decision. Recovery should resume from the last approved or saved checkpoint, not from untracked scratch work.
