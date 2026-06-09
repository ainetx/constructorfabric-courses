# Constructor Studio v1 Overview Course for Video Production


<!-- toc -->

- [Course Framing](#course-framing)
- [Lesson 1. Overview for Mixed Audience](#lesson-1-overview-for-mixed-audience)
  - [Goal](#goal)
  - [Audience Outcome](#audience-outcome)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction)
- [Lesson 2. Overview for CTO / R&D Leaders](#lesson-2-overview-for-cto--rd-leaders)
  - [Goal](#goal-1)
  - [Audience Outcome](#audience-outcome-1)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples-1)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-1)
- [Lesson 3. Overview for Product Managers](#lesson-3-overview-for-product-managers)
  - [Goal](#goal-2)
  - [Audience Outcome](#audience-outcome-2)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples-2)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-2)
- [Lesson 4. Overview for Architects](#lesson-4-overview-for-architects)
  - [Goal](#goal-3)
  - [Audience Outcome](#audience-outcome-3)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples-3)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-3)
- [Lesson 5. Overview for DevLeads and Developers](#lesson-5-overview-for-devleads-and-developers)
  - [Goal](#goal-4)
  - [Audience Outcome](#audience-outcome-4)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples-4)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-4)
- [Lesson 6. Overview for QA Engineers](#lesson-6-overview-for-qa-engineers)
  - [Goal](#goal-5)
  - [Audience Outcome](#audience-outcome-5)
  - [Role-Specific Proof Points and Examples](#role-specific-proof-points-and-examples-5)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-5)
- [Closing Note for Production Team](#closing-note-for-production-team)

<!-- /toc -->

## Course Framing

This course is an English video-production script pack for six primary lessons for Constructor Studio v1. It stays at the product and workflow level and does not lock to one strict patch or minor version. Use the current learner-facing terms throughout: Constructor Studio, `cfs`, `cf`, and the real workflow skill names such as `cf-write-docs`, `cf-sdlc-doc-prd`, and `cf-sdlc-implement`.

Common through-line for all lessons:

> Constructor Studio turns AI coding from an open-ended chat into a routed, evidence-backed operating system for software delivery, where the right context, workflow, validation, and approval happen in the right order.

Trust boundary for all lessons:

> Constructor Studio makes AI-driven delivery easier to inspect and audit: repeatable checks and linked files support review, while human review remains the final control.

Primary first-run path to visualize in every role where relevant:

`explore/brainstorm -> PRD -> ADR + DESIGN -> DECOMPOSITION -> FEATURE -> implementation -> validation/review`

Canonical sources for production:

- Product model and current distribution: `workspace-sources/constructorfabric/studio/README.md`.
- Configuration and validation behavior: `workspace-sources/constructorfabric/studio/guides/CONFIGURATION.md`.
- Software Development Lifecycle (SDLC) kit specifics: `workspace-sources/constructorfabric/studio-kit-sdlc/README.md`.

Production notes:

- Keep on-screen text minimal. Each visual cue should stay between 3 and 7 words.
- Let the narrator carry the meaning.
- Let the animation show sequence, flow, handoff, and traceability.
- Treat reverse engineering and impact analysis as brownfield adoption hooks, not the main first-run path.
- If historical context is needed, keep it to a short migration note only.

---

## Lesson 1. Overview for Mixed Audience

### Goal

Give a cross-functional audience a simple mental model of Constructor Studio as a team operating layer around AI coding tools.

### Audience Outcome

By the end of the lesson, viewers should understand what Constructor Studio is, why teams use it, how it fits into normal software delivery, and why human review remains the final control.

### Role-Specific Proof Points and Examples

- Product managers can brainstorm and write PRDs with structured workflows instead of one long chat.
- Architects can move from approved requirements into DESIGN and ADR artifacts with visible references.
- Developers can implement from approved FEATURE inputs and run repeatable checks before review.
- QA engineers can validate traceability, inspect evidence, and write automated tests against a clearer spec chain.
- Teams can adopt the default SDLC flow or customize the system to match existing process, documents, and codebase structure.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | Constructor Studio is a workflow, context, and validation layer for AI-assisted software delivery. It does not replace Claude Code, Codex, or similar tools. It organizes them. | Start with a noisy chat window. Wrap it with a clear operating frame labeled workflow, context, validation, approval. | From chat to system |
| 0:35-1:10 | The core shift is simple. Instead of one open-ended conversation, work gets routed into the right workflow with the right context and checks loaded at the right time. | Show one message splitting into routed lanes: explore, brainstorm, docs, implementation, review. | Right workflow first |
| 1:10-1:50 | Constructor Studio is designed for teams, not only for individual prompting. Product, architecture, code, and QA work can stay connected through shared artifacts and reviewable evidence. | Show PM, architect, developer, QA avatars connected to the same repo timeline. | Teams share one flow |
| 1:50-2:35 | The normal first-run path is straightforward: explore or brainstorm, write a PRD, capture ADR and DESIGN work, decompose the scope, write FEATURE artifacts, implement from those approved inputs, then validate and review. | Animate the SDLC chain as a horizontal flow with files appearing at each step. | Explore to review |
| 2:35-3:15 | Constructor Studio adds repeatable checks and file-backed evidence. That means structure, references, and configured traceability can be checked in a repeatable way. It does not prove business adequacy or guarantee bug-free code. | Show green checks on files and links, then stop at a human approval gate. | Evidence, not certainty |
| 3:15-4:05 | The command surface is split on purpose. `cfs` runs setup and validation in the terminal. `cf` routes work in the AI coding tool chat. That separation keeps execution more legible for teams. | Terminal and chat panes appear side by side, with arrows showing their roles. | `cfs` and `cf` together |
| 4:05-4:40 | The system is also customizable. Teams can fit it into their own SDLC, documentation rules, review gates, and codebase conventions instead of replacing everything at once. | Show a default template morph into several team-specific process shapes. | Adapt to your process |
| 4:40-5:00 | The right summary is this: Constructor Studio makes AI work more bounded, reviewable, and auditable, while people still decide what is good enough to ship. | End on the full chain, then highlight the final human approval node. | Human review stays final |

---

## Lesson 2. Overview for CTO / R&D Leaders

### Goal

Explain Constructor Studio as an adoption and operating model for organizations that want team-level AI delivery with governance, reuse, and visible control points.

### Audience Outcome

By the end of the lesson, CTOs and R&D leaders should understand where Constructor Studio fits in the tool stack, what kind of governance it adds, how it supports cross-team collaboration, and how to position it against individual or project-level alternatives.

### Role-Specific Proof Points and Examples

- Shared workflow across PM, architecture, development, and QA instead of isolated prompting habits.
- Canonical Provenance Trace (CPT) IDs and file-backed evidence for review and audit surfaces.
- Default SDLC kit for a fast starting point, with room to customize rules, artifacts, and validation depth.
- Better organizational fit than individual or project-only systems when teams need the same delivery language.
- Apache 2.0 open source under the Constructor Fabric Foundation positioning.
- Roadmap items to mention as future plans only: planned macOS, Windows, and web application experiences; planned PyPI release distribution.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:40 | For leaders, the main question is not whether AI can generate code. It already can. The question is how to make that work repeatable, reviewable, and usable across teams. | Start with many disconnected chats across teams, then zoom out to organizational fragmentation. | Scale needs operating rules |
| 0:40-1:20 | Constructor Studio answers that by turning AI coding into a routed operating model. Product, architecture, implementation, validation, and review all work through shared workflows and file-backed evidence. | Replace scattered chat bubbles with one shared delivery map across roles. | One delivery language |
| 1:20-2:00 | The strongest adoption point is cross-team collaboration. PMs, architects, developers, and QA engineers can all work on the same chain instead of handing off loose documents and memory from tool to tool. | Show artifact handoffs as connected files, not separate slide decks or chat logs. | Shared artifacts, shared context |
| 2:00-2:45 | Constructor Studio also gives leaders a stronger trust boundary. Repeatable checks can verify configured structure, references, and traceability markers. Human reviewers still decide adequacy, risk, and release readiness. | Show validator pass, then a separate leadership or reviewer sign-off step. | Checks support human control |
| 2:45-3:25 | Unlike project-only spec tools, Constructor Studio focuses on shared team workflow, linked documents, and repeatable checks. | Show a comparison board where Constructor Studio is highlighted on team workflow, linked docs, and checks. | Shared team workflow |
| 3:25-4:00 | Adoption does not require a process reset. Teams can start with the default SDLC kit, then customize workflows, rules, templates, and validation surfaces to match existing SDLC expectations. | Show a default kit landing first, then expanding into customized org patterns. | Start standard, adapt later |
| 4:00-4:30 | This matters for governance and sustainability too. Constructor Studio is Apache 2.0 open source under the Constructor Fabric Foundation positioning, which lowers adoption friction for long-term teams. | Animate license and foundation badges as stable infrastructure pieces. | Apache 2.0 open source |
| 4:30-5:00 | Looking ahead, current docs describe planned macOS, Windows, and web application experiences, plus planned PyPI release distribution. Present these as future direction, not current capability. | Show a roadmap lane with clearly labeled future milestones. | Roadmap, not current scope |

---

## Lesson 3. Overview for Product Managers

### Goal

Show product managers how Constructor Studio helps shape intent, improve requirement quality, and keep delivery discussion anchored in reviewable artifacts.

### Audience Outcome

By the end of the lesson, product managers should understand how to use Constructor Studio for brainstorming, PRD authoring, requirement review, and explanation workflows without needing to own the full technical stack.

### Role-Specific Proof Points and Examples

- Use `cf-brainstorm` to explore options before locking scope.
- Use `cf-write-docs` for general drafting, refinement, and review of human-facing content.
- Use `cf-sdlc-doc-prd` to create and revise PRDs in the SDLC flow.
- Use `cf-explain` and `cf-analyze` to make dense product content easier for other teams to consume and review.
- Keep requirements visible as files instead of buried in chat history.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | For product managers, Constructor Studio starts before code. Its first value is helping turn rough intent into clearer, reviewable product requirements. | Show a rough idea card becoming structured requirement sections. | Intent becomes structure |
| 0:35-1:15 | A practical first step is brainstorming. With `cf-brainstorm`, a PM can explore product options, risks, tradeoffs, and missing questions before a requirement document is written. | Animate idea branches opening, then narrowing into a chosen path. | Brainstorm before commitment |
| 1:15-1:55 | Once the direction is clearer, `cf-sdlc-doc-prd` can turn that input into a PRD with a defined structure. `cf-write-docs` supports broader writing and revision tasks when the work is less formal. | Show two paths: structured PRD flow and flexible docs flow. | PRD and docs workflows |
| 1:55-2:35 | This matters because AI can write fast, but fast text is not the same as aligned intent. Constructor Studio helps keep goals, actors, functional needs, and constraints in a form other roles can review and reuse. | Overlay a PRD with highlighted actors, goals, requirements, and constraints. | Reviewable product intent |
| 2:35-3:15 | Product managers also benefit from explanation and review workflows. A dense PRD can be summarized, clarified, or reviewed for gaps before it reaches architecture and engineering. | Show a long document collapsing into a clean executive summary and issue list. | Explain and review |
| 3:15-4:00 | In team use, this reduces drift during handoff. Architects can reference the PRD. Developers can see what feature behavior came from. QA can validate that tests trace back to something intentional. | Show one PRD feeding the next three roles through linked references. | Better downstream handoff |
| 4:00-4:35 | Constructor Studio also fits existing process. If your organization already has document standards, approval flow, or required sections, the platform can be customized instead of forcing a new template forever. | Show a company PRD template blending into the Studio workflow. | Fit existing document rules |
| 4:35-5:00 | The main takeaway for PMs is simple: use Constructor Studio to shape clearer intent, produce stronger PRDs, and create requirements that survive the trip from idea to implementation. | End on a PRD becoming the first stable file in the chain. | Clearer intent, safer handoff |

---

## Lesson 4. Overview for Architects

### Goal

Show architects how Constructor Studio supports architecture discovery, design authoring, decision capture, and controlled brownfield understanding.

### Audience Outcome

By the end of the lesson, architects should understand how to gather context, explain existing systems, write DESIGN and ADR artifacts, and use reverse engineering or impact analysis when entering a brownfield codebase.

### Role-Specific Proof Points and Examples

- Use `cf-brainstorm` to examine architecture options and tradeoffs before deciding.
- Use `cf-explore` to gather codebase and document context before writing or changing design.
- Use `cf-explain` and `cf-analyze` to inspect PRDs, DESIGNs, and codebase structure.
- Use `cf-sdlc-doc-design` and `cf-sdlc-doc-adr` to author or revise formal DESIGN and ADR artifacts.
- Use `cf-sdlc-reverse-engineer` and `cf-sdlc-change-impact-analysis` as adoption hooks for existing systems, not as the default first-run path.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:40 | Architects often enter the flow where product intent must become technical shape. Constructor Studio helps by making the context gathering and design path explicit. | Show a PRD flowing into a context board and then into design artifacts. | Intent to architecture |
| 0:40-1:20 | The first strong route here is `cf-explore`. Before changing design, architects can inspect code, docs, directories, and related artifacts so the design work starts from evidence, not assumption. | Animate a scanner moving across repo folders, docs, and diagrams. | Explore before deciding |
| 1:20-2:00 | If the problem is still open, `cf-brainstorm` helps compare patterns and tradeoffs. Once the direction is ready, `cf-sdlc-doc-design` writes the technical DESIGN and `cf-sdlc-doc-adr` records key architecture decisions. | Split screen: option comparison on one side, formal DESIGN and ADR files on the other. | Decide, then record |
| 2:00-2:40 | This is valuable because architecture is where hidden assumptions spread fast. Constructor Studio keeps drivers, decisions, constraints, and downstream feature links visible and reviewable. | Highlight requirement IDs, decision nodes, and feature links across documents. | Visible design chain |
| 2:40-3:20 | Architects also need explanation and review support. A PRD can be reviewed for technical pressure points. A design can be explained to developers. A codebase can be summarized before planning a refactor. | Show one architect using explain mode for three different artifacts. | Explain complex systems |
| 3:20-4:05 | In brownfield work, reverse engineering and impact analysis become important. They help reconstruct architecture from code and estimate what a proposed change touches. But they are adoption hooks, not the main first-run path for new work. | Show a brownfield branch peeling off from the main SDLC line. | Brownfield starts anywhere |
| 4:05-4:40 | Constructor Studio is also customizable enough for architecture governance. Teams can encode design rules, review checklists, and project conventions so the system reflects the real codebase and not only a generic template. | Animate rules and checklists snapping into the workflow frame. | Encode architecture rules |
| 4:40-5:00 | For architects, the core value is controlled translation: from product intent and existing system context into decisions, design, and impact-aware change planning. | End on a stable DESIGN feeding multiple FEATURES. | Controlled technical translation |

---

## Lesson 5. Overview for DevLeads and Developers

### Goal

Show engineering leads and developers how Constructor Studio supports implementation from approved design, bounded execution, testing, debugging, and more reliable review preparation.

### Audience Outcome

By the end of the lesson, developers and leads should understand how to analyze design inputs, implement from FEATURES, write unit tests, explore unfamiliar code, fix bugs, and use repeatable checks before human review.

### Role-Specific Proof Points and Examples

- Review DESIGN and FEATURE inputs with `cf-analyze` before implementation instead of coding from memory.
- Use `cf-sdlc-implement` to implement from approved FEATURE inputs with traceable links when configured.
- Use `cf-coding` to write focused code changes, unit tests, and supporting implementation work.
- Use `cf-explore` and `cf-analyze` for unfamiliar code or bug-fix work.
- Use repeatable checks through `cfs` before asking for review.
- Future progress tracking is relevant for leads and coordinators, but should be framed as direction, not as a fully described current feature set.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | For developers, Constructor Studio is not about adding paperwork before every edit. It is about using the right amount of structure when a change is multi-step, risky, or review-sensitive. | Start with a small fix bypassing heavy flow, then switch to a larger feature using the full chain. | Use structure when needed |
| 0:35-1:15 | A strong engineering habit is to start from approved inputs. Review the PRD, DESIGN, or FEATURE that defines the change. Then implement from that artifact instead of from a vague chat summary. | Show code editor opening beside a FEATURE file with linked references. | Code from approved inputs |
| 1:15-1:55 | During implementation, Constructor Studio helps bound the task. The workflow can separate exploration, planning, authoring, review, and validation so one long thread does not mix every job together. | Animate a large task being divided into clear stages. | Split the work |
| 1:55-2:35 | This also helps when writing unit tests. Tests become part of the same evidence chain, not an afterthought. Developers can implement behavior and the supporting tests from the same feature-level intent. | Show code and tests appearing in parallel from one feature artifact. | Tests follow the feature |
| 2:35-3:15 | For bug fixing or brownfield work, `cf-explore` and `cf-analyze` matter. They help developers inspect unfamiliar areas, explain existing logic, and reduce random edits in code they do not yet understand. | Show a bug report linking to targeted code exploration before editing begins. | Explore before fixing |
| 3:15-3:55 | Before review, `cfs` provides repeatable checks for the configured project surface. That can include structure, references, and traceability markers where the team has enabled them. It is a repeatable quality signal, not a final approval. | Show terminal checks running, then a reviewer entering after the checks pass. | Repeatable checks first |
| 3:55-4:30 | For dev leads, the team value is consistency. More work follows the same chain, evidence is easier to inspect, and future progress tracking can become more visible for coordination as the platform evolves. | Show multiple feature branches converging into one visible team board. | Better team visibility |
| 4:30-5:00 | The developer takeaway is simple: Constructor Studio helps turn AI-assisted coding into a more bounded, test-aware, review-ready engineering workflow. | End on implementation, tests, validation, and review in one lane. | Bounded and review-ready |

---

## Lesson 6. Overview for QA Engineers

### Goal

Show QA engineers how Constructor Studio improves test design, codebase analysis, evidence review, and traceability-aware validation.

### Audience Outcome

By the end of the lesson, QA engineers should understand how Constructor Studio helps them analyze the system under test, write automated tests with better context, and validate that implementation evidence aligns with approved artifacts.

### Role-Specific Proof Points and Examples

- Use `cf-explore` and `cf-analyze` to understand codebase and artifact context before creating tests.
- Use `cf-coding` to write automated tests against clearer behavior definitions and requirement links.
- Validate evidence and traceability instead of relying only on verbal handoff.
- Use repeatable checks as an input into QA review, not as a replacement for test judgment.
- Work more effectively with PM, architecture, and engineering because upstream intent remains visible.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | For QA engineers, Constructor Studio improves visibility. Instead of receiving only a code diff and a short summary, QA can inspect the requirement, design, feature intent, and validation evidence around the change. | Show a diff view expanding into linked artifacts and checks. | More than a diff |
| 0:35-1:15 | That matters for test design. When expected behavior is clearer, automated tests can target the real intent of the change, not only the shape of the implementation. | Animate a test matrix generated from visible feature behavior. | Test against intent |
| 1:15-1:55 | QA can also use `cf-explore` and `cf-analyze` to understand the codebase before writing or extending tests. This is especially useful in brownfield systems where behavior is spread across older modules. | Show test authoring starting from codebase exploration rather than guesswork. | Understand before testing |
| 1:55-2:35 | Repeatable checks add another useful signal. If references, structure, or configured traceability fail, QA sees that early. But even a clean validation result does not replace real test thinking or release judgment. | Show a validator failure surfacing before a manual QA review board. | Checks inform QA |
| 2:35-3:15 | Traceability is especially useful when the team enables it deeply. A QA engineer can follow a requirement into a feature, then into implementation markers and tests, which makes coverage conversations more concrete. | Animate a clickable chain from requirement to feature to code to test. | Follow the evidence chain |
| 3:15-4:00 | Constructor Studio also supports team collaboration. PM intent, architecture decisions, engineering implementation, and QA validation can all stay in one reviewable flow instead of separate tools and meeting notes. | Show all roles contributing to one shared release packet. | QA inside team flow |
| 4:00-4:35 | The platform is customizable too. If a team has specific test evidence rules, document standards, or validation checkpoints, those can become part of the operating model over time. | Show a QA checklist being attached to the workflow. | Add your QA gates |
| 4:35-5:00 | The QA summary is this: Constructor Studio gives QA better context, better evidence, and a stronger path from intent to test and review. | End on a release decision supported by linked evidence. | Better context, better validation |

---

## Closing Note for Production Team

Across all six primary lessons, keep the pacing calm and concrete. The narrator should explain the why, the workflow, and the trust boundary. The visuals should repeatedly reinforce four ideas:

- Constructor Studio is a team operating layer around AI coding tools.
- The main path is routed SDLC work, not open-ended prompting.
- Repeatable checks and file-backed evidence improve reviewability, but do not replace human judgment.
- The system is customizable enough to fit existing process, document, and codebase requirements.
