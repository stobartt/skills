---
name: brandbook-development
description: 'Research, design, create, update, and review brandbooks: identity rules, application examples, and usable assets adapted to each project. Use for documented brand systems, not standalone logo generation or routine UI tweaks.'
license: MIT
---

# Brandbook development

A brandbook turns identity decisions into guidance people can apply consistently. Connect intent, rules, examples, and deliverables so readers can choose an approach, produce material, and assess the result.

This skill provides the shared method and quality criteria. Keep each project's facts, visual choices, values, and exceptions in that project's documentation and assets. Adapt applications to their media within those decisions.

## 1. Establish the scope and mode

Choose the mode for each requested deliverable:

| Mode | Deliverable and completion criterion |
| --- | --- |
| Research | Findings answer the question, connect evidence to project decisions, and identify limits of transfer. |
| Design | Proposed identity decisions and representative applications answer the brief, explain tradeoffs, and distinguish proposals from established rules. Production assets are required only when included in the request. |
| Creation | The required guide and assets are delivered, observed defects are corrected, and applicable delivery checks support the claimed uses. Unverified conditions are identified. |
| Update | The requested decision and its affected rules, examples, values, and assets agree; applicable checks substantiate the change and unrelated brand decisions remain intact. |
| Review | Findings cover the requested scope with locations, observed problems, consequences, proposed corrections, and verification methods. Leave files unchanged unless edits are also requested. |

Distinguish the **guide's readers and tasks** from the **brand's audience and scope**. A general-purpose system with no narrow target audience is a valid scope. Guide readers still have concrete tasks, such as choosing a variant or applying a rule. Define audience segments or positioning only when they are part of the requested brand work.

For a new brandbook, substantial redesign, or unresolved scope, read [project context](references/project-context.md). For a narrow update, use the existing context and inspect only affected decisions. Record the **invariants** the request preserves, using available briefs, assets, code, tokens, and documentation before asking about material gaps.

Proceed when the deliverable, relevant applications, invariants, and unresolved dependencies are explicit enough to judge the result. Apply the remaining steps within that scope; in review mode, use them as assessment criteria.

## 2. Research principles and limits of transfer

Turn unresolved decisions into research questions. For a new or substantially revised brandbook, compare primary guides that address those questions and similar uses. Read the [source map](references/sources.md) when choosing references. For a small update, investigate the changed decision and its dependencies. Verify applicable technical and platform requirements against their current documentation.

Capture **source → observation → project decision → limit of applicability**. Compare how guides explain rules, distinguish variants, demonstrate misuse, provide files, and maintain current guidance. Derive the project's clear space, sizes, and container rules from its own geometry and uses; another brand's proportions or legal conditions belong to that brand.

Complete the research when each scoped question has a supported finding or an explicit evidence gap, and each recommendation states its basis and limits. Identify which decisions depend on missing evidence and continue independent work. Include direct source links in the chosen deliverable; save a research document when project documentation is in scope. For research-only work, hand off those findings here.

## 3. Define the rules readers need

Select areas by the decisions the guide must support. This is a menu of concerns, not a mandatory table of contents:

| Area | Decisions the guide should support |
| --- | --- |
| Brand foundation | Declared purpose and scope, supported characteristics, character, and limits of claims; positioning and audience distinctions when relevant |
| Logo and name | Variant selection, backgrounds, sizes, clear space, and combinations of symbol and wordmark; app icons may have separate rules |
| Color | Roles, permitted combinations, required color spaces, and applicable themes; distinguish identity colors from interface actions and semantic states |
| Typography | Families, weights, hierarchy, language coverage, fallbacks, and availability under the applicable font licenses |
| Voice and tone | A stable voice and changes of tone for specific reader situations, demonstrated with factual, useful examples |
| Applications | Real uses, correct examples, and explained errors, including constrained sizes or backgrounds |
| Assets and maintenance | Usable files, intended uses, decision status, the source of current guidance, responsibility for changes, and how changes propagate |

Include photography, illustration, motion, co-branding, or print processes when the task requires them. Link identity rules to existing design-system components and interactions where those already have an authoritative home.

Each rule should name its condition, the reader's action, and an observable example or check. Distinguish fixed requirements, recommended defaults, and permitted variations. Keep the rule beside its caveats and example. Complete this step when every required reader decision has guidance or a clearly identified unresolved dependency.

## 4. Prepare the guide and assets

When preparing or reviewing assets, read [asset preparation](references/delivery.md#asset-preparation). Preserve the invariants when deriving variants from established masters. Use a repeatable export for sizes and formats; reserve generation for a missing image or an intentional design change within the request.

When composing, implementing, or reviewing the guide, read [guide presentation](references/delivery.md#guide-presentation). Put frequent decisions near the entry point, and keep each example, explanation, and action together. Show the actual resources readers will receive.

Complete preparation when the required guide and files exist, variants are identifiable, and changed rules agree with their examples and resources. Unresolved decisions remain labeled as proposals or limitations.

## 5. Verify and hand off

Check **traceability: intent → rule → example → deliverable → target use** across the affected scope. For a delivery review or a creation/update handoff, apply the relevant [delivery checks](references/delivery.md#delivery-checks). For design work, assess representative applications against the brief and identify remaining decisions.

When validating whether readers can use the guide independently, follow the [reader handoff](references/delivery.md#reader-handoff).

Hand off the requested result: guide and asset locations, research or review findings, the source of current values, the update procedure, and material limitations. Keep change history according to repository conventions, separate from current usage guidance. Finish when the chosen mode's completion criterion is met.

When maintaining this skill, use [evaluation cases](references/evaluation.md) to check selection, scope, and transfer across projects. Add a general rule only when it changes a decision or prevents a demonstrated failure.
