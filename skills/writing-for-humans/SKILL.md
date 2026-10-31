---
name: writing-for-humans
description: 'Write, edit, and review documentation and product copy, including presentations, pitches, emails, messages, and UI text. Not for AGENTS.md, CLAUDE.md, or skill instructions.'
license: MIT
---

# Writing for humans

This skill covers the content and wording of product text in any format. Adapt the writing to its medium: a slide, email, page, message, or interface. File formatting and delivery are separate tasks.

## Preparation

- Identify the audience, their knowledge, the context, the sender, and the format from the request and source material. Establish what the reader should understand, decide, or do. Proceed when the context is sufficient; ask only about gaps that would materially change the content.
- Follow the user's and project's requirements. Preserve the original language when editing unless translation is requested.
- Check factual claims against the available source material. For documentation, use code, configuration, and primary sources. For product copy, use evidence about capabilities, terms, and results. Figures, testimonials, customer references, and claimed benefits need evidence. Distinguish existing capabilities from plans and hypotheses.
- If an important claim cannot be verified, flag the gap in your response. A requested draft may include a clear verification note. Do not fill gaps with invented promises or facts.
- Preserve numbers, units, conditions, exceptions, causal relationships, and degrees of certainty when editing. Distinguish requirements, recommendations, and possibilities. Correct factual errors against a source and report them separately from style changes.

## Interpret, then compose

Treat the user's wording and source text as evidence of what they mean. Be faithful to the intended message, the facts, and explicit constraints; choose the phrasing and structure for the reader. Preserve exact wording when it is itself required, such as quotations, identifiers, interface labels, and agreed terminology.

Before drafting, state privately what the reader needs to understand and how the relevant facts connect. Resolve shorthand, figurative language, and implied relationships from the surrounding context. If plausible interpretations would change the substance, check the source or ask a focused question. Otherwise, use the ordinary contextual meaning.

Compose the passage from that understanding. Reorder facts, combine fragments, and explain a connection when it helps the reader follow the thought. For a request to rewrite or improve a passage, reassess the whole passage; a narrow correction can stay narrow. If the result merely substitutes synonyms while preserving a fragmented or confusing explanation, rewrite it again from its main point.

Exercise editorial judgment about precision. "The app remembers your settings" is a normal description of persistence; it needs no explanation that software has no human memory. Keep useful shorthand, familiar expressions, and the author's voice when readers will understand them correctly. Add a qualification where it prevents a credible misunderstanding that matters to this audience. Place implementation detail where it helps a decision or action. One explanation of a demo's scope can cover its screens.

Examples of applying this judgment:

| Context | Literal or mechanical treatment | Writing for the reader |
| --- | --- | --- |
| Saved document versions can be opened from History; explain why an editor would use it | "The product supports saved version selection." | "Open an earlier version in History to recover your work." |
| An import accepts valid rows and lets the reader correct and retry failed rows | "Import, validation, error display, and retry are available." | "Import your file. If some rows contain errors, correct them and try those rows again." |
| The user asks to shorten a warning; cancellation permanently discards the result | Shorten it to "Cancel?" | "Cancel and discard the result? This cannot be undone." |

Read the result as a whole: does it convey the intended message, make the relationships clear, and leave the reader with the right expectation or next step? Remove details that serve only to demonstrate the writer's technical accuracy. Keep material conditions close to the claim they qualify. Natural writing comes from a clear thought, an appropriate voice, and useful detail; forced informality or decorative personality adds no clarity.

## Meaning before wording

Check substantive claims in the intended context of the passage: who or what they describe, their scope and conditions, and the supporting evidence. Judge the understanding they give the reader, rather than isolated words stripped of context. This is a drafting check, not a template to expose to the reader.

- **Attribute properties to the right subject.** Product purpose, an example, a component, a repository, a deployment, and a delivery channel are different things. A browser-only demo does not make its design system a local-only product. Keep a qualifier when it genuinely defines the subject, as in a local development environment.
- **State the actual scope.** Qualifiers such as "local", "complete", "automatic", "secure", and "supported" need a clear referent. Identify what is stored, where it is stored, which operation is automatic, or which cases were verified. Avoid turning a component property or temporary limitation into a claim about the whole product.
- **Match outcomes to evidence.** An available capability, an initiated action, a completed action, and a confirmed user outcome require different wording. A queued request is not a delivered message; a successful component test does not establish product-wide reliability. Describe the mechanism or observed result when the broader benefit is unverified.
- **Keep examples and intentions recognizable.** Sample figures are not measured results, a prepared response is not live analysis, and a prototype action is not a working integration. Name the boundary where it changes what the reader should expect or do; avoid repeating implementation notes throughout an interface.

Use concrete wording instead of an ambiguous shortcut. These examples assume the stated behavior has been verified:

| Verified situation | Misleading shortcut | Accurate wording |
| --- | --- | --- |
| A reusable design system has a browser-only demo | "A local design system" | "A design system for product interfaces. Its demo runs in the browser." |
| Note files are encrypted; the editor decrypts them | "Text stays encrypted during editing" | "Note files remain encrypted on disk. The editor holds decrypted text in memory." |
| Large report responses are retained for paging | "Reports are not stored" | "Reports are fetched on request; large responses are stored temporarily for paging." |
| A prototype accepts a fixed verification code | "Code sent. Check your messages." | "Use the sample code 123456. This prototype does not send messages." |

Read the revision without the surrounding conversation. If a reasonable reader could infer a broader capability, guarantee, cause, or completion state than the evidence supports, narrow or split the sentence. When correcting a recurring claim, check related descriptions, instructions, UI messages, and summaries for the same mismatch. Search terms locate candidates; context determines whether a correction is needed.

## Product copy

Connect product capabilities to the reader's task: what changes for them and why it matters. Include technical details when they help the reader understand the offer, assess it, or make a decision. Preserve the author's or brand's voice; adapt the tone to the situation and the relationship with the reader.

Choose a structure that fits the format. These guidelines do not require separate headings or a fixed number of sections:

| Format | How to organize the text |
| --- | --- |
| Presentation | A sequence of takeaways for the audience. Give each slide a main point and supporting evidence; move detail to notes when the format supports them |
| Pitch or proposal | Who the product helps, which problem it solves, its value, supporting evidence, and the proposed next step |
| Email or message | The reason for writing and the main point first, followed by necessary context. Include a request, owner, and deadline when known and relevant |
| Product page or announcement | The offer or change, why it matters to the audience, availability, and material conditions |
| UI text or notification | A clear action or state. For an error, include the known cause and an available way to continue |

Include a request or call to action when there is an expected next step. An informational message can end with the information itself. Build persuasion through clear value, examples, and evidence. Superlatives, urgency, and guarantees need a factual basis.

## Documentation

Use the Diátaxis distinctions to choose what documentation should contain:

| Reader's need | Document type | Core content |
| --- | --- | --- |
| Learn through practice | Tutorial | A sequence of actions with observable results |
| Complete a specific task | How-to guide | Prerequisites, required actions, and a way to verify the result |
| Look up precise information | Reference | Parameters, values, and constraints in a consistent structure |
| Understand how and why | Explanation | Connections between concepts, reasons for decisions, and tradeoffs |

Separate these needs into sections within a short document. Use separate pages when they make information easier to find and use. Preserve the project's README structure and link to details. A small edit does not require reclassifying or restructuring the entire document.

## Language and formatting

Apply the clarity principles from the Google Developer Documentation Style Guide with the genre in mind:

- Make clear who performs an action. Passive voice is appropriate when the actor is unknown or irrelevant.
- Address the reader directly in instructions and start a step with an action: "Save the settings." Put conditions and locations before the instruction: "If the backup is complete, click **Delete**."
- Use numbered lists for sequences and bullets for independent items. Use tables when items share properties that readers need to compare. Keep connected explanations in paragraphs.
- Use informative headings and maintain their hierarchy where the format supports sections. Use one term for one concept; explain unfamiliar terms on first use.
- Format commands, paths, parameters, and literal values as `code`, and UI elements in **bold**. Preserve exact identifiers, quotations, and system messages.
- Make link destinations clear from the link text. Provide text descriptions for meaningful images; essential information must remain available without the image.
- Follow the grammar, punctuation, and locale conventions of the text's language and audience. Do not impose English abbreviations, Oxford commas, or US date formats on other languages. Use unambiguous dates such as "29 October 2026", or `29-10-2026` (DD-MM-YYYY) for audiences that use day-first dates.

## Editing

Apply the Microsoft Writing Style Guide principles while preserving accuracy and the author's voice:

- Lead with the main point or the action the reader needs to take. Remove openings that merely announce what the text will cover.
- **Bureaucratic language is unacceptable.** Replace it with direct words and actions: "perform a verification" → "verify", "for the purpose of improving" → "to improve", "a decision was made by us" → "we decided".
- Remove repetition, empty adjectives, and unsupported judgments. Shorten the text while preserving essential conditions, reasons, and constraints.
- Develop one idea per paragraph. Split long sentences when doing so preserves the relationships between their parts. Sentence length alone does not determine quality.

Example of shortening without changing meaning:

> Original: "It should be noted that retrying a request may result in a duplicate if the recipient does not support idempotency."
>
> Edited: "If the recipient does not support idempotency, retrying the request may create a duplicate."

Keep "may" and the condition: removing either would change the technical claim.

## Review and delivery

Do the work and check it yourself. Read the draft as its intended audience first, then verify the facts and refine the wording. If you have preserved the source's phrasing but lost its purpose, rewrite the passage before polishing sentences:

- Can the reader understand the point and its significance without context known only to the author? An email may refer to a shared conversation. If an action is expected, is it clear? Instructions must include necessary prerequisites and a way to verify the result.
- Are important conditions, exceptions, and distinctions between requirements and recommendations intact? Examples must match the described behavior.
- Are product promises and numerical claims supported? Capabilities, plans, and assumptions must be distinguishable; bureaucratic language must be removed.
- Do changed links and links to renamed sections work? Is each link's destination clear?
- Do the tone, length, and formatting fit the audience, channel, and request? Every remaining part must help the reader; shortening must preserve essential information.

Fix the problems you find. For a review request, identify the location, the specific issue, and a suggested revision. For writing or editing requests, deliver the finished text. Report significant factual corrections and unresolved gaps separately, when present. A short email or message needs only the text itself; keep commentary about your work out of the material intended for the reader.

## Sources and adaptation scope

- [Google Developer Documentation Style Guide — Highlights](https://developers.google.com/style/highlights): language, instructions, formatting, and accessibility. Google's material is published under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/); it is summarized and adapted here.
- [Diátaxis — Start here](https://diataxis.fr/start-here/), Daniele Procida: documentation types and reader needs.
- Microsoft Writing Style Guide: [Top 10 tips](https://learn.microsoft.com/en-us/style-guide/top-10-tips-style-voice) for clarity, organization, and editing; [Brand voice](https://learn.microsoft.com/en-us/style-guide/brand-voice-above-all-simple-human) for a consistent voice and tone suited to the situation.

This is an independent adaptation, not an official skill from the source authors. Google and Diátaxis provide the documentation foundation; their genre conventions do not automatically apply to pitches or correspondence. The guidance on product formats, claim verification, and review is specific to this skill. For a specific question not covered here, consult the relevant section of the primary source; there is no need to reread every guide for each task.
