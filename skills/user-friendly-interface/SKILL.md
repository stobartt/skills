---
name: user-friendly-interface
description: 'Research, design, improve, and review product interfaces: task flows, screen composition, interaction states, and adaptation across web, mobile, desktop, and other interactive products. Use for interface work alongside implementation or brand-design skills.'
license: MIT
---

# User-friendly interface

Start with what a person needs to accomplish. Make the situation understandable, the next action discoverable, and the result recognizable. Visual quality comes from a coherent composition and carefully resolved behavior, not from adding decoration to an unclear workflow.

This is an independent synthesis of product-design guidance. It supports judgment; it does not certify usability. Consult [sources](references/sources.md) when researching a decision or selecting a reference.

## 1. Establish the task, mode, and evidence

Choose the requested mode for each part of the task. Use the following sections to investigate, assess, propose, or implement accordingly.

| Mode | Deliverable and completion criterion |
| --- | --- |
| Research | Evidence answers the question, connects reference principles to the task, and identifies limits of transfer |
| Review | Findings cover the requested scope, with observed conditions, consequences, proposed corrections, and verification methods; unchecked behavior is identified and the product remains unchanged |
| Design | A proposed scenario, composition, and relevant states meet the stated constraints; assumptions and unresolved decisions are explicit |
| Implementation | The changed scenario works, the original problem is resolved, and affected states pass the applicable checks; remaining limitations are reported |

Identify the person, their goal, what they know, frequency of use, input method, environment, and successful outcome. Preserve established product constraints. For a small fix, investigate the affected interaction. Ask only about missing information that would materially change the decision, and label remaining assumptions.

When you can access the product, inspect the rendered interface and walk through the affected task. Capture the starting state when possible. During a review, use read-only interactions with live data. Exercise actions such as moving or deleting records only when their effects are confined to designated test data or an isolated copy. If only live data is available, report which transitions remain unverified.

With only screenshots or static mockups, assess visible composition and label behavioral conclusions as hypotheses. Use supplied flows or specifications for proposed behavior. Request additional access only when a required conclusion or change depends on it.

Interpret feedback through the underlying need. “Too empty” may mean disconnected controls; “too many lines” may mean competing boundaries. Distinguish the criticized variable—such as hue, lightness, saturation, area, or spacing—from a treatment the person wants to preserve. Establish the cause before proposing the smallest coherent correction within those constraints. Separate demonstrated defects from preferences.

## 2. Model the work before arranging components

State the scenario briefly: **person → situation → decision or action → necessary information → result**.

Distinguish the main workspace, its controls, supporting context, and global navigation. Every prominent section needs a role in this scenario. Merge duplication and remove sections that exist only to occupy space. Choose a structure suited to the work: comparison, exploration, editing, monitoring, or a sequence of decisions. Read [composition patterns](references/patterns.md) when choosing or changing that structure.

Choose references with comparable tasks, content volume, frequency, and devices. Borrow an explained principle, not an entire surface treatment. Reconcile findings into one visual and interaction language; do not assemble unrelated conventions from several admired products. Popularity and a polished screenshot are not evidence of suitability. Separate observed convenience from claims about retention: familiarity, social context, data, pricing, and switching costs may all affect continued use. Prefer mechanisms that reduce effort and support user control over mechanisms that create dependence. For each borrowed pattern, identify the task it serves, the mechanism that reduces effort, the conditions that make it suitable, and the interaction that will prove it works here. A reference list without this translation is not a design decision.

Before implementing a substantial change, state a short composition contract: the primary working area, the scope of its controls, the relationships that must stay aligned, and the states the change must preserve. Express these as observable outcomes, not adjectives such as “premium” or “polished.” Use this contract to compare the rendered result with the starting point.

## 3. Compose a coherent screen

Establish a clear entry point, main content, and next action. Keep labels, values, help, errors, and related actions together. Give each prominent region a task-level role, align meaningful edges, and use a consistent rhythm. Keep common actions discoverable while disclosing secondary complexity as needed.

Read the relevant sections of the composition guide when making or reviewing these decisions:

| Decision | Reference |
| --- | --- |
| Region widths, whitespace, density, and grouping controls | [Proportion and density](references/composition.md#proportion-and-density) |
| Containers, dividers, outlines, and floating layers | [Surfaces and boundaries](references/composition.md#surfaces-and-boundaries) |
| Palettes, themes, action emphasis, and workspace identity | [Color and identity](references/composition.md#color-and-identity) |
| Control shape, adjacent states, text metrics, and optical alignment | [Component geometry and states](references/composition.md#component-geometry-and-states) |
| Shared headers, content insets, and adjoining panes | [Composition seams](references/composition.md#composition-seams) |
| Equivalent tasks and the same object in different hosts | [Consistency across screens](references/composition.md#consistency-across-screens) |

## 4. Design the complete interaction

Label actions by their outcome. Distinguish navigation, opening options, selection, and immediate changes. Give different effects distinct visible cues: selecting an item and changing its state must be distinguishable before interaction, without relying on tooltips. Use state indicators for their actual meaning: the current location, a selected option, completed work, and unread content are different states. Do not add a completion-style checkmark to every highlighted navigation item. Prefer the lightest clear treatment, preserve accessible state, and check that the open content establishes the current context. Operating a nested control must not also activate its containing row or card. Make primary, secondary, and destructive actions clear within each task; “one primary button per entire screen” is not a universal rule.

Check an action against the current state: **when it is relevant → what changes → how the person recognizes the result**. A control that looks actionable must have a meaningful outcome. If its goal is already satisfied, show the current state or omit a redundant contextual shortcut. Keep a disabled action when its stable position or discoverability helps, and explain what enables it. A validation action may need to remain available so it can explain missing input. Choose among these treatments deliberately rather than hiding every unavailable command. When a control disappears after use, preserve focus and the position of neighboring targets. Check equivalent states, such as any date within the week already displayed, not just exact value equality.

Provide feedback near the action. Cover the states the scenario actually needs: first use, no data, no matches, loading, partial results, error, permission limits, saving, and success. Explain recovery, retain input, and preserve context on return. Confirmations should reflect consequences; routine reversible work should not accumulate unnecessary steps.

**State lifetime.** Define what happens to entered text, selection, filters, and reading position on dismissal, navigation, return, and application restart: what survives and what intentionally resets. Match persistence to the task and explain consequential loss before commitment. Saving a draft preserves unfinished work; applying or publishing makes it effective or shared. Keep these actions and their feedback distinguishable.

**State coherence.** Drafts belong to their conversation or object; changing a view changes representation, not the underlying records. After filtering, deleting, or moving an item, check the list, count, selection, detail pane, and available actions together. They must describe one coherent situation, including when the selected object leaves the current scope. Make recovery proportionate to consequences through undo, restore, or retained versions. Common actions should be discoverable before optional shortcuts accelerate them. Consult [familiar interaction patterns](references/patterns.md#familiar-interaction-patterns) when designing repeated operational work.

Keep the target under the pointer. Opening a menu, showing validation, or starting an operation must not unexpectedly displace its trigger. Motion should explain continuity without delaying an available action, including during closing or interrupted transitions. Respect reduced-motion preferences.

Give each bounded workspace a clear scrolling model. Keep ordinary reading in the primary flow; introduce independent scrolling only where it supports the task. Retain access to controls and context, make continuation discoverable, and provide enough inset at the end to read and operate the last item. Clipping a container must not make content or focus unreachable.

## 5. Adapt to people and environments

Preserve the task as available space changes. Base adaptation on the space left for the work after persistent navigation and supporting panes, not just the overall window. Reorder or sequence panels rather than shrinking the desktop composition. Retain selection, input, and return position. Check long content, localization, text enlargement, reading direction, safe areas, and the on-screen keyboard.

Account for applicable input methods: pointer, keyboard, touch, remote, voice, and assistive technology. Required actions cannot depend on hover alone. Provide recognizable focus, predictable traversal, adequate targets, and alternatives to color-only meaning. Give controls meaningful accessible names and appropriate roles. Expose their current state or value to assistive technology when applicable. Keep essential labels readable and provide an accessible way to reveal truncated values.

Use the target platform's accessibility requirements and conventions. Measure contrast for the actual adjacent colors and states. Necessary control boundaries and meaningful graphics have different requirements from decorative separators. Perceptually uniform color tools help tune a palette but do not establish readability or accessibility by themselves. Avoid arbitrary visual thresholds presented as scientific guarantees.

## 6. Verify against the requested mode

For a review or implementation handoff, read [the review guide](references/review.md) and select checks for the affected scenario. In a running product, walk through the task with representative content and relevant viewport, theme, and input variations. With static evidence, report visible findings and the interactions still requiring verification. Research and design work can finish with the evidence or proposal defined in the mode table; behavioral validation remains a separate requirement for claims about a working product.

For tasks that span navigation or dismissal, follow the [interruption and resumption checks](references/review.md#interruption-and-resumption) to verify state lifetime and the distinction between draft saving and applying changes.

Compare equivalent regions at the same scale; measure rendered alignment and dimensions when consistency is in question. Check shared components inside their actual hosts and inspect junctions between regions. A passing isolated component does not establish that the assembled screen preserves its geometry, hierarchy, or state. For implementation, fix causes at the responsible boundary and revisit affected uses.

Use the selected mode's completion criterion. Report remaining uncertainty and untested conditions. If an implementation cannot be exercised, identify the unverified outcome rather than claiming the original problem is resolved. Compilation, screenshots, and expert review answer different questions; observing representative users is necessary when actual usability needs to be established.

When maintaining this skill, use [evaluation cases](references/evaluation.md) to check its selection and execution. Keep transferable discoveries here and product-specific values and decisions in the product's documentation. Add guidance when it changes a decision or prevents a demonstrated failure, merging it with the existing principle.
