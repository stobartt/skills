# Skill evaluation cases

Evaluate decisions and outcomes rather than matching wording. Select cases affected by the skill change. When exercising a case on real files, use a separate workspace and remove disposable artifacts afterward. Distinguish a document walkthrough from an executed behavioral test.

For a substantial method change, include contrasting project contexts, a narrow update, and a boundary case. Reuse the quality criteria while checking that project-specific decisions differ appropriately. Record inputs, observed outputs, and remaining uncertainty; a scenario table alone is not evidence of a successful run.

## Scope and transfer

| Request and inputs | Expected behavior | Failure signal |
| --- | --- | --- |
| Document a general-purpose design system whose owner explicitly specifies no narrow target audience. | Accept its broad scope, identify guide-reader tasks and application contexts, and work with its established identity. | Inventing personas or treating absent market segmentation as a blocker. |
| Develop a second project's brandbook after completing one with a different palette, material, and clear-space ratio. | Reuse the method and quality checks while deriving the second project's values and rules from its own brief and evidence. | Carrying the first project's visual choices or quantitative rules into the second as defaults. |
| Review logo placement against an approved diagram that excludes the trademark symbol from the clear-space measurement. | Measure from the edges identified in the diagram and account for padding already in the file. | Rejecting a compliant placement because the symbol extends beyond the measurement edge or counting built-in padding twice. |
| A shared framework has its own identity and supports products with independently chosen identities. | Separate the framework's identity from consumer identities and document only the intended reuse boundaries. | Imposing the framework's logo or colors on every consumer, or inventing permission to replace restricted elements. |
| Propose an identity direction for a new brandbook; the brief requests concepts rather than production assets. | Use design mode, explain the relevant choices and tradeoffs, and distinguish proposals from established rules. | Declaring proposals approved or expanding delivery to an unrequested asset package. |
| A web-only brandbook has no print requirements, while a packaging brief lacks a printer profile. | Treat print as outside scope in the first case and identify the dependent production decisions in the second. | Treating both omissions as blockers or inventing production values to fill a template. |

## Workflow and delivery

| Request and inputs | Expected behavior | Failure signal |
| --- | --- | --- |
| Research how existing brand guides organize logo usage rules; no guide or assets requested. | Compare relevant primary sources, connect findings to the question, state transfer limits, and deliver the research. | Inventing a new identity or creating an unrequested asset package. |
| Build a digital brandbook from two approved raster logos; web graphics must be AVIF. | Preserve both masters, export AVIF with required transparency, prepare a supported favicon separately, and show selection rules with actual files. | Regenerated proportions, recoloring one master to invent the other, a false vector SVG, or AVIF as the sole favicon. |
| Update a logo built from SVG circles and rectangles and remove raster graphics from its brandbook and package. | Preserve the editable shapes and check previews, downloads, and the package for vector-only artwork. | Requiring conversion to paths without a delivery requirement, embedding a bitmap in SVG, or leaving raster deliverables in the package. |
| Change only the accent color in an existing brandbook. | Find the source value, update dependent rules and examples, and check contrast and affected assets. | Unrequested changes to the mission, typeface, navigation, or document structure. |
| Create a brandbook for printed packaging without a color profile or approved logo. | Identify proposals and missing inputs, research the medium, and complete work independent of the missing production decisions. | Arbitrary CMYK or Pantone values presented as approved production specifications. |
| Review an existing guide without changing files. | Use the relevant asset and presentation checks, then report located problems, consequences, proposed corrections, and verification methods in the review deliverable. | Writing project files during the review, skipping asset-use rules, or declaring complete WCAG compliance without sufficient evidence. |
| The favicon is light, the app was manually switched to dark mode, and the browser remains light. | Assess the tab's background separately from the app theme and inspect both contexts. | Synchronizing every asset to one theme setting regardless of its surface. |
| A halo appears around the logo only in a preview tool. | Inspect the alpha channel and ordinary compositing before changing the master. | Regenerating the image or removing edges based on one faulty preview. |
| Adjust a button's padding or generate one standalone logo. | Handle the local task with the appropriate tool without invoking the brandbook workflow. | An unnecessary brand brief, strategy research, or document package. |
| Validate whether a new reader can use a finished guide; only expert inspection has been performed. | Distinguish existing technical and visual evidence from reader testing, and use an observable application task when a participant is available. | Presenting the author's walkthrough as independent reader evidence. |
