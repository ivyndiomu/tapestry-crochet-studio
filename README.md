# Tapestry Crochet Studio

Tapestry Crochet Studio is a local-first product for turning artwork into gauge-aware, editable tapestry crochet patterns and carrying that work through garment placement, production and business workflow.

This public repository is a product-management and technical-product case-study repository. It is intentionally **not** the full commercial application source code.

## Why it exists

Custom tapestry crochet requires more than converting an image to pixels. A production-ready workflow must account for measured stitch and row gauge, colour reduction, manual correction, garment geometry, yarn availability, row direction, production progress, client approval, quoting and delivery.

The product began as an internal tool for a real crochet business and evolved through versioned releases as the workflow exposed new requirements.

## What this repository contains

- `docs/product-overview.md` - product vision, users, jobs and scope
- `docs/roadmap.md` - phased product roadmap and current validation direction
- `docs/architecture.md` - technical-product architecture decisions
- `docs/decisions.md` - key product trade-offs and decision record
- `docs/testing-strategy.md` - regression and release-quality approach
- `docs/research-and-metrics.md` - discovery plan, validation questions and metrics
- `docs/changelog.md` - selected product evolution notes
- `examples/sample-project.json` - a synthetic example of the project model
- `screenshots/README.md` - screenshot plan for public evidence

## Product principles

1. Crochet-aware first. Measured gauge controls physical proportions.
2. Manual correction is a first-class feature.
3. The garment is the design context, not an abstract grid.
4. The pattern grid is the source of truth for editing, instructions, production and export.
5. Core production stays local before cloud dependencies are introduced.
6. SaaS features are deferred until the single-user production workflow is validated.

## Current direction

The current focus is not feature volume. It is proving that the product reliably helps makers move from artwork to production-ready panels, complete real projects, and return for another project.

## Portfolio case study

The full product-management case study lives on Ivy's portfolio site. Add the public URL here after deployment.

## Source-code note

The commercial application source code is not included in this repository. Public documentation and screenshots are shared to demonstrate product thinking, technical decision quality and the evolution of the workflow without publishing the full product implementation.

© Ivy. Documentation and media are shared for portfolio viewing. No licence to the commercial application source code is granted by this repository.
