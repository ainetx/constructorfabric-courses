# Constructor Studio Academy - Course Blueprint and Table of Contents

## 0. Course Frame

Description: This course teaches Constructor Studio from first principles through advanced operation and extension authoring. It uses the established Constructor Studio terminology throughout the learner-facing material.

### 0.1 Audience and Tracks

Description: The course has one shared foundation, then separates into an Operator track and a Kit and Extension Author track. Learners can complete the Operator track alone or continue into authoring and certification work.

#### Lessons and Checkpoints

- 0.1.1 Who the course is for
- 0.1.2 Operator path: using Constructor Studio in real projects
- 0.1.3 Author path: building kits, workflows, skills, and extensions
- 0.1.4 Recommended paths by role
- 0.1.5 Checkpoint: choose your learner path

### 0.2 Command and Terminology Standard

Description: All lessons use the standard Constructor Studio names: Constructor Studio, `cfs`, `/cf`, `/cf-studio`, and `/cf-*`. Learners practice the command vocabulary they will use in real projects.

#### Lessons and Checkpoints

- 0.2.1 Product name: Constructor Studio
- 0.2.2 CLI name: `cfs`
- 0.2.3 Root skill and activation: `/cf`
- 0.2.4 Studio command surface: `/cf-studio`
- 0.2.5 Core workflow commands: `/cf-plan`, `/cf-generate`, `/cf-analyze`
- 0.2.6 Kit workflow commands: `/cf-{kit}-{name}`
- 0.2.7 Naming practice: choosing the right command form

### 0.3 Course Project and Assessment Model

Description: The course uses one running repository project so each concept becomes a practical artifact, command, or workflow result. Assessments emphasize repeatable operation, traceability, validation, and review readiness.

#### Lessons and Checkpoints

- 0.3.1 The running course repository
- 0.3.2 What learners will build
- 0.3.3 Labs, checkpoints, and capstone rules
- 0.3.4 Evidence required for completion
- 0.3.5 Certification rubric overview

## 1. Foundation - Mental Model and Operating Principles

Description: This part explains what Constructor Studio is, where it fits around AI coding tools, and why the system uses artifacts, workflows, validation, and traceability instead of one long prompt.

### 1.1 What Constructor Studio Is

Description: Learners build a simple mental model: Constructor Studio is the workflow, context, and validation layer around an AI coding tool. It helps teams keep requirements, design, plans, and code aligned.

#### Lessons and Checkpoints

- 1.1.1 The core problem: AI work without durable control surfaces
- 1.1.2 Constructor Studio as a repo-attached delivery system
- 1.1.3 Inspectable artifacts versus chat memory
- 1.1.4 Deterministic checks versus model reasoning
- 1.1.5 Checkpoint: explain the system in one paragraph

### 1.2 Actors and Responsibilities

Description: This module separates the responsibilities of the human, AI coding tool, agent, Constructor Studio, CLI, and CI pipeline. The goal is to prevent learners from treating the system as either magic automation or just documentation.

#### Lessons and Checkpoints

- 1.2.1 Human owner and approval authority
- 1.2.2 AI coding tool as the host environment
- 1.2.3 Agent as the reasoning and writing executor
- 1.2.4 Constructor Studio as workflow and validation control
- 1.2.5 `cfs` as deterministic local and CI interface
- 1.2.6 Checkpoint: assign responsibilities for a change request

### 1.3 The Artifact-First Delivery Model

Description: Learners see how requirements, design, decomposition, features, plans, implementation, and review outputs form a delivery chain. This module introduces stable IDs and links without going deep into validation internals yet.

#### Lessons and Checkpoints

- 1.3.1 Why artifacts exist
- 1.3.2 Requirement to design to plan to code
- 1.3.3 Stable identifiers and references
- 1.3.4 Drift as a visible signal
- 1.3.5 Lab: read a simple evidence chain

### 1.4 Fit and Non-Fit

Description: This module teaches when Constructor Studio is worth the overhead and when a normal edit is better. Learners practice choosing based on risk, ambiguity, review pressure, and traceability needs.

#### Lessons and Checkpoints

- 1.4.1 Good fit: risky, multi-step, review-sensitive work
- 1.4.2 Good fit: brownfield understanding before editing
- 1.4.3 Non-fit: tiny edits and throwaway spikes
- 1.4.4 Tradeoff: more structure for more control
- 1.4.5 Checkpoint: classify ten work requests

### 1.5 Core Vocabulary

Description: This module establishes the language used across the rest of the course. Terms are defined as the normal Constructor Studio vocabulary learners will use in daily work.

#### Lessons and Checkpoints

- 1.5.1 Project, setup directory, and Studio installation
- 1.5.2 Artifacts, systems, codebases, and registries
- 1.5.3 Workflows, skills, commands, and generated integrations
- 1.5.4 Kits, templates, rules, checklists, and examples
- 1.5.5 Workspace sources and cross-repo resolution
- 1.5.6 Checkpoint: vocabulary matching exercise

## 2. Getting Started - Installation, Setup, and First Use

Description: This part takes a new learner from no installed tool to a working repository with generated agent integrations and a first useful workflow run.

### 2.1 Local Prerequisites

Description: Learners prepare the development environment required for Constructor Studio. The module keeps the setup practical and focuses only on what is needed to run the system.

#### Lessons and Checkpoints

- 2.1.1 Required tools: Python, Git, `pipx`, and AI coding host
- 2.1.2 Optional tools: GitHub CLI for PR workflows
- 2.1.3 Supported hosts and practical differences
- 2.1.4 Environment checks before installation
- 2.1.5 Lab: verify prerequisites

### 2.2 Installing the CLI

Description: This module introduces `cfs` as the Constructor Studio CLI. Learners verify installation before touching a project.

#### Lessons and Checkpoints

- 2.2.1 Installing `cfs`
- 2.2.2 Verifying the installed executable
- 2.2.3 Checking CLI version
- 2.2.4 Understanding global proxy behavior
- 2.2.5 Troubleshooting PATH issues
- 2.2.6 Lab: install and verify the CLI

### 2.3 Initializing a Repository

Description: Learners initialize Constructor Studio in a repository and inspect the generated surfaces. The focus is on what gets created, what is generated, and what the user owns.

#### Lessons and Checkpoints

- 2.3.1 Running `cfs init`
- 2.3.2 Choosing the setup directory
- 2.3.3 Generated versus user-editable files
- 2.3.4 Project config and setup directory layout
- 2.3.5 Root AGENTS navigation block
- 2.3.6 Lab: initialize a sandbox repository

### 2.4 Generating Host Integrations

Description: This module explains how Constructor Studio projects workflows into AI coding tools. Learners regenerate integrations and learn when regeneration is required.

#### Lessons and Checkpoints

- 2.4.1 What `cfs generate-agents` creates
- 2.4.2 Host integration directories
- 2.4.3 Slash commands, skills, prompts, and subagents
- 2.4.4 Regenerating after setup changes
- 2.4.5 Lab: generate integrations for one host

### 2.5 Activating Constructor Studio in Chat

Description: Learners activate the system from their AI coding tool and understand the difference between terminal commands and chat commands. This module establishes the core operating rule for the rest of the course.

#### Lessons and Checkpoints

- 2.5.1 Terminal: use `cfs`
- 2.5.2 Chat: use `/cf` and workflow commands
- 2.5.3 Activating Constructor Studio with `/cf on`
- 2.5.4 Confirming activation
- 2.5.5 Common activation failures
- 2.5.6 Lab: activate and run a first analysis prompt

### 2.6 First Five-Minute Trial

Description: Learners perform a small but meaningful first run without overloading the system. The goal is to experience planning or analysis before attempting generation.

#### Lessons and Checkpoints

- 2.6.1 Why first use should often be `/cf-analyze` or `/cf-plan`
- 2.6.2 First prompt patterns that work
- 2.6.3 Reading the response structure
- 2.6.4 Deciding the next action
- 2.6.5 Lab: run the first guided workflow

## 3. Operator Track - Daily Workflows

Description: This part teaches the core workflows an operator uses every day: plan, generate, analyze, validate, review, and iterate.

### 3.1 Workflow Selection

Description: Learners learn to choose the right workflow before asking the agent to act. The module emphasizes task shape, risk, context size, and expected output.

#### Lessons and Checkpoints

- 3.1.1 `/cf-plan` for large or risky work
- 3.1.2 `/cf-generate` for creating or changing artifacts and code
- 3.1.3 `/cf-analyze` for validation, review, and inspection
- 3.1.4 `/cf-studio` as the broader command surface
- 3.1.5 Kit-specific commands with `/cf-{kit}-{name}`
- 3.1.6 Checkpoint: choose a workflow for each scenario

### 3.2 Planning Work with `/cf-plan`

Description: This module teaches how to decompose work into phase files and checkpoints. Learners understand that planning produces execution artifacts rather than doing the underlying implementation.

#### Lessons and Checkpoints

- 3.2.1 When planning is mandatory
- 3.2.2 Plan scope, target, and input signature
- 3.2.3 Phase files and compilation briefs
- 3.2.4 Plan lifecycle choices
- 3.2.5 Execution readiness and validation
- 3.2.6 Lab: create a plan for a medium-risk change

### 3.3 Generating Artifacts with `/cf-generate`

Description: Learners create and update structured artifacts using templates, examples, rules, and confirmation gates. The module focuses on bounded generation rather than free-form writing.

#### Lessons and Checkpoints

- 3.3.1 Generation inputs and required context
- 3.3.2 Template-driven artifact writing
- 3.3.3 Example-guided style and quality
- 3.3.4 Confirming proposed inputs before writing
- 3.3.5 Post-write validation and review
- 3.3.6 Lab: generate a small artifact

### 3.4 Implementing Code from Approved Artifacts

Description: This module teaches how code changes are constrained by approved requirements, designs, or feature specs. Learners preserve traceability while making practical implementation changes.

#### Lessons and Checkpoints

- 3.4.1 Source artifact selection
- 3.4.2 Extracting implementation requirements
- 3.4.3 Proposed approach review
- 3.4.4 Traceability markers in code
- 3.4.5 Validation after implementation
- 3.4.6 Lab: implement a bounded feature from a spec

### 3.5 Analyzing Artifacts with `/cf-analyze`

Description: Learners validate artifacts through deterministic gates and semantic review. The module shows why a validator pass alone is not the same as a complete review.

#### Lessons and Checkpoints

- 3.5.1 Full analysis versus semantic-only analysis
- 3.5.2 File existence and registration checks
- 3.5.3 Deterministic validation gate
- 3.5.4 Semantic checklist review
- 3.5.5 Fix prompt and plan prompt outputs
- 3.5.6 Lab: analyze an artifact and triage findings

### 3.6 Reviewing Code and Implementation Behavior

Description: This module teaches code review through Constructor Studio's analysis model. Learners focus on defects, regressions, missing tests, and gaps against approved artifacts.

#### Lessons and Checkpoints

- 3.6.1 Code mode and design requirements
- 3.6.2 Bug-finding methodology
- 3.6.3 Missing or stale traceability markers
- 3.6.4 Review output severity and actionability
- 3.6.5 Lab: review a changed module against a feature

### 3.7 Validate-Review-Fix Loop

Description: Learners practice the standard loop: generate or implement, validate, review, fix, and validate again. This module makes iteration explicit instead of treating the first model output as done.

#### Lessons and Checkpoints

- 3.7.1 Why first-pass output is not final
- 3.7.2 Local validation before review
- 3.7.3 Separating generation and review contexts
- 3.7.4 Fixing deterministic failures
- 3.7.5 Fixing semantic findings
- 3.7.6 Lab: complete a full loop

### 3.8 Prompt Patterns for Operators

Description: This module gives learners practical prompt shapes for real work without turning the course into a prompt library. The focus is on bounded, reviewable requests.

#### Lessons and Checkpoints

- 3.8.1 Structured generation prompts
- 3.8.2 Structured analysis prompts
- 3.8.3 Planning prompts
- 3.8.4 Brownfield understanding prompts
- 3.8.5 Context-bounded execution prompts
- 3.8.6 Checkpoint: rewrite weak prompts

## 4. Artifacts, Traceability, and Validation

Description: This part goes deeper into the core evidence model: artifact registries, IDs, references, validation, and code traceability.

### 4.1 Artifact Registry Fundamentals

Description: Learners understand how Constructor Studio discovers and registers artifacts. This module explains systems, artifact kinds, paths, codebases, and ignore rules.

#### Lessons and Checkpoints

- 4.1.1 Purpose of the artifact registry
- 4.1.2 Systems and artifact kinds
- 4.1.3 Artifact paths and autodetect rules
- 4.1.4 Codebase entries and ignore patterns
- 4.1.5 Lab: inspect an artifact registry

### 4.2 Stable IDs

Description: This module teaches the role of stable identifiers in traceable delivery. Learners define, reference, query, and validate IDs.

#### Lessons and Checkpoints

- 4.2.1 ID purpose and lifecycle
- 4.2.2 ID kinds and naming conventions
- 4.2.3 Versioned IDs
- 4.2.4 Finding definitions with `cfs where-defined`
- 4.2.5 Finding usage with `cfs where-used`
- 4.2.6 Lab: trace an ID across documents

### 4.3 Cross-Artifact Links

Description: Learners connect requirements, design, decomposition, features, and implementation evidence. The module focuses on alignment and drift detection.

#### Lessons and Checkpoints

- 4.3.1 Outgoing references
- 4.3.2 Incoming references
- 4.3.3 Required links and coverage expectations
- 4.3.4 Broken links and orphaned IDs
- 4.3.5 Lab: repair a broken reference chain

### 4.4 Code Traceability

Description: This module connects artifacts to implementation through code markers and codebase scanning. Learners learn what traceability can show and what it cannot prove.

#### Lessons and Checkpoints

- 4.4.1 Code markers and implementation evidence
- 4.4.2 Marker naming policy
- 4.4.3 FULL versus DOCS-ONLY traceability
- 4.4.4 Marker recovery
- 4.4.5 Lab: add missing implementation markers

### 4.5 Deterministic Validation

Description: Learners run `cfs validate` and interpret results. The module explains exit codes, JSON output, and the difference between deterministic failure and semantic concern.

#### Lessons and Checkpoints

- 4.5.1 Validation scope
- 4.5.2 Exit codes and failure classes
- 4.5.3 JSON output and stderr messages
- 4.5.4 Local-only validation
- 4.5.5 CI validation basics
- 4.5.6 Lab: run and interpret validation

### 4.6 Validation Limits

Description: This module sets realistic expectations. Constructor Studio can expose missing, broken, or inconsistent evidence, but it does not prove business adequacy or implementation correctness.

#### Lessons and Checkpoints

- 4.6.1 What deterministic checks can prove
- 4.6.2 What semantic review must still cover
- 4.6.3 What human review must still decide
- 4.6.4 Avoiding false confidence
- 4.6.5 Checkpoint: classify validation claims

## 5. Advanced Operator Track - Brownfield, Workspaces, PRs, and Storytelling

Description: This part teaches advanced use in real teams: existing codebases, multi-repo workspaces, PR workflows, onboarding, and troubleshooting.

### 5.1 Brownfield Projects

Description: Learners use Constructor Studio in projects that already have code and inconsistent conventions. The module emphasizes understanding and auto-configuration before large edits.

#### Lessons and Checkpoints

- 5.1.1 Brownfield risks
- 5.1.2 Task-matched project rules
- 5.1.3 Auto-config purpose and outputs
- 5.1.4 Reviewing inferred rules
- 5.1.5 Lab: run a brownfield understanding pass

### 5.2 Large Task Handling

Description: This module teaches learners to avoid giant direct generation requests. They practice escalating to planning, chunking inputs, and keeping context boundaries healthy.

#### Lessons and Checkpoints

- 5.2.1 Context budget warnings
- 5.2.2 Raw input overflow
- 5.2.3 Phase boundaries and checkpoints
- 5.2.4 Resume after context loss
- 5.2.5 Lab: convert an oversized request into a plan

### 5.3 Multi-Repo Workspace Federation

Description: Learners connect multiple repositories into one reachable traceability surface. The module covers discovery, configuration, validation, and graceful degradation.

#### Lessons and Checkpoints

- 5.3.1 Workspace use cases
- 5.3.2 Source roles: artifacts, codebase, mixed, and support repos
- 5.3.3 Standalone versus inline workspace config
- 5.3.4 Cross-repo ID resolution
- 5.3.5 Missing source behavior
- 5.3.6 Lab: configure a two-repo workspace

### 5.4 Workspace Commands

Description: This module teaches the operational command set for workspaces. Learners inspect, add, sync, and validate workspace sources.

#### Lessons and Checkpoints

- 5.4.1 `cfs workspace-init`
- 5.4.2 `cfs workspace-add`
- 5.4.3 `cfs workspace-info`
- 5.4.4 `cfs workspace-sync`
- 5.4.5 Cross-repo `list-ids`, `where-defined`, and `where-used`
- 5.4.6 Lab: inspect cross-repo traceability

### 5.5 PR Review Workflows

Description: Learners run structured PR review and status workflows where supported by kits and GitHub tooling. The focus is review quality, checklists, unresolved comments, and status reporting.

#### Lessons and Checkpoints

- 5.5.1 PR review prerequisites
- 5.5.2 `/cf-sdlc-pr-review` as a kit workflow pattern
- 5.5.3 `/cf-sdlc-pr-status` as a kit workflow pattern
- 5.5.4 Review findings and severity
- 5.5.5 Resolved comment audit
- 5.5.6 Lab: produce a PR review report

### 5.6 Storytelling and Onboarding Workflows

Description: This module teaches the explain and onboarding modes for pedagogical walkthroughs. Learners use them to understand artifacts, PRs, and codebase conventions without turning analysis into a one-shot summary.

#### Lessons and Checkpoints

- 5.6.1 Storytelling intent and mode selection
- 5.6.2 Presentation mode
- 5.6.3 Review mode
- 5.6.4 Onboarding mode
- 5.6.5 Socratic and quiz mode
- 5.6.6 Explain package export
- 5.6.7 Lab: create an onboarding walkthrough

### 5.7 Host Tool Strategy

Description: Learners compare practical behavior across supported AI coding hosts. The module focuses on subagents, review isolation, model selection, and manual separation when host support is limited.

#### Lessons and Checkpoints

- 5.7.1 Claude Code strategy
- 5.7.2 Cursor strategy
- 5.7.3 GitHub Copilot strategy
- 5.7.4 OpenAI Codex strategy
- 5.7.5 Windsurf strategy
- 5.7.6 Checkpoint: choose a host strategy for a team

### 5.8 Troubleshooting and Recovery

Description: This module covers common setup, activation, validation, and workflow problems. Learners practice diagnosing issues without weakening the process.

#### Lessons and Checkpoints

- 5.8.1 CLI not found
- 5.8.2 Generated integrations not picked up
- 5.8.3 Wrong project root
- 5.8.4 Missing or stale AGENTS block
- 5.8.5 Validation failure triage
- 5.8.6 Plan recovery after interruption
- 5.8.7 Lab: diagnose a broken setup

## 6. Kit and Extension Author Track - Building the System Surface

Description: This part teaches maintainers how to extend Constructor Studio with kits, artifacts, rules, workflows, skills, subagents, and host integrations.

### 6.1 Kit Architecture

Description: Learners understand kits as domain-specific packages that extend the core platform. The module separates core responsibilities from kit responsibilities.

#### Lessons and Checkpoints

- 6.1.1 Core platform versus kits
- 6.1.2 Kit lifecycle: install, update, move, validate
- 6.1.3 Kit files and ownership
- 6.1.4 User-editable kit content
- 6.1.5 SDLC kit architecture
- 6.1.6 Checkpoint: identify core versus kit concerns

### 6.2 Kit Manifest and Resources

Description: This module teaches manifest-driven kit installation and resource binding. Learners see how relocatable kit resources are declared, copied, updated, and resolved.

#### Lessons and Checkpoints

- 6.2.1 Manifest purpose
- 6.2.2 Resource identifiers and default paths
- 6.2.3 User-modifiable resources
- 6.2.4 Resource binding in config
- 6.2.5 Existing kit resource transition
- 6.2.6 Lab: inspect a kit manifest

### 6.3 Artifact Kind Design

Description: Learners design an artifact kind with a template, rules, examples, and checklist. The module teaches how to make generation and analysis reliable.

#### Lessons and Checkpoints

- 6.3.1 Artifact kind purpose
- 6.3.2 Template structure
- 6.3.3 Example quality
- 6.3.4 Checklist scope
- 6.3.5 Rules and dependencies
- 6.3.6 Lab: draft an artifact kind package

### 6.4 Rules and Checklists

Description: This module goes deeper into the authoring rules that drive generation, analysis, and planning. Learners write rules that are specific enough for agents to follow and validators to support.

#### Lessons and Checkpoints

- 6.4.1 Generation-phase dependencies
- 6.4.2 Validation-phase dependencies
- 6.4.3 Mandatory versus optional checks
- 6.4.4 Interaction points and confirmation gates
- 6.4.5 Avoiding vague author instructions
- 6.4.6 Lab: strengthen a weak checklist

### 6.5 Workflow Authoring

Description: Learners create and maintain workflows that route user intent into reliable agent behavior. The module emphasizes navigation rules, fail-stop gates, and context hygiene.

#### Lessons and Checkpoints

- 6.5.1 Workflow purpose and frontmatter
- 6.5.2 ALWAYS open and follow rules
- 6.5.3 WHEN conditions
- 6.5.4 Phase structure and gates
- 6.5.5 Output contracts
- 6.5.6 Lab: design a small kit workflow

### 6.6 Skill Authoring

Description: This module teaches skills as host-visible entry points that route into workflows and methods. Learners write concise skill descriptions that trigger correctly.

#### Lessons and Checkpoints

- 6.6.1 Skill role in Constructor Studio
- 6.6.2 `SKILL.md` structure
- 6.6.3 Description quality and trigger behavior
- 6.6.4 Generated versus hand-maintained skills
- 6.6.5 Lab: write a skill entry point

### 6.7 Command Naming for Kits

Description: Learners apply the Constructor Studio command naming model to kit workflows. The module standardizes names such as `/cf-{kit}-{name}` and teaches how to keep command sets clear.

#### Lessons and Checkpoints

- 6.7.1 Core command namespace
- 6.7.2 Kit command namespace
- 6.7.3 Naming collisions and reserved names
- 6.7.4 Host-specific aliases
- 6.7.5 Lab: name a kit command set

### 6.8 Subagents and Delegation

Description: This module teaches when and how specialized agents support planning, phase compilation, phase execution, PR review, and large change orchestration. Learners understand host support differences and fallback behavior.

#### Lessons and Checkpoints

- 6.8.1 Subagent responsibilities
- 6.8.2 Phase compiler agent
- 6.8.3 Phase runner agent
- 6.8.4 PR review agent
- 6.8.5 Delegation and RalphEx-style orchestration
- 6.8.6 Lab: design a subagent role

### 6.9 Project-Level Extensibility

Description: Learners extend behavior inside a single project without changing the core platform. This module covers local rules, workflows, commands, and host-specific generated surfaces.

#### Lessons and Checkpoints

- 6.9.1 Project rules
- 6.9.2 Project specs
- 6.9.3 Local workflows and commands
- 6.9.4 Generated host integrations
- 6.9.5 Governance for local extensions
- 6.9.6 Lab: add a project-specific rule

### 6.10 Testing and Validating Extensions

Description: This module teaches authors to validate extension behavior before publishing or rolling it into team use. Learners combine deterministic checks, semantic reviews, and fixture projects.

#### Lessons and Checkpoints

- 6.10.1 Structural validation for kits
- 6.10.2 Fixture projects
- 6.10.3 Prompt and workflow reviews
- 6.10.4 Regression tests for generated surfaces
- 6.10.5 Release checklist for kit changes
- 6.10.6 Lab: validate a custom kit slice

## 7. Governance, CI, and Team Adoption

Description: This part teaches teams how to adopt Constructor Studio without turning it into bureaucracy. The focus is practical governance, CI, review expectations, and maintainable operating habits.

### 7.1 Team Operating Model

Description: Learners define how Constructor Studio fits into team delivery. The module covers ownership, review gates, conventions, and what should be enforced versus documented.

#### Lessons and Checkpoints

- 7.1.1 Who owns artifacts
- 7.1.2 Who owns rules and kits
- 7.1.3 When plans are required
- 7.1.4 When validation is required
- 7.1.5 Human approval boundaries
- 7.1.6 Checkpoint: draft a team operating policy

### 7.2 CI Integration

Description: This module teaches how deterministic checks move from local development into CI. Learners understand which commands belong in CI and how to treat failures.

#### Lessons and Checkpoints

- 7.2.1 Local checks before PR
- 7.2.2 `cfs validate` in CI
- 7.2.3 Local-only versus workspace validation
- 7.2.4 Exit code handling
- 7.2.5 Reporting validation results
- 7.2.6 Lab: design a CI validation gate

### 7.3 Review Readiness

Description: Learners prepare changes so reviewers can see scope, intent, evidence, validation, and remaining risk. The module turns Constructor Studio outputs into a review package.

#### Lessons and Checkpoints

- 7.3.1 What reviewers need
- 7.3.2 Evidence chain summary
- 7.3.3 Validation result summary
- 7.3.4 Known risks and open questions
- 7.3.5 PR review handoff
- 7.3.6 Lab: assemble a review-ready change summary

### 7.4 Version and Update Management

Description: This module teaches how teams update the CLI, project-installed core, generated integrations, and kits. Learners handle version notices, diffs, and schema changes.

#### Lessons and Checkpoints

- 7.4.1 Global cache and project-installed core
- 7.4.2 Version notices
- 7.4.3 `cfs update`
- 7.4.4 Kit update diffs
- 7.4.5 Regenerating integrations after update
- 7.4.6 Lab: plan a safe update

### 7.5 Adoption Patterns and Anti-Patterns

Description: This module helps teams avoid both underuse and overuse. Learners identify where Constructor Studio adds value and where it becomes unnecessary overhead.

#### Lessons and Checkpoints

- 7.5.1 Good first team use cases
- 7.5.2 Bad first team use cases
- 7.5.3 Avoiding giant prompt culture
- 7.5.4 Avoiding false proof claims
- 7.5.5 Keeping artifacts alive
- 7.5.6 Checkpoint: adoption scenario review

## 8. Capstone and Certification

Description: This part turns the course into an end-to-end proof of skill. Learners complete a realistic delivery scenario and produce artifacts, plans, implementation evidence, validation output, review notes, and an extension slice.

### 8.1 Capstone Scenario

Description: Learners receive a realistic brownfield or multi-repo change request. The scenario requires both operator skills and, for advanced certification, a small extension or kit workflow.

#### Lessons and Checkpoints

- 8.1.1 Scenario brief
- 8.1.2 Repository setup
- 8.1.3 Success criteria
- 8.1.4 Constraints and allowed shortcuts
- 8.1.5 Checkpoint: capstone readiness review

### 8.2 Operator Capstone Path

Description: The operator path proves daily use competence. Learners initialize or inspect setup, choose workflows, produce or update artifacts, plan the change, implement, validate, analyze, and prepare review evidence.

#### Lessons and Checkpoints

- 8.2.1 Environment and setup evidence
- 8.2.2 Workflow selection rationale
- 8.2.3 Artifact generation or update
- 8.2.4 Execution plan
- 8.2.5 Implementation with traceability
- 8.2.6 Validation and review loop
- 8.2.7 Final review package

### 8.3 Author Capstone Path

Description: The author path adds an extension requirement on top of operator competence. Learners design a small kit artifact kind, workflow, skill, or project-level rule and validate that it works.

#### Lessons and Checkpoints

- 8.3.1 Extension concept
- 8.3.2 Artifact kind or workflow design
- 8.3.3 Skill or command entry point
- 8.3.4 Generated host integration expectation
- 8.3.5 Extension validation
- 8.3.6 Final authoring review

### 8.4 Certification Review

Description: This module defines the evaluation rubric and evidence package. Learners are assessed on correctness, traceability, workflow choice, validation discipline, and clarity of handoff.

#### Lessons and Checkpoints

- 8.4.1 Operator rubric
- 8.4.2 Author rubric
- 8.4.3 Required evidence files
- 8.4.4 Common failure modes
- 8.4.5 Remediation path
- 8.4.6 Final certification checklist

## Appendix A. Command and Terminology Reference

Description: This appendix collects the Constructor Studio names used throughout the course. It is a quick reference for product terms, terminal commands, chat commands, and kit command naming.

### A.1 Product and CLI Names

Description: This mapping covers product and terminal interface naming.

#### Reference

- Product name: Constructor Studio
- CLI: `cfs`
- Project setup directory: `.cf-studio/`
- Root chat command or skill: `/cf`
- Studio command surface: `/cf-studio`

### A.2 Chat and Workflow Names

Description: This mapping covers AI coding tool commands and skills.

#### Reference

- Root command or skill: `/cf`
- Studio surface: `/cf-studio`
- Plan workflow: `/cf-plan`
- Generate workflow: `/cf-generate`
- Analyze workflow: `/cf-analyze`
- Kit workflow pattern: `/cf-{kit}-{name}`

### A.3 Course Writing Rules

Description: These rules keep lesson text consistent and prevent mixed terminology from confusing new learners.

#### Rules

- Use Constructor Studio as the primary product name.
- Use `cfs` for terminal examples.
- Use `/cf-*` for chat commands.
- Use `/cf-{kit}-{name}` for kit workflow examples.
- Keep internal implementation names out of learner-facing lesson titles.

## Appendix B. Learner Journey Map

Description: This appendix summarizes recommended completion paths for different learners.

### B.1 New Operator Path

Description: This path is for developers, technical leads, and product-minded engineers who want to use Constructor Studio in daily project work.

#### Recommended Sequence

- Complete Part 0: Course Frame
- Complete Part 1: Foundation
- Complete Part 2: Getting Started
- Complete Part 3: Operator Track
- Complete Part 4: Artifacts, Traceability, and Validation
- Complete Part 5 modules 5.1 through 5.8 as needed
- Complete Part 7 modules 7.1 through 7.5
- Complete Part 8.2 Operator Capstone Path

### B.2 Kit and Extension Author Path

Description: This path is for maintainers who design kits, workflows, skills, and project extensions. It assumes the learner has completed the operator foundations first.

#### Recommended Sequence

- Complete all New Operator Path modules
- Complete Part 6: Kit and Extension Author Track
- Complete Part 8.3 Author Capstone Path
- Complete Part 8.4 Certification Review

### B.3 Team Adoption Path

Description: This path is for technical leads planning rollout across a team or workspace. It prioritizes operating model, validation, review readiness, and adoption discipline.

#### Recommended Sequence

- Complete Part 1: Foundation
- Complete Part 2: Getting Started
- Complete Part 3 modules 3.1, 3.2, 3.5, and 3.7
- Complete Part 4 modules 4.1 through 4.6
- Complete Part 5 modules 5.3, 5.4, 5.5, and 5.8
- Complete Part 7: Governance, CI, and Team Adoption
- Review Part 8 certification rubric for internal enablement