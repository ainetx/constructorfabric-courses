# Constructor Studio Academy - Course Blueprint and Table of Contents

> NOTE: These course materials are a draft, generated from the following source repositories:
> - https://github.com/cyberfabric/cyber-constructor (to be renamed `constructor-studio`)
> - https://github.com/cyberfabric/cyber-constructor-kit-sdlc (to be renamed `constructor-studio-kit-sdlc`)

## 1. Course Frame

Description: This course teaches Constructor Studio from first principles through advanced operation and extension authoring. It uses the established Constructor Studio terminology throughout the learner-facing material.

### 1.1 Audience and Tracks

Description: The course has one shared foundation, then separates into an Operator track and a Kit and Extension Author track. Learners can complete the Operator track alone or continue into authoring and certification work.

#### Lessons and Checkpoints

- 1.1.1 Who the course is for
- 1.1.2 Operator path: using Constructor Studio in real projects
- 1.1.3 Author path: building kits, workflows, skills, and extensions
- 1.1.4 Recommended paths by role
- 1.1.5 Checkpoint: choose your learner path

### 1.2 Command and Terminology Standard

Description: All lessons use the standard Constructor Studio terms and tools: Constructor Studio, `cfs`, `/cf`, `/cf-studio`, and `/cf-*`. Learners practice the command vocabulary they will use in real projects.

#### Lessons and Checkpoints

- 1.2.1 Product name: Constructor Studio
- 1.2.2 CLI name: `cfs`
- 1.2.3 Root skill and activation: `/cf`
- 1.2.4 Studio command surface: `/cf-studio`
- 1.2.5 Core workflow commands: `/cf-plan`, `/cf-generate`, `/cf-analyze`
- 1.2.6 Kit workflow commands: `/cf-{kit}-{name}`
- 1.2.7 Naming practice: choosing the right command form

### 1.3 Course Project and Assessment Model

Description: The course uses one running repository project so each concept becomes a practical artifact, command, or workflow result. Assessments emphasize repeatable operation, traceability, validation, and review readiness.

#### Lessons and Checkpoints

- 1.3.1 The running course repository
- 1.3.2 What learners will build
- 1.3.3 Labs, checkpoints, and capstone rules
- 1.3.4 Evidence required for completion
- 1.3.5 Certification rubric overview

## 2. Foundation - Mental Model and Operating Principles

Description: This part explains what Constructor Studio is, where it fits around AI coding tools, and why the system uses artifacts, workflows, validation, and traceability instead of one long prompt.

### 2.1 What Constructor Studio Is

Description: Learners build a simple mental model: Constructor Studio is the workflow, context, and validation layer around an AI coding tool. It helps teams keep requirements, design, plans, and code aligned.

#### Lessons and Checkpoints

- 2.1.1 The core problem: AI work without durable control surfaces
- 2.1.2 Constructor Studio as a repo-attached Spec Driven Development system
- 2.1.3 Inspectable artifacts versus chat memory
- 2.1.4 Deterministic checks versus model reasoning
- 2.1.5 Checkpoint: explain the system in one paragraph

### 2.2 Actors and Responsibilities

Description: This module separates the responsibilities of the human, AI coding tool, agent, Constructor Studio, CLI, and CI pipeline. The goal is to prevent learners from treating the system as either magic automation or just documentation.

#### Lessons and Checkpoints

- 2.2.1 Human owner and approval authority
- 2.2.2 AI coding tool as the host environment
- 2.2.3 Agent as the reasoning and writing executor
- 2.2.4 Constructor Studio as workflow and validation control
- 2.2.5 `cfs` as deterministic local and CI interface
- 2.2.6 Checkpoint: assign responsibilities for a change request

### 2.3 The Artifact-First Delivery Model

Description: Learners see how requirements, design, decomposition, features, plans, implementation, and review outputs form a delivery chain. This module introduces stable IDs and links without going deep into validation internals yet.

#### Lessons and Checkpoints

- 2.3.1 Why artifacts exist
- 2.3.2 Requirement to design to plan to code
- 2.3.3 Stable identifiers and references
- 2.3.4 Drift as a visible signal
- 2.3.5 Lab: read a simple evidence chain

### 2.4 Fit and Non-Fit

Description: This module teaches when Constructor Studio is worth the overhead and when a normal edit is better. Learners practice choosing based on risk, ambiguity, review pressure, and traceability needs.

#### Lessons and Checkpoints

- 2.4.1 Good fit: risky, multi-step, review-sensitive work
- 2.4.2 Good fit: brownfield understanding before editing
- 2.4.3 Non-fit: tiny edits and throwaway spikes
- 2.4.4 Tradeoff: more structure for more control
- 2.4.5 Checkpoint: classify ten work requests

### 2.5 Core Vocabulary

Description: This module establishes the language used across the rest of the course. Terms are defined as the normal Constructor Studio vocabulary learners will use in daily work.

#### Lessons and Checkpoints

- 2.5.1 Project, setup directory, and Studio installation
- 2.5.2 Artifacts, systems, codebases, and registries
- 2.5.3 Workflows, skills, commands, and generated integrations
- 2.5.4 Kits, templates, rules, checklists, and examples
- 2.5.5 Workspace sources and cross-repo resolution
- 2.5.6 Language complexity setting and output language control
- 2.5.7 Checkpoint: vocabulary matching exercise

## 3. Getting Started - Installation, Setup, and First Use

Description: This part takes a new learner from no installed tool to a working repository with generated agent integrations and a first useful workflow run.

### 3.1 Local Prerequisites

Description: Learners prepare the development environment required for Constructor Studio. The module keeps the setup practical and focuses only on what is needed to run the system.

#### Lessons and Checkpoints

- 3.1.1 Required tools: Python, Git, `pipx`, and AI coding host
- 3.1.2 Optional tools: GitHub CLI for PR workflows
- 3.1.3 Supported hosts and practical differences
- 3.1.4 Environment checks before installation
- 3.1.5 Running `cfs doctor` to verify environment health
- 3.1.6 Lab: verify prerequisites

### 3.2 Installing the CLI

Description: This module introduces `cfs` as the Constructor Studio CLI. Learners verify installation before touching a project.

#### Lessons and Checkpoints

- 3.2.1 Installing `cfs`
- 3.2.2 Verifying the installed executable
- 3.2.3 Checking CLI version
- 3.2.4 Understanding global proxy behavior
- 3.2.5 Troubleshooting PATH issues
- 3.2.6 Lab: install and verify the CLI

### 3.3 Initializing a Repository

Description: Learners initialize Constructor Studio in a repository and inspect the generated surfaces. The focus is on what gets created, what is generated, and what the user owns.

#### Lessons and Checkpoints

- 3.3.1 Running `cfs init`
- 3.3.2 Choosing the setup directory
- 3.3.3 Generated versus user-editable files
- 3.3.4 Project config and setup directory layout
- 3.3.5 Root AGENTS navigation block
- 3.3.6 Lab: initialize a sandbox repository

### 3.4 Generating Host Integrations

Description: This module explains how Constructor Studio projects workflows into AI coding tools. Learners regenerate integrations and learn when regeneration is required.

#### Lessons and Checkpoints

- 3.4.1 What `cfs generate-agents` creates
- 3.4.2 Host integration directories
- 3.4.3 Slash commands, skills, prompts, and subagents
- 3.4.4 Regenerating after setup changes
- 3.4.5 Lab: generate integrations for one host

### 3.5 Activating Constructor Studio in Chat

Description: Learners activate the system from their AI coding tool and understand the difference between terminal commands and chat commands. This module establishes the core operating rule for the rest of the course.

#### Lessons and Checkpoints

- 3.5.1 Terminal: use `cfs`
- 3.5.2 Chat: use `/cf` and workflow commands
- 3.5.3 Activating Constructor Studio with `/cf on`
- 3.5.4 Confirming activation
- 3.5.5 Common activation failures
- 3.5.6 Lab: activate and run a first analysis prompt

### 3.6 First Five-Minute Trial

Description: Learners perform a small but meaningful first run without overloading the system. The goal is to experience planning or analysis before attempting generation.

#### Lessons and Checkpoints

- 3.6.1 Why first use should often be `/cf-analyze` or `/cf-plan`
- 3.6.2 First prompt patterns that work
- 3.6.3 Reading the response structure
- 3.6.4 Deciding the next action
- 3.6.5 Lab: run the first guided workflow

## 4. Operator Track - Daily Workflows

Description: This part teaches the core workflows an operator uses every day: plan, generate, analyze, validate, review, and iterate.

### 4.1 Workflow Selection

Description: Learners learn to choose the right workflow before asking the agent to act. The module emphasizes task shape, risk, context size, and expected output.

#### Lessons and Checkpoints

- 4.1.1 `/cf-plan` for large or risky work
- 4.1.2 `/cf-generate` for creating or changing artifacts and code
- 4.1.3 `/cf-analyze` for validation, review, and inspection
- 4.1.4 `/cf-studio` as the broader command surface
- 4.1.5 Kit-specific commands with `/cf-{kit}-{name}`
- 4.1.6 Checkpoint: choose a workflow for each scenario

### 4.2 Planning Work with `/cf-plan`

Description: This module teaches how to decompose work into phase files and checkpoints. Learners understand that planning produces execution artifacts rather than doing the underlying implementation.

#### Lessons and Checkpoints

- 4.2.1 When planning is mandatory
- 4.2.2 Plan scope, target, and input signature
- 4.2.3 Phase files and compilation briefs
- 4.2.4 Plan lifecycle choices
- 4.2.5 Execution readiness and validation
- 4.2.6 Lab: create a plan for a medium-risk change

### 4.3 Generating Artifacts with `/cf-generate`

Description: Learners create and update structured artifacts using templates, examples, rules, and confirmation gates. The module focuses on bounded generation rather than free-form writing.

#### Lessons and Checkpoints

- 4.3.1 Generation inputs and required context
- 4.3.2 Template-driven artifact writing
- 4.3.3 Example-guided style and quality
- 4.3.4 Confirming proposed inputs before writing
- 4.3.5 Post-write validation and review
- 4.3.6 Lab: generate a small artifact

### 4.4 Implementing Code from Approved Artifacts

Description: This module teaches how code changes are constrained by approved requirements, designs, or feature specs. Learners preserve traceability while making practical implementation changes.

#### Lessons and Checkpoints

- 4.4.1 Source artifact selection
- 4.4.2 Extracting implementation requirements
- 4.4.3 Proposed approach review
- 4.4.4 Traceability markers in code
- 4.4.5 Validation after implementation
- 4.4.6 Lab: implement a bounded feature from a spec

### 4.5 Analyzing Artifacts with `/cf-analyze`

Description: Learners validate artifacts through deterministic gates and semantic review. The module shows why a validator pass alone is not the same as a complete review.

#### Lessons and Checkpoints

- 4.5.1 Full analysis versus semantic-only analysis
- 4.5.2 File existence and registration checks
- 4.5.3 Deterministic validation gate
- 4.5.4 Semantic checklist review
- 4.5.5 Fix prompt and plan prompt outputs
- 4.5.6 Lab: analyze an artifact and triage findings

### 4.6 Reviewing Code and Implementation Behavior

Description: This module teaches code review through Constructor Studio's analysis model. Learners focus on defects, regressions, missing tests, and gaps against approved artifacts.

#### Lessons and Checkpoints

- 4.6.1 Code mode and design requirements
- 4.6.2 Bug-finding methodology
- 4.6.3 Missing or stale traceability markers
- 4.6.4 Review output severity and actionability
- 4.6.5 Lab: review a changed module against a feature

### 4.7 Validate-Review-Fix Loop

Description: Learners practice the standard loop: generate or implement, validate, review, fix, and validate again. This module makes iteration explicit instead of treating the first model output as done.

#### Lessons and Checkpoints

- 4.7.1 Why first-pass output is not final
- 4.7.2 Local validation before review
- 4.7.3 Separating generation and review contexts
- 4.7.4 Fixing deterministic failures
- 4.7.5 Fixing semantic findings
- 4.7.6 Lab: complete a full loop

### 4.8 Prompt Patterns for Operators

Description: This module gives learners practical prompt shapes for real work without turning the course into a prompt library. The focus is on bounded, reviewable requests.

#### Lessons and Checkpoints

- 4.8.1 Structured generation prompts
- 4.8.2 Structured analysis prompts
- 4.8.3 Planning prompts
- 4.8.4 Brownfield understanding prompts
- 4.8.5 Context-bounded execution prompts
- 4.8.6 Checkpoint: rewrite weak prompts

### 4.9 How Constructor Studio Routes Workflows

Description: This module explains the Protocol Guard and execution protocol that determines which files the agent loads, how variables are resolved, and why specific rules and specs are matched for each request. Understanding this mechanism helps operators debug routing issues and predict agent behavior.

#### Lessons and Checkpoints

- 4.9.1 Protocol Guard purpose and load sequence
- 4.9.2 Variable resolution with `cfs info`
- 4.9.3 Registry understanding and target determination
- 4.9.4 WHEN-clause spec matching
- 4.9.5 Navigation rules: ALWAYS open, OPEN and follow
- 4.9.6 Debugging routing problems
- 4.9.7 Lab: trace how a workflow request is routed

## 5. Artifacts, Traceability, and Validation

Description: This part goes deeper into the core evidence model: artifact registries, IDs, references, validation, and code traceability.

### 5.1 Artifact Registry Fundamentals

Description: Learners understand how Constructor Studio discovers and registers artifacts. This module explains systems, artifact kinds, paths, codebases, and ignore rules.

#### Lessons and Checkpoints

- 5.1.1 Purpose of the artifact registry
- 5.1.2 Systems and artifact kinds
- 5.1.3 Artifact paths and autodetect rules
- 5.1.4 Codebase entries and ignore patterns
- 5.1.5 Lab: inspect an artifact registry

### 5.2 Stable IDs

Description: This module teaches the role of stable identifiers in traceable delivery. Learners define, reference, query, and validate IDs.

#### Lessons and Checkpoints

- 5.2.1 ID purpose and lifecycle
- 5.2.2 ID kinds and naming conventions
- 5.2.3 Versioned IDs
- 5.2.4 Finding definitions with `cfs where-defined`
- 5.2.5 Finding usage with `cfs where-used`
- 5.2.6 Lab: trace an ID across documents

### 5.3 Cross-Artifact Links

Description: Learners connect requirements, design, decomposition, features, and implementation evidence. The module focuses on alignment and drift detection.

#### Lessons and Checkpoints

- 5.3.1 Outgoing references
- 5.3.2 Incoming references
- 5.3.3 Required links and coverage expectations
- 5.3.4 Broken links and orphaned IDs
- 5.3.5 Lab: repair a broken reference chain

### 5.4 Code Traceability

Description: This module connects artifacts to implementation through code markers and codebase scanning. Learners learn what traceability can show and what it cannot prove.

#### Lessons and Checkpoints

- 5.4.1 Code markers and implementation evidence
- 5.4.2 Marker naming policy
- 5.4.3 FULL versus DOCS-ONLY traceability
- 5.4.4 Marker recovery
- 5.4.5 Lab: add missing implementation markers

### 5.5 Deterministic Validation

Description: Learners run `cfs validate` and interpret results. The module explains exit codes, JSON output, and the difference between deterministic failure and semantic concern.

#### Lessons and Checkpoints

- 5.5.1 Validation scope
- 5.5.2 Exit codes and failure classes
- 5.5.3 JSON output and stderr messages
- 5.5.4 Local-only validation
- 5.5.5 CI validation basics
- 5.5.6 Lab: run and interpret validation

### 5.6 Validation Limits

Description: This module sets realistic expectations. Constructor Studio can expose missing, broken, or inconsistent evidence, but it does not prove business adequacy or implementation correctness.

#### Lessons and Checkpoints

- 5.6.1 What deterministic checks can prove
- 5.6.2 What semantic review must still cover
- 5.6.3 What human review must still decide
- 5.6.4 Avoiding false confidence
- 5.6.5 Checkpoint: classify validation claims

## 6. Advanced Operator Track - Brownfield, Workspaces, PRs, and Storytelling

Description: This part teaches advanced use in real teams: existing codebases, multi-repo workspaces, PR workflows, onboarding, and troubleshooting.

### 6.1 Brownfield Projects

Description: Learners use Constructor Studio in projects that already have code and inconsistent conventions. The module emphasizes understanding and auto-configuration before large edits.

#### Lessons and Checkpoints

- 6.1.1 Brownfield risks
- 6.1.2 Task-matched project rules
- 6.1.3 Auto-config purpose and outputs
- 6.1.4 When the agent offers auto-config: the brownfield detection gate
- 6.1.5 Reviewing and refining inferred rules
- 6.1.6 Re-running auto-config after project evolution
- 6.1.7 Lab: run auto-config and review inferred project rules

### 6.2 Large Task Handling

Description: This module teaches learners to avoid giant direct generation requests. They practice escalating to planning, chunking inputs, and keeping context boundaries healthy.

#### Lessons and Checkpoints

- 6.2.1 Context budget warnings
- 6.2.2 Raw input overflow
- 6.2.3 Phase boundaries and checkpoints
- 6.2.4 Resume after context loss
- 6.2.5 Lab: convert an oversized request into a plan

### 6.3 Multi-Repo Workspace Federation

Description: Learners connect multiple repositories into one reachable traceability surface. The module covers discovery, configuration, validation, and graceful degradation.

#### Lessons and Checkpoints

- 6.3.1 Workspace use cases
- 6.3.2 Source roles: artifacts, codebase, mixed, and support repos
- 6.3.3 Standalone versus inline workspace config
- 6.3.4 Cross-repo ID resolution
- 6.3.5 Missing source behavior
- 6.3.6 Lab: configure a two-repo workspace

### 6.4 Workspace Commands

Description: This module teaches the operational command set for workspaces. Learners inspect, add, sync, and validate workspace sources.

#### Lessons and Checkpoints

- 6.4.1 `cfs workspace-init`
- 6.4.2 `cfs workspace-add`
- 6.4.3 `cfs workspace-info`
- 6.4.4 `cfs workspace-sync`
- 6.4.5 Cross-repo `list-ids`, `where-defined`, and `where-used`
- 6.4.6 Lab: inspect cross-repo traceability

### 6.5 PR Review Workflows

Description: Learners run structured PR review and status workflows where supported by kits and GitHub tooling. The focus is review quality, checklists, unresolved comments, and status reporting.

#### Lessons and Checkpoints

- 6.5.1 PR review prerequisites
- 6.5.2 `/cf-sdlc-pr-review` as a kit workflow pattern
- 6.5.3 `/cf-sdlc-pr-status` as a kit workflow pattern
- 6.5.4 Review findings and severity
- 6.5.5 Resolved comment audit
- 6.5.6 Lab: produce a PR review report

### 6.6 Storytelling and Onboarding Workflows

Description: This module teaches the explain and onboarding modes for pedagogical walkthroughs. Learners use them to understand artifacts, PRs, and codebase conventions without turning analysis into a one-shot summary.

#### Lessons and Checkpoints

- 6.6.1 Storytelling intent and mode selection
- 6.6.2 Presentation mode
- 6.6.3 Review mode
- 6.6.4 Onboarding mode
- 6.6.5 Socratic and quiz mode
- 6.6.6 Explain package export
- 6.6.7 Lab: create an onboarding walkthrough

### 6.7 Host Tool Strategy

Description: Learners compare practical behavior across supported AI coding hosts. The module focuses on subagents, review isolation, model selection, and manual separation when host support is limited.

#### Lessons and Checkpoints

- 6.7.1 Claude Code strategy
- 6.7.2 Cursor strategy
- 6.7.3 GitHub Copilot strategy
- 6.7.4 OpenAI Codex strategy
- 6.7.5 Windsurf strategy
- 6.7.6 Checkpoint: choose a host strategy for a team

### 6.8 Troubleshooting and Recovery

Description: This module covers common setup, activation, validation, and workflow problems. Learners practice diagnosing issues without weakening the process.

#### Lessons and Checkpoints

- 6.8.1 CLI not found
- 6.8.2 Generated integrations not picked up
- 6.8.3 Wrong project root
- 6.8.4 Missing or stale AGENTS block
- 6.8.5 Validation failure triage
- 6.8.6 Plan recovery after interruption
- 6.8.7 Using `cfs doctor` for environment diagnosis
- 6.8.8 Lab: diagnose a broken setup

## 7. Kit and Extension Author Track - Building the System Surface

Description: This part teaches maintainers how to extend Constructor Studio with kits, artifacts, rules, workflows, skills, subagents, and host integrations.

### 7.1 Kit Architecture

Description: Learners understand kits as domain-specific packages that extend the core platform. The module separates core responsibilities from kit responsibilities.

#### Lessons and Checkpoints

- 7.1.1 Core platform versus kits
- 7.1.2 Kit lifecycle: install, update, move, validate
- 7.1.3 Kit files and ownership
- 7.1.4 User-editable kit content
- 7.1.5 SDLC kit architecture
- 7.1.6 Checkpoint: identify core versus kit concerns

### 7.2 Kit Manifest and Resources

Description: This module teaches manifest-driven kit installation and resource binding. Learners see how relocatable kit resources are declared, copied, updated, and resolved.

#### Lessons and Checkpoints

- 7.2.1 Manifest purpose
- 7.2.2 Resource identifiers and default paths
- 7.2.3 User-modifiable resources
- 7.2.4 Resource binding in config
- 7.2.5 Existing kit resource transition
- 7.2.6 Lab: inspect a kit manifest

### 7.3 Artifact Kind Design

Description: Learners design an artifact kind with a template, rules, examples, and checklist. The module teaches how to make generation and analysis reliable.

#### Lessons and Checkpoints

- 7.3.1 Artifact kind purpose
- 7.3.2 Template structure
- 7.3.3 Example quality
- 7.3.4 Checklist scope
- 7.3.5 Rules and dependencies
- 7.3.6 Lab: draft an artifact kind package

### 7.4 Rules and Checklists

Description: This module goes deeper into the authoring rules that drive generation, analysis, and planning. Learners write rules that are specific enough for agents to follow and validators to support.

#### Lessons and Checkpoints

- 7.4.1 Generation-phase dependencies
- 7.4.2 Validation-phase dependencies
- 7.4.3 Mandatory versus optional checks
- 7.4.4 Interaction points and confirmation gates
- 7.4.5 Avoiding vague author instructions
- 7.4.6 Lab: strengthen a weak checklist

### 7.5 Behavior Description Language (CDSL)

Description: This module teaches the Cypilot DSL (CDSL) used for writing algorithms, actor flows, and state machines in DESIGN and FEATURE artifacts. CDSL is a plain-English behavior description language with structured control flow keywords, mandatory phase tokens, instruction IDs, and implementation checkboxes.

#### Lessons and Checkpoints

- 7.5.1 CDSL purpose and when to use it
- 7.5.2 Basic format: numbered lists, bold keywords, plain English
- 7.5.3 Control flow keywords: IF, FOR EACH, WHILE, TRY/CATCH, PARALLEL, MATCH
- 7.5.4 Phase tokens, instruction IDs, and implementation checkboxes
- 7.5.5 State machines in CDSL
- 7.5.6 Validation rules: required and prohibited patterns
- 7.5.7 Lab: write a behavior specification in CDSL

### 7.6 Workflow Authoring

Description: Learners create and maintain workflows that route user intent into reliable agent behavior. The module emphasizes navigation rules, fail-stop gates, and context hygiene.

#### Lessons and Checkpoints

- 7.6.1 Workflow purpose and frontmatter
- 7.6.2 ALWAYS open and follow rules
- 7.6.3 WHEN conditions
- 7.6.4 Phase structure and gates
- 7.6.5 Output contracts
- 7.6.6 Lab: design a small kit workflow

### 7.7 Skill Authoring

Description: This module teaches skills as host-visible entry points that route into workflows and methods. Learners write concise skill descriptions that trigger correctly.

#### Lessons and Checkpoints

- 7.7.1 Skill role in Constructor Studio
- 7.7.2 `SKILL.md` structure
- 7.7.3 Description quality and trigger behavior
- 7.7.4 Generated versus hand-maintained skills
- 7.7.5 Lab: write a skill entry point

### 7.8 Command Naming for Kits

Description: Learners apply the Constructor Studio command naming model to kit workflows. The module standardizes names such as `/cf-{kit}-{name}` and teaches how to keep command sets clear.

#### Lessons and Checkpoints

- 7.8.1 Core command namespace
- 7.8.2 Kit command namespace
- 7.8.3 Naming collisions and reserved names
- 7.8.4 Host-specific aliases
- 7.8.5 Lab: name a kit command set

### 7.9 Subagents and Delegation

Description: This module teaches when and how specialized agents support planning, phase compilation, phase execution, PR review, and large change orchestration. Learners understand host support differences and fallback behavior.

#### Lessons and Checkpoints

- 7.9.1 Subagent responsibilities
- 7.9.2 Phase compiler agent
- 7.9.3 Phase runner agent
- 7.9.4 PR review agent
- 7.9.5 Delegation and RalphEx-style orchestration
- 7.9.6 Lab: design a subagent role

### 7.10 Project-Level Extensibility

Description: Learners extend behavior inside a single project without changing the core platform. This module covers local rules, workflows, commands, and host-specific generated surfaces.

#### Lessons and Checkpoints

- 7.10.1 Project rules
- 7.10.2 Project specs
- 7.10.3 Local workflows and commands
- 7.10.4 Generated host integrations
- 7.10.5 Governance for local extensions
- 7.10.6 Lab: add a project-specific rule

### 7.11 Testing and Validating Extensions

Description: This module teaches authors to validate extension behavior before publishing or rolling it into team use. Learners combine deterministic checks, semantic reviews, and fixture projects.

#### Lessons and Checkpoints

- 7.11.1 Structural validation for kits
- 7.11.2 Using `cfs self-check` to validate kit examples against templates
- 7.11.3 Fixture projects
- 7.11.4 Prompt and workflow reviews
- 7.11.5 Regression tests for generated surfaces
- 7.11.6 Release checklist for kit changes
- 7.11.7 Lab: validate a custom kit slice

## 8. Governance, CI, and Team Adoption

Description: This part teaches teams how to adopt Constructor Studio without turning it into bureaucracy. The focus is practical governance, CI, review expectations, and maintainable operating habits.

### 8.1 Team Operating Model

Description: Learners define how Constructor Studio fits into team delivery. The module covers ownership, review gates, conventions, and what should be enforced versus documented.

#### Lessons and Checkpoints

- 8.1.1 Who owns artifacts
- 8.1.2 Who owns rules and kits
- 8.1.3 When plans are required
- 8.1.4 When validation is required
- 8.1.5 Human approval boundaries
- 8.1.6 Checkpoint: draft a team operating policy

### 8.2 CI Integration

Description: This module teaches how deterministic checks move from local development into CI. Learners understand which commands belong in CI and how to treat failures.

#### Lessons and Checkpoints

- 8.2.1 Local checks before PR
- 8.2.2 Git pre-commit hooks with `cfs hook install`
- 8.2.3 `cfs validate` in CI
- 8.2.4 Local-only versus workspace validation
- 8.2.5 Exit code handling
- 8.2.6 Reporting validation results
- 8.2.7 Lab: design a CI validation gate

### 8.3 Review Readiness

Description: Learners prepare changes so reviewers can see scope, intent, evidence, validation, and remaining risk. The module turns Constructor Studio outputs into a review package.

#### Lessons and Checkpoints

- 8.3.1 What reviewers need
- 8.3.2 Evidence chain summary
- 8.3.3 Validation result summary
- 8.3.4 Known risks and open questions
- 8.3.5 PR review handoff
- 8.3.6 Lab: assemble a review-ready change summary

### 8.4 Version and Update Management

Description: This module teaches how teams update the CLI, project-installed core, generated integrations, and kits. Learners handle version notices, diffs, and schema changes.

#### Lessons and Checkpoints

- 8.4.1 Global cache and project-installed core
- 8.4.2 Version notices
- 8.4.3 `cfs update`
- 8.4.4 Kit update diffs
- 8.4.5 Regenerating integrations after update
- 8.4.6 Lab: plan a safe update

### 8.5 Adoption Patterns and Anti-Patterns

Description: This module helps teams avoid both underuse and overuse. Learners identify where Constructor Studio adds value and where it becomes unnecessary overhead.

#### Lessons and Checkpoints

- 8.5.1 Good first team use cases
- 8.5.2 Bad first team use cases
- 8.5.3 Avoiding giant prompt culture
- 8.5.4 Avoiding false proof claims
- 8.5.5 Keeping artifacts alive
- 8.5.6 Checkpoint: adoption scenario review

## 9. Capstone and Certification

Description: This part turns the course into an end-to-end proof of skill. Learners complete a realistic delivery scenario and produce artifacts, plans, implementation evidence, validation output, review notes, and an extension slice.

### 9.1 Capstone Scenario

Description: Learners receive a realistic brownfield or multi-repo change request. The scenario requires both operator skills and, for advanced certification, a small extension or kit workflow.

#### Lessons and Checkpoints

- 9.1.1 Scenario brief
- 9.1.2 Repository setup
- 9.1.3 Success criteria
- 9.1.4 Constraints and allowed shortcuts
- 9.1.5 Checkpoint: capstone readiness review

### 9.2 Operator Capstone Path

Description: The operator path proves daily use competence. Learners initialize or inspect setup, choose workflows, produce or update artifacts, plan the change, implement, validate, analyze, and prepare review evidence.

#### Lessons and Checkpoints

- 9.2.1 Environment and setup evidence
- 9.2.2 Workflow selection rationale
- 9.2.3 Artifact generation or update
- 9.2.4 Execution plan
- 9.2.5 Implementation with traceability
- 9.2.6 Validation and review loop
- 9.2.7 Final review package

### 9.3 Author Capstone Path

Description: The author path adds an extension requirement on top of operator competence. Learners design a small kit artifact kind, workflow, skill, or project-level rule and validate that it works.

#### Lessons and Checkpoints

- 9.3.1 Extension concept
- 9.3.2 Artifact kind or workflow design
- 9.3.3 Skill or command entry point
- 9.3.4 Generated host integration expectation
- 9.3.5 Extension validation
- 9.3.6 Final authoring review

### 9.4 Certification Review

Description: This module defines the evaluation rubric and evidence package. Learners are assessed on correctness, traceability, workflow choice, validation discipline, and clarity of handoff.

#### Lessons and Checkpoints

- 9.4.1 Operator rubric
- 9.4.2 Author rubric
- 9.4.3 Required evidence files
- 9.4.4 Common failure modes
- 9.4.5 Remediation path
- 9.4.6 Final certification checklist

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

- Complete Part 1: Course Frame
- Complete Part 2: Foundation
- Complete Part 3: Getting Started
- Complete Part 4: Operator Track
- Complete Part 5: Artifacts, Traceability, and Validation
- Complete Part 6 modules 6.1 through 6.8 as needed
- Complete Part 7 modules 7.1 through 7.6
- Complete Part 9.2 Operator Capstone Path

### B.2 Kit and Extension Author Path

Description: This path is for maintainers who design kits, workflows, skills, and project extensions. It assumes the learner has completed the operator foundations first.

#### Recommended Sequence

- Complete all New Operator Path modules
- Complete Part 7: Kit and Extension Author Track
- Complete Part 9.3 Author Capstone Path
- Complete Part 9.4 Certification Review

### B.3 Team Adoption Path

Description: This path is for technical leads planning rollout across a team or workspace. It prioritizes operating model, validation, review readiness, and adoption discipline.

#### Recommended Sequence

- Complete Part 2: Foundation
- Complete Part 3: Getting Started
- Complete Part 4 modules 4.1, 4.2, 4.5, and 4.7
- Complete Part 5 modules 5.1 through 5.6
- Complete Part 6 modules 6.3, 6.4, 6.5, and 6.8
- Complete Part 8: Governance, CI, and Team Adoption
- Review Part 9 certification rubric for internal enablement