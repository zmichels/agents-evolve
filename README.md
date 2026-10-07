# Agents evolve

**[Read the article: Automation as a product that learns](https://zmichels.github.io/agents-evolve/)**

An opinion article by Zachary D. Michels arguing for automation products that evolve through use and earn trust through tested improvements. RPA supplies the historical foundation and remains a practical part of hybrid delivery.

## Current state

The article source is [index.md](index.md), with an SVG improvement cycle in [assets/improvement-cycle.svg](assets/improvement-cycle.svg) and a [PNG preview](assets/improvement-cycle.png). It leads with learning through use as a production capability, using RPA and coding-agent observations as the practical inspiration and Decision-PGA as a diagnostic connection. Examples are generic and illustrative, with no internal project names. Langfuse is acknowledged as an existing platform for tracing and evaluation; the proposed ledger and decision-geometry layers remain distinct. HITL, HOTL, and human-out-of-the-loop execution are defined by scope.

## GitHub Pages foundation

GitHub Pages publishes from `main` at `/ (root)` in [zmichels/agents-evolve](https://github.com/zmichels/agents-evolve), using GitHub's standard Jekyll build. The custom layout and stylesheet follow the restrained reading style of the [Decision-PGA series](https://zmichels.github.io/decision-pga-pages/article/). `_config.yml` sets the project base path to `/agents-evolve`.

To update the article, edit `index.md`, update its `date_modified`, and push to `main`. Check the **pages build and deployment** run and verify the live article and diagram after it completes. `sitemap.xml` and `llms.txt` provide discovery links. The repository retains its original MIT license.

## Editorial direction

- The visualization connects execution within each run to knowledge and improvement across runs: record and link experience, map decision states, then propose and test changes. Its return path requires adoption within delegated authority. Keep labels brief and distinguish diagnostic patterns from demonstrated improvement.
- Lead with improvement cycling as a proposed production-delivery expectation. An evolving MVP should demonstrate one useful, bounded cycle. RPA supplies concrete inspiration within the broader story.
- Explain agents as a way to resolve some interpretation and recovery gaps within explicit limits.
- Distinguish evidence-based validation from model confidence or repeated agreement.
- Treat HOTL as process oversight that can contain individual HITL escalations.
- Frame human-out-of-the-loop execution as an ambition, with evidence and reversible delegation determining the scope.
- Present Decision-PGA articles, code, and examples as exploratory starting points. Adapt ledger designs to explicit workflow goals, with room for finer detail, links across scales, and evaluated updates; distinguish workflow learning from model retraining.
- Treat development ledgers as portable project and organizational memory in their own right. External long-term memory preserves context for future work; retrieval, review, and tested application make that context useful for learning.
- Keep examples hypothetical unless supported by an approved, attributable case study.
- Keep the public article free of internal project details. Retain the public Decision-PGA series links and the requested, source-backed Langfuse acknowledgment without making the argument vendor-dependent.

Potential follow-up articles: choosing between APIs, robots, and direct computer use; designing useful escalation packets; measuring escalation reduction without hiding errors.
