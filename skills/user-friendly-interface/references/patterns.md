# Choosing a composition

Read when selecting or changing a screen structure. These are starting models, not mandatory templates.

| Human task | Useful starting structure | Keep together | When to choose differently |
| --- | --- | --- | --- |
| Find or compare records | List or table | Collection identity, search, filters, creation, and selected-record actions | Cards suit visual recognition; retain comparable distinguishing information |
| Process a queue | List and detail | Selected item, content, local actions, and concise context | In narrow space, use a sequence with a reliable return to the same list position |
| Create or edit an object | Form with meaningful groups | Label, field, help, error, and resulting action | A long dependent process may need steps, review, and backward navigation |
| Configure a product | Sections organized by understandable topics | Setting, current value, and consequences | A few short settings do not each need a separate page |
| Monitor and respond | Status overview | Measure, period, unit, comparison, and associated action | A queue may be more useful than charts when decisions concern individual records |
| Edit a document or diagram | Workspace and contextual tools | Global commands, selected object, and its properties | Reading needs fewer persistent tools than editing |
| Choose content | Catalogue or feed | Name, distinguishing attributes, filters, and useful previews | Similar text records are often easier to compare in a list |
| Understand an offering | Explanation, evidence, and next step | What it is, who it helps, value, conditions, and action | Repeated operational work should not begin behind a promotional introduction |

## Collections and queues

The heading, controls, headers, and records should read as one working region. Use consistent column alignment and a distinguishable header treatment. A quiet separator can establish the transition into records without boxing every cell. Keep the header's meaning clear when scrolling. Sort direction, active filters, result count, and a way to clear conditions should be understandable.

Distinguish opening a record from selecting it for a batch action. If a row opens details, its useful area should respond consistently; nested actions remain independent. Provide an equivalent keyboard path. Make partial selection and batch scope explicit, especially across filtering or pagination. Preserve the connection between the selected item and its details.

A small collection can occupy a small region. A large collection needs comparison, retrieval, and return context. Introduce pagination, virtualization, or column controls for an actual volume or task constraint, not to imitate an enterprise product. No matches is different from having no records. Pagination supports bounded comparison and returning to a known position; incremental loading supports a continuous history or exploration. Show scope and progress, preserve reading position when inserting earlier content, and make the end recognizable. Filters and sorting apply to the entire relevant collection. Keep paging controls in a stable location when the last page is shorter; state whether batch selection covers the visible page or the full result set.

When filtering, deleting, or moving removes the selected record from the current scope, choose the resulting selection deliberately. Clear or move it and update the detail pane and actions, or make intentionally retained context outside the scope explicit. Counts and batch scope must describe that same result, including an empty list or a page that no longer exists. Apply the task's retention rules to filters, selection, and reading position when returning to the collection.

## Forms and settings

Order fields by how a person makes decisions, placing dependencies after their controlling choice. Start with a clear reading axis. Related short values may sit together; unrelated columns can create a confusing path. Fit field widths to expected values while accommodating localization and larger text.

Place actionable errors at the relevant field or group, preserve input, and make it possible to reach every error. Distinguish saved from unsaved work, automatic application from explicit submission, and reversible changes from consequential ones. Explain consequences before commitment. A multi-step process needs meaningful progress, review, and backward movement without data loss.

For staged edits, define whether cancellation discards current input, restores applied values, or retains a draft. Match the wording and feedback to that effect. Dismissing a form is a separate transition from applying its changes. In an autosaving form, make clear which edits become effective immediately and what recovery remains available.

For bulk operations, distinguish ready, invalid, skipped, and completed items. Keep a record in place while the person edits it, even if a correction changes its filter membership. Keep corrections attached to their records, state the scope before applying changes, and make partial success understandable. A retry processes unfinished work; it must not duplicate completed work or silently overwrite existing records.

## Workspaces and supporting panes

Separate tools from the object being edited. Choose the editing model from the task: frequent personal capture benefits from direct editing and automatic persistence; shared publication, restricted permissions, or consequential changes may warrant an explicit edit or publish step. Make editing discoverable without adding a mode switch to a surface whose primary purpose is writing. Distinguish a working draft, a saved object, and a published result when those stages exist. Match feedback to the actual persistence boundary and retain or reset work according to its intended lifetime. Keep focus recognizable without outlining an entire writing surface. A diagram needs free space for navigation and growth, but its initial framing should make nodes and relationships readable. Show the starting point and path; reveal object properties in context. Empty canvas area is not missing content.

For adjacent list and detail panes, use the [composition seams](composition.md#composition-seams) guidance to align their shared boundaries. On a narrow device, each pane becomes a complete step with a reliable return path.

In conversations, establish the person, topic or channel, and reply context. Give each contribution a recognizable author and readable grouping; use identity, spacing, alignment, and restrained surface treatment without making every speaker a competing colored panel. Prioritize information used to respond. Collapse secondary metadata, avoid repeated empty sections, and preserve access to full values. Choose message grouping from the conversation: a many-person discussion benefits from a consistent reading axis and replies attached to their source; a personal exchange may use incoming and outgoing alignment. Preserve author identity in both. Keep available message actions easy to discover while making existing reactions, replies, and saved state more prominent than unused actions. Retained drafts should also be recognizable from the conversation list. Short conversations can legitimately leave space. A supporting pane should have a stable boundary, clear dismissal when overlaid, and a readable final item when scrolled.

## Overviews and home screens

A working product answers “where do I continue?” or “what needs attention?” A pattern library helps choose an example. A public service explains an offer. These purposes need different starting screens. Combine repeated introductions into one useful heading and move the choice or continuation into the first viewport. A catalogue needs recognizable groups and distinguishing details; repeated logos, slogans, and oversized introductions should not push those choices away.

Use real or clearly identified sample data. Group measures by the decisions they support and supply context for interpretation. Do not fabricate urgency, trends, or activity to make a composition appear complete. An analytical view should connect an observation to a comparison and a useful next investigation. Keep the period, population, units, and definitions consistent across measures, charts, filters, detail views, and exports. A decorative trend beside unrelated live counts invites a false comparison.

## Layers and progressive disclosure

Use inline disclosure for nearby detail, a menu for a choice of actions, a popover for brief contextual work, and a dialog when focused attention or a distinct subtask warrants interruption. A larger page may be better for substantial editing or comparison. Pick the smallest surface that comfortably supports the task, not the smallest possible box.

The floating surface must remain distinguishable from its surroundings. Keep its anchor stable, padding sufficient, placement within available space, and focus and dismissal predictable. Preserve entered data where appropriate. Avoid stacking interruptions that obscure the original task.

## Adapting size and input

Use extra space for useful comparison or context. In smaller space, change panel order or sequence while retaining the selected object and return position. Ensure that essential actions remain reachable with the on-screen keyboard open.

A remote needs visible focus and predictable travel between regions; touch needs adequate targets; a keyboard needs a coherent traversal order; voice needs recognizable options and correction. Follow platform conventions rather than imitating mouse hover where no hover exists.

## Familiar interaction patterns

Use these mechanisms when the task calls for them. Preserve the causal relationship, not a reference product's branding or exact control placement.

| Situation | Mechanism worth transferring | Check before using it |
| --- | --- | --- |
| Many conversations | Stable channel or person context, replies attached to their original message, separate drafts | Switching conversations must neither send nor replace another draft; a saved result must lead back to its source |
| Processing correspondence | Folder or queue scope, readable list–detail relationship, explicit recipient, recoverable archive or removal | Sending and replying need a clear destination; selecting, reading, and bulk actions must stay distinct |
| Repeated document work | Direct editing, quiet content surface, contextual formatting, understandable save status, outline, named recovery points | Restoring an earlier version must not silently erase the only copy of later work; a save label must reflect persistence |
| Multiple views of work | List, board, calendar, or overview as views of the same objects | Editing an object in one view must be reflected in the others; switching layout should preserve meaningful filters and selection |
| Finding prior material | Search with an explicit scope, recognizable previews, stable location and return path | Search this folder and search everything are different promises; a no-match state needs a way to broaden or clear conditions |
| File organization | Breadcrumbs, recognizable object actions, batch selection, reversible trash | Prevent impossible moves and cycles; preserve children when restoring a folder; explain partial failure |
| Frequent use | Visible commands plus familiar shortcuts and remembered context | A shortcut supplements discovery; platform conventions and assistive technology take precedence over novelty |

Use consistent controls within these structures: collection title and creation in the header; search, filters, count, and batch scope next to the collection; object actions next to the selected object. This is a relationship model, not a universal pixel layout. On smaller screens, sequence panels while keeping the same work and a reliable return path.
