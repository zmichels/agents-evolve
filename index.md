---
layout: default
title: Automation as a product that learns
date_published: "2026-10-06"
date_modified: "2026-10-07"
---

# Automation as a product that learns

*Zachary D. Michels · Perspective · October 6, 2026*
{: .article-meta }

The future of automation is a product that evolves. It completes useful work, learns from the experience, and earns trust in its next improvement.

That is a production expectation worth building toward. We already improve software between releases. Agentic systems let us bring more of that cycle into the product itself: record a correction, recognize a recurring gap, propose a change, and test whether it helps. The design determines how much of that work the agent performs independently.

Generation gets the work started. Dependable execution gets it finished. Learning carries something useful into the next run. A newer model can expand capability, but the lessons specific to a workflow need a deliberate path into future behavior.

RPA set the stage for this ambition and remains part of its delivery. The next step is a product that adapts while earning the confidence we associate with a well-engineered, deterministic automation.

## RPA established a foundation for trust

In a conventional RPA workflow, developers and subject matter experts translate judgment into explicit logic. We can inspect the branches, test the checks, and specify where execution stops. That work gives us a basis for letting a process run without watching every step.

The logic still needs to be right. Websites change, sessions expire, and transactions fail halfway through. Automation engineers build detection and recovery around those conditions. Trust comes from understanding what the system does and how it responds when the expected path breaks.

RPA also continues to close practical gaps. An agent can interpret a document and prepare the right information, yet still reach a destination application without a suitable API. A robot enters the information and checks the result. That familiar integration is the closer: it turns the agent's output into completed work.

Agents extend the range of interpretation and choice. RPA supplies one dependable way to act. Together with APIs, direct computer use, and human review, they form workflows whose parts need to learn from one another's outcomes.

## Agents can learn where the gaps are and build bridges across them

Coding capabilities extend an agent's role. Alongside choosing and using tools, it can help draft integrations, applications, and robot workflows. That connects three useful activities: identify a gap, plan a bridge, and help build it.

A changed screen calls for a different repair from a missing source or an incorrect mapping. The first task is to understand which problem occurred. A robot can faithfully execute the wrong instruction; an agent can choose correctly and encounter a broken interface.

Once the problem is clear, an agent can help develop the missing check, revised integration, or new workflow step. Its participation belongs in the production design. One product collects evidence and proposes repairs. Another drafts changes for review. A more dynamic product applies tested changes within a defined area, checks the outcome, and retains a reversal path.

This is how we specify the agent's sphere of influence. The ability to write a change, the evidence that it works, and the authority to release it remain distinct.

## Learning must follow the whole workflow

A useful lesson connects the request, the evidence, the decision, the action, and the verified outcome. If the record ends when an agent launches a bot, the explanation for success or failure may disappear at the handoff. The same applies when work passes to an API, another agent, or a person.

The final step often contains the lesson. An expert corrects a field. A robot encounters an unexpected screen. A reviewer finds conflicting sources. Preserve what happened and why, and the next run has something to learn from.

[![Each run decides, acts, and verifies. Evidence across the workflow feeds linked records, decision-state mapping, and tested improvements. Changes adopted within delegated authority feed future runs.]({{ '/assets/improvement-cycle.svg' | relative_url }})]({{ '/assets/improvement-cycle.svg' | relative_url }})

*Today's workflow builds tomorrow's decision knowledge. Tested changes carry it forward.*
{: .figure-caption }

Observability and evaluation tools already connect production feedback to reviewed examples, test datasets, and comparisons of proposed changes. The work now is to make that cycle part of the complete product, including its handoffs and exceptions.

A recurring problem becomes a proposed improvement. Tests establish where it helps and where it fails. An accepted change enters the workflow, and outcome checks continue. The change might be a better instruction, a source lookup, a deterministic rule, or new code. Learning does not always require model retraining.

Design this path before release: what evidence survives, how corrections become lessons, what the agent may change, and how changes reach production. Recording experience provides the material. The improvement cycle puts it to work.

## Map how decisions and their supporting knowledge evolve

As an automation changes, so does the knowledge behind its decisions. A source resolves an ambiguity. A reviewer explains an exception. A new check changes when the workflow proceeds. We need to preserve those connections and track how they develop across steps, executions, and revisions.

Platforms such as [Langfuse](https://langfuse.com/docs/evaluation/core-concepts) already support much of the surrounding work: tracing, human feedback, evaluation datasets, and experiments that compare proposed changes. Its [feedback-to-evaluation workflow](https://langfuse.com/resources/engineering/user-feedback-to-evaluation-datasets) connects production observations and corrections to future tests. These capabilities provide a growing foundation for learning through use.

The [Decision-PGA article series](https://zmichels.github.io/decision-pga-pages/article/) offers a starting point for exploring two layers of that work. Its articles, code, and examples are exploratory material to adapt to a purpose, not a prescribed application architecture.

**The first layer preserves and links experience.** A customizable ledger records evidence, actions, tool results, corrections, outcomes, and the versions and conditions involved. Decision states are part of that record, alongside the surrounding knowledge. Links show which source supported an interpretation, which test challenged it, and which lesson led to a change. New understanding adds to the history rather than erasing what the system knew at the time.

**The second layer examines how decision support takes shape and changes.** Decision-PGA represents each observation as a probability vector: a list of support values for choices such as proceed, retrieve more evidence, or request review. Repeated observations form a cloud of points, mapped onto a curved surface for analysis.

PGA stands for [Principal Geodesic Analysis](https://pubmed.ncbi.nlm.nih.gov/15338733/). It extends the idea behind Principal Component Analysis—finding the main directions of variation—to curved spaces. Decision-PGA adapts that idea to examine how support spreads across possible decisions. The geometry describes those observations, rather than the agent's internal reasoning.

The [telescoping perspective](https://zmichels.github.io/decision-pga-pages/telescoping/) examines smaller structures and possible connections within that uncertainty. The [kinematic perspective](https://zmichels.github.io/decision-pga-pages/kinematics/) follows movement as evidence arrives and actions return results.

Within a run, we can examine how a lookup or verification step changes support for proceeding. Across comparable runs, we can investigate which patterns recur and which interventions consistently resolve them. Across product revisions, we can ask whether a change improves those outcomes or moves uncertainty elsewhere. Those comparisons require consistent candidate meanings and a record of what changed in the workflow.

For example, repeated mapping exceptions may appear to share one cause. Linked records reveal that some lack a source, while others remain ambiguous even with that source present. Decision-state observations help investigate those differences; evaluated outcomes establish whether a new lookup or check actually helps. The resulting lesson returns to the ledger, available for the next investigation and improvement.

Platforms support collection, review, and testing. The ledger design and geometric diagnostics add the workflow-specific interpretation described here; they are not automatic consequences of tracing. Stable decision support still needs correctness checks, and simpler measures may be sufficient. The aim is a useful, evolving map of decisions, their relationships, and the knowledge that makes them dependable.

## Give the project a memory of its own

The ledger also helps the people and agents building the product. Development accumulates context: why an approach was chosen, what failed, which constraint came from a stakeholder, and what still needs checking. Much of it lives in conversations and working sessions. Recording that context with its sources, status, and scope gives the project a durable memory that survives a closed chat or a change of team.

This is a practical way to offload context. A new collaborator can recover the reasoning behind a choice without reconstructing every conversation. A record might explain why a shortcut failed, link the test, and say when the decision should be revisited. Those records can travel with the project and contribute to organizational memory, while preserving where each lesson applies and what remains uncertain.

For learning, the ledger provides a form of external long-term memory. Capturing an experience makes it available for later use. Retrieving it, checking its relevance, and testing an improvement turn that memory into changed behavior. The record can support that work during development, inside the running product, or both.

A practical starting point is to give an agent the [articles](https://github.com/zmichels/decision-pga-pages) and [code and examples](https://github.com/zmichels/Decision-PGA), together with a specific goal. Ask it to consider what fits the work, explain its choices, and build the smallest useful record. A coding assistant can develop that record alongside the application as decisions emerge. The same approach can inform tools a running agent uses to consult history, add observations, and propose updates.

For example:

> Use these materials as inspiration. Design a ledger for the decisions and exceptions in this workflow. Keep the evidence, alternatives, outcomes, and links that serve that purpose. Leave room to examine finer details and connect them back to broader decisions. Explain which ideas you used, and suggest how lessons from future runs should be reviewed, tested, and incorporated.

The goal gives the record its shape. A project might begin with a simple exception ledger, then add smaller decision categories, relationships across stages, or diagnostics as they become useful. Compatible records can travel with context, instructions, and skills between agents and projects, carrying their source, scope, and history. Reusing an idea still requires checking whether it applies in the new setting.

Start before the long-term platform is chosen. A small collection of Markdown notes and structured JSON or CSV records can preserve decisions, evidence, corrections, and tested lessons during development. An existing project can begin by assembling that knowledge from its current artifacts, marking what is documented and what still needs confirmation. Give records stable identifiers, source links, and version history so the knowledge can grow with the product.

That early work can feed a larger platform later. For example, [Langfuse datasets](https://langfuse.com/docs/evaluation/experiments/datasets) accept examples through CSV upload or its SDK, including inputs, expected outputs, and metadata. Selected cases from a local knowledge base can become evaluation examples, while richer explanations and relationships remain in linked records. Moving between tools takes some mapping; portable records preserve the material that makes that work worthwhile.

Start now, with whatever fits the work. Capture what the team learns, then design how future runs will contribute and how proposed lessons will be tested. The platform can change. The knowledge should carry forward.

## Independence follows demonstrated performance

The product earns greater independence one kind of decision at a time. A user can retain review while evaluating an automated check, then delegate the cases it handles reliably. The capability to automate often arrives before the willingness to rely on it.

A person **in the loop** must participate for a case to proceed. A person **on the loop** supervises and can intervene. A person **out of the loop** does not participate in that piece of work. One product can contain all three arrangements.

Improvement moves the boundary where evidence supports it. Review unresolved cases and sample completed ones. Track incorrect outcomes as well as fewer interruptions. Restore review when conditions change. Required human authorization remains part of the process until that authority is explicitly delegated.

This is the trust standard to carry forward from deterministic automation: clear operating limits, observable results, tested changes, and dependable responses to failure. An adaptive system has to earn that confidence through its behavior.

## An MVP must demonstrate how it improves

For a product intended to evolve, the minimum viable product should complete one useful task and demonstrate one complete improvement cycle.

Consider a recurring field-mapping correction. The application preserves the source, the correction, and its scope. It proposes a rule, tests it on additional examples—including cases where it must not apply—and presents the results for approval. Later runs use the accepted rule while recording outcomes and retaining a way to reverse it.

That is a small but meaningful learning capability. The first release can limit change to one mapping table or one verification step. Broader powers, including integration repairs, come as the mechanism demonstrates reliability.

The deliverable includes an initial behavior, a tested way to improve it, and boundaries on what can change. Versioning and evaluation continue. We also test whether learning preserves what already works.

## Teaching belongs in everyday use

Agents gather context from documents, references, and tools. Local expertise supplies what those sources often leave implicit: which exception matters, which source takes precedence, and why a plausible answer misses the point.

People want better results without repeatedly stopping work to train a system. Make teaching easier. Capture corrections and successful recoveries. Ask focused questions when the reason is unclear. Preserve the scope of a lesson, and show people what their contribution changed. One person's preference does not automatically become everyone's rule.

This is shared work. An expert explains an exception. An engineer turns the explanation into a test. An agent helps investigate and implement a proposed improvement. Knowledge contributed during one difficult case becomes useful in the next.

The agency to learn magnifies the ambition of automation. It also touches a familiar science-fiction nerve: a machine changing what it can do. How much of our hesitation concerns the system, and how much concerns our confidence as its teachers and stewards?

We build that confidence through practice: recognize a bad lesson, demonstrate a useful change, and intervene when the system carries an idea too far. A product that learns asks us to become better teachers together.

The future looks wild. If we want the field to grow in intelligence, we need to be its teachers.
