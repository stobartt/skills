# Brandbook delivery

Use the sections relevant to the requested assets and publication medium. During a review, assess the available evidence and identify checks that require access to the working guide or source files.

## Asset preparation

Preserve editable sources where available. Select output formats by content and intended use:

| Asset or use | Preparation decisions |
| --- | --- |
| Vector logo | Deliver vector artwork and its editable source. Keep native SVG shapes such as circles and rectangles unless the brief or output format calls for paths. For vector-only delivery, check previews and downloads for raster content, including embedded bitmaps. |
| Raster relief, light, or texture | Retain a lossless master and required transparency. Export the requested web formats with enough resolution for target display density. |
| Favicon | Select formats and dimensions supported by the target browsers. The guide's image format and the browser icon's format can differ. |
| Installation, PWA, or store icon | Consult the target platform's current requirements for shape, safe area, background, dimensions, and transparency. |
| Print | Use the agreed production process, color profile, dimensions, and printer specifications. Treat missing production values as unresolved; HEX alone does not determine a unique CMYK or Pantone equivalent. |

Measure clear space from the edges specified for that logo variant in the brand's approved guide or annotated master. Account for any exclusions, such as a trademark symbol, and any clear space built into the file. When developing a new rule, choose a reference edge, such as the visible contour, and test the proposed spacing in a representative application. Use the same geometry for dimensioned diagrams and label schematic illustrations as such. For symbol-and-name combinations, define the relevant size relationship, spacing, alignment, and permitted arrangements in the project's units.

Establish minimum sizes by inspecting the actual mark on its intended surface and show the claimed boundary size among the examples. Give delivered variants, including monochrome versions when present, a visible selection rule and representative use. Compare applicable theme variants side by side: each needs appropriate optical weight and contrast, which simple dimming or inversion may not preserve.

For transparency and compression, inspect the alpha channel, ordinary compositing on representative backgrounds, edges, internal openings, and color at the intended size. Confirm whether a visible defect belongs to the file or its preview before altering the master. File size alone does not establish export quality.

Use project tokens and file metadata as sources of truth where available. Give each asset a distinguishable filename and state its use, theme or background, format, and dimensions. For recurring updates, derive the catalog from those sources and use repeatable exports with integrity checks. A one-off package can use a documented manual export.

Confirm permission to redistribute included third-party assets and font files; reference restricted resources through their authorized source instead.

## Guide presentation

Make variant comparison, selection rules, and downloads easy to find. On a long web page, provide a table of contents and direct section links. Label intentional misuse in words as well as visually. Keep demonstrations of light and dark variants local to their examples unless the reader explicitly changes the product theme.

For a web guide, use semantic headings, keyboard access, visible focus, readable line lengths, and layouts that work on narrow screens. Give a standalone brand image an accessible name; an image beside the same brand name may be decorative. Report copying success only after the operation succeeds, and leave the value available for manual copying on failure.

Check contrast between the actual adjacent colors. WCAG's exception for logo text does not extend to ordinary guide text or controls. A ratio for one flat color pair does not assess a multitone image or certify the whole guide.

For PDF or other document delivery, keep navigation, examples, and file references usable in the delivered format. Inspect the rendered document rather than inferring layout quality from its source.

## Delivery checks

Select checks by the affected scope and medium. Correct observed defects within the authorized work and repeat the affected checks; identify outcomes that available evidence cannot establish.

| Area | Observable evidence |
| --- | --- |
| Files and package | Open each affected deliverable; confirm its actual format, dimensions, transparency, and agreement with the master. Inspect archive contents separately from the link to the archive. |
| Real use | Inspect the mark at its claimed minimum size and on target backgrounds. Check a favicon in a browser tab. Match the variant to the surface's owner: the tab and the application can use different themes. |
| Values and rights | Trace published values to their current sources. Check that links reach the stated material and included third-party files have applicable redistribution terms. |
| Web guide | Exercise relevant themes, narrow layouts, keyboard operation, direct section links, back navigation, copying success/failure, and downloads. Downloaded contents must match the named resources. |
| Document guide | Render and inspect the final pages, including examples, page boundaries, navigation, and resource links. Check production specifications when print is in scope. |

## Reader handoff

When the task includes validating the guide's usability, give a representative reader an application task with an observable result: choose the appropriate variant, obtain its file, and apply the relevant rule without the author's explanation. Observe where they hesitate or need missing information and identify the guidance to improve. Select tasks from the project's actual uses; [GOV.UK's testing method](https://www.gov.uk/service-manual/user-research/using-moderated-usability-testing) explains how to set goals without giving away the solution.

Report technical checks, visual inspection, and reader testing separately, with the tested conditions and remaining uncertainty. When no reader is available, use an expert walkthrough and label it as such. A screenshot establishes appearance in that captured state; it does not establish working downloads or complete accessibility.
