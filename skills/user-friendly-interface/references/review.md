# Reviewing composition and interaction

Use for a review or before handing off an interface change. Select checks relevant to the scenario; this is not an obligatory full audit for every edit.

## Look for observable evidence

| Question | Useful evidence | Failure signal |
| --- | --- | --- |
| Is the task understandable? | The object, state, scope, and next action are identifiable | A generic slogan displaces useful material; controls require guesswork |
| Does hierarchy support the task? | Necessary information is easy to locate and related elements form clear groups | Equal emphasis everywhere, disconnected labels, unrelated regions appearing to be one control |
| Are proportions purposeful? | Width supports reading, comparison, entry, or manipulation | A short value spans the monitor; a related control wraps alone despite sufficient usable width; an empty container dominates without a working purpose |
| Are surfaces distinguishable? | The collection, header, selected object, and floating layers retain clear roles | A header merges with the page; a menu disappears into its background; nested containers repeat one role and multiply padding; indiscriminate neutralization erases meaningful differences |
| Do equivalent tasks behave alike? | Side-by-side comparison of names, placement, scope, state and feedback | The same collection search or batch action becomes a new pattern on each screen |
| Do adjoining regions form one composition? | Equivalent headers share an alignment rule; boundaries meet intentionally without doubled strokes | Independent bars create a stepped divider; equal outer padding hides unequal content heights |
| Are component states coherent? | Layout bounds and painted silhouettes, text metrics, icon slots, optical alignment, and behavior remain consistent | A label widens on selection, mixed icons shift text, hover creates a new contour, nested corners disagree with their inset, neighboring state fills merge, an open or close control loses its normal shape, or selected plus hover loses meaning |
| Does each action fit the current state? | Its prerequisite, effect, and resulting feedback are clear | An active control silently repeats the current state; dismissal loses focus; a retry repeats completed work |
| Is interaction stable? | The trigger stays in place, feedback arrives promptly, dismissal restores context | A target jumps, an animation stalls, focus disappears, closing content flashes |
| Can the person recover? | The cause, correction, and retained input are visible | Generic error, lost work, or a dead end |
| Does state survive for the intended lifetime? | Text, selection, filters, and reading position are retained or reset as specified after dismissal, navigation, return, and restart | A lost draft, stale selection, or feedback that confuses draft saving with applying changes |
| Does the screen describe one situation? | List, count, selection, details, and actions agree after filtering or after moving or deleting a test record | Details or actions silently target an object outside the current scope, or the count contradicts the list |
| Is overflow intentional? | The last item, focused control, and full important values are reachable | Clipped content with no clear continuation, competing scroll regions, an inaccessible footer |
| Does adaptation preserve the task? | Relevant themes, narrower windows, larger text, and input methods reach the same outcome | Missing functions, overlapping panels, illegible values, keyboard traps |
| Can assistive technology identify each affected control? | Inspect its name, role, and applicable state or value in the platform's accessibility tree. Check the exposed state or value again after it changes. | An icon-only button has no accessible name, or a switch shown as on exposes the off state |

Inspect combined states where they can conflict: selected and hovered, adjacent keyboard focus, invalid and focused, loading after submission, menu-to-dialog handoff, and closing during navigation. Check surfaces against their actual neighbors, text and icons at the intended viewing scale, and content against its intended container. Two regions that expanded together can conceal overflow. For a changed palette or boundary, revisit the affected grouping, state, and layer in the rendered result; compare wrapped labels and enlarged text where alignment matters. Use the relevant [composition guidance](composition.md) to diagnose the observed relationship.

## Interruption and resumption

Start a task, leave for another section, return, and continue. Check Escape, window closure, explicit cancellation, and restart separately where applicable. Observe retained input, selection, filters, reading position, committed changes, and restored focus against the intended state lifetime. Saving an unfinished draft must remain distinguishable from applying changes. Check rapid repetition and interruption during opening, closing, and pending operations.

## Findings and coverage

For each finding, record the observed state, consequence, proposed correction, and how to verify it. Prioritize task blockers and misleading behavior over decorative polish. A whitespace finding needs an identified broken relationship or missing function. Report checks that could not be performed; visible evidence supports visible findings, while unobserved behavior remains unverified.
