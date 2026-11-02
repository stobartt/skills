---
name: writing-for-humans
description: 'Write, edit, and review documentation and product copy, including presentations, pitches, emails, messages, and UI text. Not for AGENTS.md, CLAUDE.md, or skill instructions.'
license: MIT
---

# Writing for humans

This skill covers the content and wording of product text in any format. Adapt the writing to its medium: a slide, email, page, message, or interface. File formatting and delivery are separate tasks.

## 1. Establish the scope and reader

Choose the requested mode before working on the text:

| Mode | Result |
| --- | --- |
| Writing or editing | Finished text that serves the reader's purpose and respects the supplied facts and constraints |
| Review | Findings with a location, a specific issue, and a suggested revision; leave the source unchanged unless edits are also requested |

Identify the audience, their knowledge, the context, the sender, and the format from the request and source material. Establish what the reader should understand, decide, or do. Ask only about gaps that would materially change the content. Preserve the original language when editing unless translation is requested.

Proceed when the mode, intended takeaway or action, and relevant constraints are clear enough to assess the text. A narrow correction needs only the context that can affect it.

## 2. Interpret and verify the message

State privately what the reader needs to understand and how the relevant facts connect. Resolve shorthand, figurative language, and implied relationships from the surrounding context. If plausible interpretations would change the substance, check the source or ask a focused question. Otherwise, use the ordinary contextual meaning.

Check material claims against available evidence. For documentation, use code, configuration, and primary sources. For product copy, use evidence about capabilities, terms, and results. Figures, testimonials, customer references, and claimed benefits need support.

- **Subject and scope.** Identify who or what a claim describes and under which conditions. Product purpose, an example, a component, a repository, a deployment, and a delivery channel are different subjects. Qualifiers such as "local", "complete", "automatic", "secure", and "supported" need a clear referent.
- **Evidence and certainty.** Distinguish a capability, an initiated action, a completed action, and a confirmed user outcome. Describe the mechanism or observed result when a broader benefit is unverified. A successful component test does not establish product-wide reliability.
- **Facts and constraints.** Preserve numbers, units, conditions, exceptions, causal relationships, and degrees of certainty. Keep requirements, recommendations, and possibilities distinct. Base factual corrections on a source and distinguish them from style suggestions.
- **Examples and intentions.** Keep sample figures, plans, hypotheses, and prototype behavior recognizable as such. Explain their boundary where it changes what the reader should expect or do. One explanation of a demo's scope can cover its screens.

These examples assume the stated behavior has been verified:

| Verified situation | Misleading shortcut | Accurate wording |
| --- | --- | --- |
| A reusable design system has a browser-only demo | "A local design system" | "A design system for product interfaces. Its demo runs in the browser." |
| Note files are encrypted; the editor decrypts them | "Text stays encrypted during editing" | "Note files remain encrypted on disk. The editor holds decrypted text in memory." |
| Large report responses are retained for paging | "Reports are not stored" | "Reports are fetched on request; large responses are stored temporarily for paging." |
| A prototype accepts a fixed verification code | "Code sent. Check your messages." | "Use the sample code 123456. This prototype does not send messages." |

Proceed with supported claims and explicitly identified gaps. Flag an important claim that cannot be verified; a requested draft may include a clear verification note. When a mismatch recurs, check related descriptions, instructions, UI messages, and summaries within the requested scope. Search terms locate candidates; context determines whether a correction is needed.

## 3. Compose for the reader

For writing and editing, compose from the verified understanding. For review, use these principles to assess the text and develop suggested revisions.

Choose phrasing and structure that make the relationships clear. Reorder facts, combine fragments, and explain a connection when it helps the reader follow the thought. Reassess the whole passage when asked to rewrite or improve it; a narrow correction can stay narrow. If a revision merely substitutes synonyms while retaining a fragmented explanation, rebuild it from its main point. Preserve exact wording when it is required, such as quotations, identifiers, interface labels, and agreed terminology.

Exercise editorial judgment about precision. "The app remembers your settings" is a normal description of persistence; it needs no explanation that software has no human memory. Keep useful shorthand, familiar expressions, and the author's or brand's voice. Add qualifications where they prevent a credible misunderstanding that matters to the audience, and keep material conditions close to their claim. Include implementation detail when it helps the reader understand, decide, or act.

| Context | Literal or mechanical treatment | Writing for the reader |
| --- | --- | --- |
| Saved document versions can be opened from History; explain why an editor would use it | "The product supports saved version selection." | "Open an earlier version in History to recover your work." |
| An import accepts valid rows and lets the reader correct and retry failed rows | "Import, validation, error display, and retry are available." | "Import your file. If some rows contain errors, correct them and try those rows again." |
| The user asks to shorten a warning; cancellation permanently discards the result | Shorten it to "Cancel?" | "Cancel and discard the result? This cannot be undone." |

### Product copy

Connect capabilities to the reader's task: what changes for them and why it matters. Adapt the tone to the situation and relationship. Choose a structure suited to the format; these guidelines do not require separate headings or a fixed number of sections.

| Format | How to organize the text |
| --- | --- |
| Presentation | A sequence of takeaways. Give each slide a main point and supporting evidence; move detail to notes when the format supports them |
| Pitch or proposal | Who the product helps, which problem it solves, its value, supporting evidence, and the proposed next step |
| Email or message | The reason for writing and the main point first, followed by necessary context. Include a request, owner, and deadline when known and relevant |
| Product page or announcement | The offer or change, why it matters to the audience, availability, and material conditions |
| UI text or notification | A clear action or state. For an error, include the known cause and an available way to continue |

Include a call to action when a next step is expected; an informational message can end with the information itself. Build persuasion through clear value, examples, and evidence. Superlatives, urgency, and guarantees need the same support as other factual claims.

### Documentation

Use the Diátaxis distinctions to choose what documentation should contain:

| Reader's need | Document type | Core content |
| --- | --- | --- |
| Learn through practice | Tutorial | A sequence of actions with observable results |
| Complete a specific task | How-to guide | Prerequisites, required actions, and a way to verify the result |
| Look up precise information | Reference | Parameters, values, and constraints in a consistent structure |
| Understand how and why | Explanation | Connections between concepts, reasons for decisions, and tradeoffs |

Separate these needs into sections within a short document. Use separate pages when they make information easier to find and use. Preserve the project's README structure and link to details. A small edit does not require reclassifying or restructuring the entire document.

### Language and editing

Apply the clarity principles from the Google Developer Documentation Style Guide and Microsoft Writing Style Guide with the genre in mind:

- Lead with the main point or action. Develop one idea per paragraph and retain the connections between sentences. Remove openings that merely announce what the text will cover.
- Replace bureaucratic language with direct words and actions: "perform a verification" → "verify", "for the purpose of improving" → "to improve", "a decision was made by us" → "we decided".
- Remove repetition, empty adjectives, and unsupported judgments. Shorten while preserving essential conditions, reasons, and constraints. Sentence length alone does not determine quality.
- Make clear who performs an action. Passive voice is appropriate when the actor is unknown or irrelevant.
- Address the reader directly in instructions and start a step with an action: "Save the settings." Put conditions and locations before the instruction: "If the backup is complete, click **Delete**."
- Use numbered lists for sequences and bullets for independent items. Use tables for comparisons and paragraphs for connected explanations. Maintain informative headings where the format supports sections.
- Use one term for one concept; explain unfamiliar terms on first use. Format commands, paths, parameters, and literal values as `code`, and UI elements in **bold**.
- Make link destinations clear from the link text. Provide text descriptions for meaningful images; essential information must remain available without the image.
- Follow the grammar, punctuation, and locale conventions of the text's language and audience. Use unambiguous dates such as "29 October 2026", or `29-10-2026` (DD-MM-YYYY) for audiences that use day-first dates.

Example of shortening without changing meaning:

> Original: "It should be noted that retrying a request may result in a duplicate if the recipient does not support idempotency."
>
> Edited: "If the recipient does not support idempotency, retrying the request may create a duplicate."

Keep "may" and the condition: removing either would change the technical claim.

## 4. Check and deliver

Read the text with only the context available to its intended audience. An email may rely on a shared conversation; standalone documentation must supply its own context. Check these completion criteria within the requested scope:

- The point, its significance, and any expected next action are clear. Instructions include necessary prerequisites and a way to verify the result.
- Material claims satisfy the subject, scope, evidence, and certainty checks above. Examples match the described behavior, and unresolved factual gaps are explicit.
- The tone, length, and formatting fit the audience and channel. Every remaining part helps the reader; essential meaning survives shortening.
- Changed links and links to renamed sections resolve to their intended destinations.

For writing and editing, correct remaining problems before delivering the finished text. For review, tie each finding to evidence and a usable revision, and report limitations on what could be checked. Deliver the result for the selected mode. Keep significant factual corrections and unresolved gaps outside the reader-facing material; a short email or message needs only its text when no such notes are necessary.

## Sources and adaptation scope

- [Google Developer Documentation Style Guide — Highlights](https://developers.google.com/style/highlights): language, instructions, formatting, and accessibility. Google's material is published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); it is summarized and adapted here.
- [Diátaxis — Start here](https://diataxis.fr/start-here/), Daniele Procida: documentation types and reader needs.
- Microsoft Writing Style Guide: [Top 10 tips](https://learn.microsoft.com/en-us/style-guide/top-10-tips-style-voice) for clarity, organization, and editing; [Brand voice](https://learn.microsoft.com/en-us/style-guide/brand-voice-above-all-simple-human) for a consistent voice and tone suited to the situation.

This is an independent adaptation, not an official skill from the source authors. Google and Diátaxis provide the documentation foundation; their genre conventions do not automatically apply to pitches or correspondence. The guidance on product formats, claim verification, and review is specific to this skill. For a specific question not covered here, consult the relevant section of the primary source; there is no need to reread every guide for each task.
