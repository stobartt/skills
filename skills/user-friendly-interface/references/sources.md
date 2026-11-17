# Sources and visual references

Reviewed November 1, 2026. This is an independent synthesis, not a skill issued or endorsed by these organizations. Guidance is paraphrased; source text and visual examples remain with their authors. Recheck the relevant primary source when platform guidance or a measurable requirement matters.

## Principles and their scope

| Primary source | Principle to apply | Limit of transfer |
| --- | --- | --- |
| [Nielsen Norman Group: Ten usability heuristics](https://www.nngroup.com/articles/ten-usability-heuristics/) | Understandable status, familiar language, control, recognition, error prevention and recovery | Heuristics guide evaluation; they do not prove a particular product is usable |
| [NN/g: Proximity](https://www.nngroup.com/articles/gestalt-proximity/) | Distance communicates relationships | More space can weaken a relationship; it is not always better |
| [NN/g: Progressive disclosure](https://www.nngroup.com/articles/progressive-disclosure/) | Reveal secondary complexity when needed | Frequent and necessary actions must remain discoverable |
| [Fluent 2: Layout](https://fluent2.microsoft.design/layout) | Meaningful space, shared alignment, flexible grids, and consistent rhythm | The Fluent spacing scale is one system's convention, not a universal requirement |
| [Fluent 2: Color](https://fluent2.microsoft.design/color) | Separate neutral, product-identity, and semantic palettes; carry identity through purposeful accent locations | Product recognition does not justify tinting every surface or changing the meaning of feedback colors |
| [Fluent 2: Shapes](https://fluent2.microsoft.design/shapes/) and [Material Web: Buttons](https://material-web.dev/components/button/) | Choose form by role and scale; resolve nested and joined contours as relationships | A product’s radius scale or capsule treatment is not a requirement for every platform or control |
| [Fluent 2: Divider](https://fluent2.microsoft.design/components/web/react/core/divider/usage) | Combine boundaries with spacing and headings to make content groups understandable | A divider needs a grouping purpose; placing one between every item adds noise |
| [Fluent 2: Elevation](https://fluent2.microsoft.design/elevation) | Depth communicates layers through coordinated surface and shadow treatment | A shadow is not a substitute for every boundary; platform treatment differs |
| [Atlassian: Spacing](https://atlassian.design/foundations/spacing) | Within-group and between-group spacing serve different roles | Inherit or define one product scale instead of mixing unrelated scales |
| [Apple HIG: Layout](https://developer.apple.com/design/human-interface-guidelines/layout), [Boxes](https://developer.apple.com/design/human-interface-guidelines/boxes), and [Toolbars](https://developer.apple.com/design/human-interface-guidelines/toolbars) | Group with alignment and spacing; use containers for distinct groups and organize tools by their task | Nested framing can crowd content; platform materials and toolbar placement are not universal styling rules |
| [GOV.UK: Text input](https://design-system.service.gov.uk/components/text-input/) | Visible labels and input widths suited to expected content | A public-service flow does not dictate the density of a professional editor |
| [Carbon: Empty states](https://www.carbondesignsystem.com/building-blocks/core/patterns/empty-states) | Distinguish first use, no matches, and a problem; provide an appropriate next step | An empty state does not automatically need an illustration or a separate page |

## Examples worth inspecting

- [Material: Canonical layouts](https://m3.material.io/foundations/layout/canonical-examples/overview) and [Android: Adaptive canonical layouts](https://developer.android.com/develop/ui/compose/layouts/adaptive/canonical-layouts): compare feed, list-detail, and supporting-pane relationships and how they adapt. These are task models, not three mandatory screens or a required implementation stack.
- [Cloudscape: Table view](https://cloudscape.design/patterns/resource-management/view/table-view/) and its [working example](https://cloudscape.design/examples/react/table.html): inspect how collection identity, actions, retrieval, and records form one working region. The extensive controls address large resource collections; small collections need fewer.
- [Carbon: Data table](https://www.carbondesignsystem.com/building-blocks/core/components/data-table/guidelines): inspect header treatment, row rhythm, toolbar placement, sorting, selection, and batch actions. Preserve the functional relationships without copying Carbon's dimensions or colors into another system.
- [Apple HIG: Materials](https://developer.apple.com/design/human-interface-guidelines/materials): inspect how layers separate controls and content. Translucency and Liquid Glass are platform-specific choices; apply the hierarchy principle rather than making every surface transparent.

- [Cloudscape: Wizard](https://cloudscape.design/components/wizard/): inspect dependent steps, validation, review, and return without losing input. A short independent form does not need a wizard; persisted drafts may make a discard warning unnecessary.
- [IBM Design Language: Data visualization](https://www.ibm.com/design/language/data-visualization/design/basics/): use interaction to reveal context and support interpretation. A chart is useful for a comparison or investigation, not simply because a dashboard needs visual variety.
- [NN/g: Contextual menus](https://www.nngroup.com/articles/contextual-menus/): relevant commands and stable, discoverable options reduce guessing. The advice to retain disabled menu items is scoped to menus; it does not require retaining every redundant contextual shortcut.

- [Fluent 2: Cards](https://fluent2.microsoft.design/components/web/react/core/card/usage/) and [Avatars](https://fluent2.microsoft.design/components/web/react/core/avatar/usage/): inspect information slots, distinct object actions, and the stable visual identity of people and groups. The transferable lesson is to preserve a component's meaning and anatomy inside its host; component names, dimensions, and framework APIs remain implementation choices.

## Established interaction patterns

The sources below document product behavior. They do not establish that a particular feature causes retention. Assess the mechanism against the person's task and validate the resulting interface.

| Primary source | Transferable mechanism | Boundary |
| --- | --- | --- |
| [NN/g: Consistency and standards](https://www.nngroup.com/articles/consistency-and-standards/) and [Mental models](https://www.nngroup.com/articles/mental-models/) | Internal consistency and established expectations reduce relearning | Familiarity does not require identical styling or ignoring the target platform |
| [Slack: Threads](https://slack.com/help/articles/115000769927-Use-threads-to-organize-discussions) and [Saved messages](https://slack.com/help/articles/360042650274-Save-messages-and-files-for-later) | Replies and saved items preserve their source context | Product navigation changes; retain the relationship rather than hardcoding old menu names |
| [Telegram: Drafts](https://telegram.org/blog/drafts) | An interrupted draft remains attached to its conversation and visible in the list | This source introduced the behavior in 2016; it is evidence for continuity, not for a current visual layout or a requirement to reorder every list |
| [Google Docs: Product examples](https://workspace.google.com/products/docs/) and [Version history](https://support.google.com/docs/answer/190843?hl=en) | Named versions and restoration support iterative work | Revision history, collaboration, and synchronization are separate capabilities; recovery is limited to retained versions |
| [Apple Notes: Create and edit](https://support.apple.com/en-gb/guide/notes/not9474646a9/mac) | Personal capture starts in the content; editing does not require a separate read-mode command | Publication workflows and restricted documents can need a different commitment model |
| [Apple Mail: Write and send](https://support.apple.com/en-by/guide/mail/mlhlp1098/mac) | Clear recipient, composition, and a chance to undo sending | Cancelling a pending send and recalling an already delivered message have different guarantees |
| [Todoist: Filters](https://www.todoist.com/help/todoist/features/introduction-to-filters-V98wIH) and [Board layout](https://www.todoist.com/help/todoist/features/use-the-board-layout-in-todoist-AiAVsyEI) | Different views and scopes operate on shared task objects | Multiple views earn their cost only when they support different decisions |
| [Apple Finder: Tags](https://support.apple.com/en-gb/guide/mac-help/mchlp15236/27/mac/27) | A file can be retrieved through meaningful attributes as well as location | Additional organization systems need a clear role; folders, favorites and tags are not automatically all necessary |
| [Notion: Links and backlinks](https://www.notion.com/en-gb/help/guides/creating-links-and-backlinks) | Related knowledge retains navigable context | Links should connect useful work rather than add decorative relationship panels |

- [Carbon: Pagination](https://www.carbondesignsystem.com/building-blocks/core/components/pagination/specifications) and [NN/g: Infinite scrolling](https://www.nngroup.com/articles/infinite-scrolling-tips/): compare bounded navigation with continuous exploration and explicit incremental loading. Pick by the retrieval and return task, not a rule that every collection needs pages or infinite scroll.
- [Slack: Message display](https://slack.com/help/articles/213893898-Change-how-messages-are-displayed): inspect the relationship between author identity, grouping, and reading density. A preference offered by one product is not a requirement to expose the same setting elsewhere.

## Accessibility and color

- Check that web controls expose their name, role, and applicable state or value, including changes after interaction. [WCAG 2.2, Name, Role, Value](https://www.w3.org/WAI/WCAG22/Understanding/name-role-value.html)
- [WCAG 2.2: Contrast minimum](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html): evaluate text against its actual background. Size and weight affect the applicable threshold; text contrast alone does not establish full accessibility.
- [WCAG 2.2: Non-text contrast](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html): necessary visual information that identifies a control, state, or graphic requires adequate contrast against adjacent colors. This does not require a high-contrast border around every card, button, or decorative separator.
- [WCAG 2.2: Target size minimum](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html) and [Reflow](https://www.w3.org/WAI/WCAG22/Understanding/reflow.html): use the actual criteria, scope, and exceptions. Web CSS-pixel requirements should not be copied blindly into television, native-mobile, or other platform units.
- [W3C CSS Color 4: OKLab and OKLCH](https://www.w3.org/TR/css-color-4/#ok-lab): perceptually organized lightness and chroma help reason about color scales and interpolation. They do not guarantee WCAG contrast or appearance outside the display gamut. Choose a color representation for the work it enables; merely rewriting an existing palette changes no design decision.

The skill is independent of a component library, framework, or platform. Consult the target platform's current guidance for specialized input, accessibility, and safety constraints.
