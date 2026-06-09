# Constructor Studio v1 Overview Scripts for Video Production

<!-- toc -->

- [Production Framing](#production-framing)
- [Overview 1. Constructor Studio for a Mixed Audience](#overview-1-constructor-studio-for-a-mixed-audience)
  - [Story Goal](#story-goal)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction)
- [Overview 2. Constructor Studio for CTO and R&D Leaders](#overview-2-constructor-studio-for-cto-and-rd-leaders)
  - [Story Goal](#story-goal-1)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-1)
- [Overview 3. Constructor Studio for Product Managers](#overview-3-constructor-studio-for-product-managers)
  - [Story Goal](#story-goal-2)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-2)
- [Overview 4. Constructor Studio for Architects](#overview-4-constructor-studio-for-architects)
  - [Story Goal](#story-goal-3)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-3)
- [Overview 5. Constructor Studio for DevLeads and Developers](#overview-5-constructor-studio-for-devleads-and-developers)
  - [Story Goal](#story-goal-4)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-4)
- [Overview 6. Constructor Studio for QA Engineers](#overview-6-constructor-studio-for-qa-engineers)
  - [Story Goal](#story-goal-5)
  - [Narrator Script and Visual Direction](#narrator-script-and-visual-direction-5)
- [Closing Note for Production Team](#closing-note-for-production-team)

<!-- /toc -->

## Production Framing

This document is a script pack for six 5-minute overview videos about Constructor Studio v1. Each video should feel like a simple story for a wide audience: first the problem, then the solution, then how the solution works.

Use minimal text on screen. Let the narrator explain. Let animation show growth, fragmentation, connection, and control.

Default story spine for every overview:

1. Problem: AI tools now help teams generate much more code, markdown, specs, tasks, tests, and documentation. In mid-size and large organizations, the number of files and handoffs grows quickly. Existing tools can help generate even more, but they do not automatically give the organization control.
2. Solution: Constructor Studio is a customizable team environment for organizing AI-assisted software delivery across Product Managers, Architects, DevLeads, Developers, and QA engineers.
3. How it works: Studio routes work through shared workflows, file-backed evidence, role-specific skills, repeatable validation, and traceability between documents, code, and tests.

Keep technical names late in the story. Start with the organizational pain, not with commands or internal mechanics.

Learner-facing terms that can appear when needed:

- `cfs` for terminal setup, validation, and project operations.
- `cf` for invoking Studio workflows in the AI coding tool.
- Concrete skills such as `cf-write-docs`, `cf-brainstorm`, `cf-explore`, `cf-explain`, `cf-sdlc-doc-prd`, `cf-sdlc-doc-design`, `cf-sdlc-doc-adr`, `cf-sdlc-implement`, `cf-sdlc-reverse-engineer`, `cf-sdlc-change-impact-analysis`, and `cf-coding`.

Do not mention router-level workflow names in learner-facing video scripts.

---

## Overview 1. Constructor Studio for a Mixed Audience

### Story Goal

Explain why Constructor Studio exists for teams and organizations, not just for individual AI prompting.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | Modern AI tools give software teams a real productivity boost. They help write code, create markdown files, draft specs, generate tests, and explain unfamiliar systems much faster than before. | Show a team using AI tools. Code files, markdown docs, tasks, and tests appear rapidly around them. | AI makes more |
| 0:35-1:10 | But that boost creates a new problem. In a growing organization, the number of generated files and decisions can explode. Requirements drift. Design docs become stale. Tests stop matching intent. Code changes are hard to connect back to why they exist. | The generated files spread into disconnected clusters. Some links fade, some files conflict, some are marked incomplete. | More output, less control |
| 1:10-1:45 | Tools like OpenSpec and similar systems can help teams produce structured specs. That is useful. But generating more documents is not the same as keeping an organization aligned, consistent, and reviewable across teams. | Show a “generate specs” machine producing clean documents, then zoom out to messy handoffs between PM, architecture, development, and QA. | Generation is not governance |
| 1:45-2:20 | Constructor Studio is designed for that organizational layer. It gives teams a shared environment for AI-assisted delivery, where product work, architecture work, coding work, and QA work can stay connected. | The scattered files move into one shared delivery map with role lanes. | One shared delivery flow |
| 2:20-3:05 | Studio is not only for one person writing better prompts. It is for collaboration between roles and between teams. Product Managers shape requirements. Architects turn intent into decisions and design. Developers implement from approved context. QA checks behavior against traceable evidence. | PM, Architect, Developer, and QA lanes connect through shared files. | Teams, not solo prompting |
| 3:05-3:45 | The basic idea is simple: work is routed into the right workflow, with the right context, and with checks that make the result easier to inspect. Instead of one long chat, the team gets a repeatable path from intent to implementation and review. | A single chat thread transforms into a guided path: intent, design, feature, code, tests, review. | Right workflow, right context |
| 3:45-4:25 | Studio is also customizable. An organization can adapt templates, rules, workflows, validation, and codebase conventions instead of throwing away its existing process. The default SDLC kit gives teams a starting point, not a prison. | A default workflow adapts into several company-specific variants. | Fit your process |
| 4:25-5:00 | The outcome is control. AI can still help teams move faster, but the work becomes easier to connect, review, validate, and maintain. Constructor Studio turns AI-assisted output into a team delivery system. | End on a clean map where docs, code, tests, and review are connected. | Speed with control |

---

## Overview 2. Constructor Studio for CTO and R&D Leaders

### Story Goal

Help technical leaders decide whether Constructor Studio is a useful organizational control layer for AI-assisted delivery.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | For CTOs and R&D leaders, the main AI question is no longer “can developers generate code faster?” They can. The harder question is what happens when many teams generate code, documents, tests, and decisions faster at the same time. | Multiple teams generate artifacts in parallel. The volume rises quickly. | Scale changes the problem |
| 0:35-1:10 | Without a shared operating model, speed can turn into fragmentation. Teams may use different templates, lose decision history, skip review evidence, or produce documents that no longer match the codebase. | Show separate team islands with inconsistent docs and unclear handoffs. | Fragmentation risk |
| 1:10-1:45 | Constructor Studio is a proposed solution for that layer. It is an open-source, customizable environment that helps organize collaboration across Product Managers, Architects, Developers, DevLeads, and QA engineers. | The islands connect into one shared operating layer. | Shared operating layer |
| 1:45-2:25 | Studio differs from individual or project-centered specification tools because it is focused on organizational delivery control. The goal is not just to create one more spec. The goal is to keep intent, decisions, implementation, tests, and review evidence connected. | Compare “project spec” with “organization workflow”: the second shows cross-role links. | Beyond project specs |
| 2:25-3:05 | The mechanism is straightforward. Studio uses workflows and concrete skills for different kinds of work: brainstorming, exploration, PRD writing, design, ADRs, implementation, reverse engineering, and change impact analysis. | Role lanes call specific skills only after the problem is introduced. | Workflows by role |
| 3:05-3:40 | Traceability is the control point. Canonical Provenance Trace IDs can connect documents and code so teams can reason about consistency. Validation can check structure, references, and configured rules. Human review remains the final authority. | A chain connects PRD, DESIGN, FEATURE, code, tests, and approval. | Traceable evidence |
| 3:40-4:20 | Adoption does not require a process reset. Teams can start with the default SDLC kit and then customize document templates, checklists, workflows, and codebase rules to match existing governance. | Default kit expands into organization-specific process gates. | Start standard, adapt |
| 4:20-5:00 | The leadership case is simple: Constructor Studio helps preserve the AI productivity boost while reducing the risk that generated code and documents become inconsistent, incomplete, or impossible to govern at scale. | End with a leader dashboard-style view of connected teams and artifacts. | AI speed, governed delivery |

---

## Overview 3. Constructor Studio for Product Managers

### Story Goal

Show Product Managers how Studio helps keep product intent clear, reviewable, and reusable downstream.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | Product work often starts as a conversation: a customer need, a stakeholder request, a feature idea, or a rough market assumption. AI can turn that into text very quickly. | A rough idea becomes a long generated document. | Ideas become text |
| 0:35-1:10 | The problem is that fast text can still be unclear. It may miss actors, constraints, edge cases, success criteria, or tradeoffs. When that unclear intent moves downstream, architects and developers fill gaps with assumptions. | Missing requirement fields create warning marks in later role lanes. | Fast text can drift |
| 1:10-1:45 | Constructor Studio helps Product Managers turn early intent into product requirements that are easier for the whole team to review and reuse. | Rough notes become a structured PRD connected to architecture and QA. | Intent becomes reviewable |
| 1:45-2:25 | A PM can use `cf-brainstorm` to explore options before committing to scope. The point is not to get a pretty answer. The point is to surface alternatives, risks, missing questions, and decision criteria early. | Branching options appear, then collapse into a chosen direction with open questions. | Explore before scope |
| 2:25-3:05 | When the direction is ready, `cf-sdlc-doc-prd` helps create or review a PRD using structured expectations. `cf-write-docs` supports broader product writing when the document is less formal. | Two paths: formal PRD and flexible product document. | PRD and docs |
| 3:05-3:40 | Studio also helps with review. `cf-explain` can make dense material easier to understand, and PRD-specific workflows can validate whether the requirement is clear enough for architecture, development, and QA. | A dense PRD becomes a concise summary plus review notes. | Review before handoff |
| 3:40-4:25 | This improves collaboration because downstream teams receive something more stable than a chat transcript. Architects can reference the PRD. Developers can implement against it. QA can design tests against visible intent. | One PRD feeds architecture, implementation, and QA lanes. | Stable handoff |
| 4:25-5:00 | For Product Managers, the value is not more documentation for its own sake. The value is clearer intent that survives the path from idea to design, code, tests, and release decisions. | End with a single requirement connected across the delivery chain. | Intent that survives |

---

## Overview 4. Constructor Studio for Architects

### Story Goal

Show Architects how Studio helps turn requirements and existing codebase context into controlled design decisions.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | Architects often sit in the middle of the AI acceleration problem. Product intent is changing faster. Code is changing faster. Documentation is being generated faster. But architecture still needs coherence. | Product docs, code changes, and design notes move quickly around an architect. | Speed needs coherence |
| 0:35-1:10 | The risk is hidden drift. A PRD may imply one architecture. Existing code may support another. A design document may become stale as implementation moves ahead. | Show PRD, design, and code slowly separating from each other. | Hidden drift |
| 1:10-1:45 | Constructor Studio gives Architects a way to work from evidence instead of memory. Before deciding, they can collect context from documents, folders, code, and existing architecture material. | Evidence cards collect from repo, docs, and previous decisions. | Evidence before design |
| 1:45-2:25 | `cf-explore` supports that discovery step. It helps gather relevant codebase and document context before the architect writes or changes a design. | A search beam scans repo and docs, then produces a context board. | Explore first |
| 2:25-3:05 | If the decision is still open, `cf-brainstorm` helps compare options and tradeoffs. Once the direction is clear, `cf-sdlc-doc-design` captures the design and `cf-sdlc-doc-adr` records key architecture decisions. | Options board turns into DESIGN and ADR files. | Decide, then record |
| 3:05-3:45 | In existing systems, Architects can also use `cf-sdlc-reverse-engineer` to reconstruct design understanding from code, and `cf-sdlc-change-impact-analysis` to estimate what a proposed change may touch. | Brownfield code turns into a design map and impact links. | Brownfield needs maps |
| 3:45-4:25 | The important point is control. Studio does not make architecture automatic. It helps keep requirements, decisions, constraints, codebase evidence, and downstream features visible to reviewers. | Architecture chain connects PRD, ADR, DESIGN, FEATURE, code, and review. | Visible decisions |
| 4:25-5:00 | For Architects, Constructor Studio is a way to slow the right things down: not delivery speed, but unreviewed assumptions. The result is faster collaboration with fewer invisible architecture gaps. | End with design decisions anchored to evidence and downstream work. | Fewer invisible gaps |

---

## Overview 5. Constructor Studio for DevLeads and Developers

### Story Goal

Show DevLeads and Developers how Studio keeps implementation work bounded, traceable, and easier to review.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | Developers feel the AI boost directly. Code can be generated faster. Tests can be drafted faster. Bug explanations can arrive faster. But faster editing can also create faster confusion. | Code, tests, and fixes appear quickly in an editor. Some lose links to requirements. | Faster code, faster confusion |
| 0:35-1:10 | The problem is not that AI writes code. The problem is code without enough context: unclear requirement links, missing design decisions, weak tests, or changes that reviewers cannot trace back to intent. | A pull request appears with unanswered questions around it. | Context is the bottleneck |
| 1:10-1:45 | Constructor Studio helps developers start from approved inputs instead of a vague chat summary. Work can begin from PRD, DESIGN, ADR, or FEATURE artifacts that explain why the change exists. | Editor opens next to linked FEATURE and DESIGN files. | Code from intent |
| 1:45-2:25 | For planned feature work, `cf-sdlc-implement` helps implement from approved FEATURE context. For smaller focused changes, `cf-coding` supports code and unit test work without pretending every edit needs a large process. | A large feature uses full workflow; a small fix uses a lighter path. | Right size workflow |
| 2:25-3:05 | For unfamiliar code or bugs, `cf-explore` helps developers understand the area before changing it. That matters because random edits in unknown code create review risk and regression risk. | A bug report links to targeted code exploration before the fix. | Explore before fixing |
| 3:05-3:45 | Tests become part of the same story. Instead of writing tests only against implementation details, developers can connect tests back to feature intent and expected behavior. | FEATURE intent generates code and tests side by side. | Tests follow intent |
| 3:45-4:25 | Before review, `cfs` can run repeatable checks for the configured project surface. These checks do not replace human judgment, but they give reviewers a cleaner evidence packet. | Terminal checks pass, then a reviewer inspects the linked evidence. | Checks before review |
| 4:25-5:00 | For DevLeads, the value is consistency across a team. More work follows a visible chain from intent to code to tests, and less knowledge is trapped in private prompts or one-off chats. | Multiple developer lanes converge into one reviewable team flow. | Reviewable team work |

---

## Overview 6. Constructor Studio for QA Engineers

### Story Goal

Show QA engineers how Studio makes expected behavior, evidence, and traceability easier to inspect before test work begins.

### Narrator Script and Visual Direction

| Time | Narrator Script | Animation / Visual Direction | On-Screen Text |
|---|---|---|---|
| 0:00-0:35 | QA teams are also affected by AI acceleration. More code changes arrive. More generated tests appear. More documents claim to describe behavior. But QA still needs to know what is actually expected. | A QA board receives many code, doc, and test artifacts at once. | More artifacts to verify |
| 0:35-1:10 | The problem is weak evidence. If requirements, design, implementation, and tests are disconnected, QA has to reconstruct intent from tickets, chats, diffs, and meetings. | A QA engineer follows broken links between ticket, doc, code, and test. | Intent gets scattered |
| 1:10-1:45 | Constructor Studio helps QA work from a clearer chain. A change can carry product intent, design context, feature behavior, implementation evidence, and validation results together. | The scattered artifacts connect into one evidence chain. | Clearer evidence chain |
| 1:45-2:25 | `cf-explore` and `cf-explain` help QA engineers understand the codebase and related documents before writing or extending tests. This is especially useful in brownfield systems where behavior is spread across older modules. | QA starts from a context map before writing tests. | Understand before testing |
| 2:25-3:05 | `cf-coding` can support automated test authoring when the expected behavior is clear. The goal is not to generate tests blindly, but to write tests against visible intent and requirement links. | Test cases connect back to feature behavior and requirements. | Test against intent |
| 3:05-3:45 | Repeatable checks add another signal. If references, structure, or configured traceability fail, QA can see that early. Passing checks do not prove quality, but failing checks expose review risk. | Validator catches a broken reference before QA approval. | Checks expose risk |
| 3:45-4:25 | This changes collaboration. QA is no longer only at the end of a code diff. QA can inspect the same delivery chain that Product, Architecture, and Development used to create the change. | QA joins the shared PM, Architect, Developer workflow map. | QA inside the flow |
| 4:25-5:00 | For QA engineers, Constructor Studio provides better context before testing, stronger evidence during review, and a clearer path from requirement to behavior to automated tests. | End on requirement, feature, code, test, and approval connected. | Better context, better tests |

---

## Closing Note for Production Team

Each overview must lead with the organizational problem before naming Studio mechanics. The audience should first feel the pain: AI creates more code and markdown faster, and that creates control, consistency, completeness, and review problems.

Only after that should the narrator introduce Constructor Studio as the solution: a customizable collaboration environment for teams, roles, workflows, evidence, validation, and traceability.

Recurring visual pattern:

- First show artifact explosion.
- Then show drift and inconsistency.
- Then show Studio connecting roles and artifacts.
- Then show a simple evidence chain from intent to code to tests to review.
