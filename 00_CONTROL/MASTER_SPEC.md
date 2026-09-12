# Cognito Consulting AI Construction Project Management Training Factory Master Specification

## 1. Objective
Establish a controlled factory for designing an AI-enabled construction project management training program for Cognito Consulting. This specification governs research, project-data design, content curation, exercise creation, workflow design, review, and final packaging.

The repository must support repeatable agent work, clear checkpoints, traceable artifacts, and strict separation between planning, approved source material, participant-facing materials, and trainer-only answers.

## 2. Training Audience
The intended audience is construction project management professionals and adjacent delivery stakeholders who need practical, grounded AI workflows for planning, coordination, controls, documentation, risk management, reporting, and project communication.

Audience assumptions must remain provisional until Phase 1 confirms persona, seniority, organization type, and delivery context.

## 3. Delivery Model
The final training architecture must support three delivery lengths:

- 2-day model: condensed, high-priority workflows and core exercises.
- 3-day model: standard version with deeper practice and review.
- 4-day model: expanded version with additional case work, implementation planning, and facilitation time.

The same core training architecture should scale across all three models without creating contradictory curricula.

## 4. Curriculum Topics
Curriculum topics may include:

- AI fundamentals for construction project management.
- Prompting and task decomposition.
- Project planning, scheduling, and controls.
- Meeting, RFI, submittal, change, risk, and issue workflows.
- Document review and information extraction.
- Stakeholder communication and reporting.
- Quality, safety, cost, and schedule scenario analysis.
- Governance, human review, confidentiality, and responsible AI use.
- Team adoption and workflow integration.

This repository must not generate the full curriculum until later phases approve the training architecture.

## 5. Fictional Construction Project Concept
The training will use one coherent fictional construction project as its case environment. The concept must be realistic enough to support PM documentation, controls, trade coordination, planted issues, and participant exercises.

The specific project concept, data, documents, chronology, stakeholders, risks, costs, schedule details, and issue history are Phase 1 outputs and must not be fabricated outside the approved task flow.

## 6. Required Project Artifacts
The final factory may produce:

- Research question set and reference category map.
- Construction project concept brief.
- Project data schema and document taxonomy.
- Curated content library with source tracking.
- Fictional project data and documents.
- Planted issue methodology and issue register.
- Exercises and scenario prompts.
- AI workflow guides and prompt packs.
- Trainer guide, answer keys, facilitation notes, and review rubrics.
- Participant workbook and clean exercise materials.
- Presentation deck and supporting visuals.
- Final packaged deliverables.

Artifacts become authoritative only after review approval and listing in `00_CONTROL/PROJECT_STATE.json`.

## 7. Required Agent Roles
The factory requires these roles:

- Supervisor
- Research
- Project/Data
- Curation
- Workflow
- Review
- Document Builder
- Final QA

Responsibilities, limits, and handoff rules are defined in `00_CONTROL/AGENT_ROLES.md`.

## 8. Quality Requirements
All outputs must follow `00_CONTROL/QUALITY_RULES.md`. Core requirements include traceability, no unsupported claims, construction realism, data consistency, participant/answer-key separation, validation before approval, checkpointing, and recoverable task state.

## 9. Output Structure
Repository outputs must remain organized by function:

- `00_CONTROL/`: governing state, rules, roles, task queue, and changelog.
- `01_RESEARCH/`: research plans, questions, and source maps.
- `02_PROJECT/`: fictional project concept, schemas, and project data design.
- `03_SOURCE_DOCUMENTS/`: raw or supplied source documents.
- `04_CURATED_CONTENT/`: reviewed excerpts, summaries, and reusable content.
- `05_EXERCISES/`: exercise designs and scenario materials.
- `06_PROMPTS/`: prompt libraries and prompt patterns.
- `07_WORKFLOWS/`: AI workflow procedures and job aids.
- `08_REVIEWS/`: review notes, validation reports, and approvals.
- `09_TRAINER/`: trainer-only guides, answer keys, and facilitation notes.
- `10_PARTICIPANT/`: participant-facing materials only.
- `11_PRESENTATION/`: presentation planning and slide assets.
- `12_FINAL/`: approved final packaged deliverables.
- `99_ARCHIVE/`: superseded or retired artifacts.

## 10. Dependency Rules
Work must proceed by phase and dependency:

- Phase 1 defines the control system, research questions, concept direction, schema, taxonomy, methodology, source categories, training architecture, and quality gates.
- Later phases must not begin until their prerequisite Phase 1 artifacts are approved.
- Fictional data must depend on an approved project concept and schema.
- Exercises must depend on approved fictional data, planted-issue methodology, and workflow goals.
- Participant materials must not include trainer answers or hidden issue keys.
- Final packaging must depend on completed review and Final QA approval.
