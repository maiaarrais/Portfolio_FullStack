# Design QA

final result: passed

## Visual target and evidence

- Source: selected Engineering Editorial direction, saved as `qa/selected-reference.jpg`.
- Original source pixels: 1024 × 1600; normalized to 1440 × 2250 for comparison.
- Desktop implementation: `../portfolio-desktop.jpg`, captured at 1440 CSS pixels wide, density 1. Viewport 1440 × 1024; full-page image includes the expanded portfolio below the fold.
- Combined full-region comparison: `qa/comparison-final.jpg`.
- Focused typography/hero comparison: `qa/hero-comparison-final.jpg`.
- Case-study interaction evidence: `../portfolio-case-study.jpg`.
- Mobile tested at 390 × 844 CSS pixels; measured document width 390 with no horizontal overflow. Default in-app browser layout also checked at 615 pixels wide.

## Intended adaptations

The user selected direction 1, then requested real project pictures, previews, fuller project explanations, and a separate repository. Original screenshots, hardware photos, and the original video therefore replace the concept's illustrative diagrams. Case-study dialogs, archive, biography, technical skills, and contact extend the initial concept. The site retains its white/slate/teal palette, editorial hierarchy, practice rail, thin rules, and open project rows. The decorative wave is omitted to keep the expanded page quiet and focused on original project evidence.

## Comparison history

1. Initial implementation: [P2] Rising Intentions used a confirmation-screen capture, which did not show its central visualization. Replaced it with the original skyline image from `project3.png`. Verified in the final full-page capture.
2. Initial normalized comparison: [P2] The hero scale and page margins weakened the chosen editorial hierarchy. Increased desktop heading size to 78px, constrained the headline to 850px, expanded the page grid to 1440px, increased title sizes, and recaptured. The final focused comparison now retains the four-line headline and strong hierarchy.
3. Final comparison: no actionable P0/P1/P2 findings. Original media additions explain the different lower-page density and project order.

## Required fidelity surfaces

- Typography: DM Sans renders correctly. Slate headings, restrained teal labels, and distinct body/metadata scales remain readable. Desktop headline wrapping matches the chosen hierarchy. Mobile scales to a single column.
- Layout rhythm: consistent 64px desktop outer padding, section rules, image/copy alignment, and open rows. Mobile uses 24px padding. No horizontal overflow was observed at 390px.
- Colors: slate `#2d3945`, muted teal `#327781`, pale teal surfaces, and light rules follow the resume and selected direction. Focus outlines are visible.
- Images: original project captures and photos load without broken-image results; web-optimized formats retain recognizable detail. Photo galleries use contain sizing. Thumbnail crops are intentional, while case-study photos expose the complete image. The video poster is an actual demo frame.
- Copy: project role, API/data flow, decisions, prototype limitations, and next improvements are explicit. No invented measured outcomes, AWS credentials, professional experience, or BETA affiliation are claimed.

## Interaction checks

- Case studies open from text and image buttons.
- Flow Studio gallery changes from capture 1/2 to 2/2.
- Bracelet gallery advances between original photos.
- Native dialog opens with close-button focus; Escape dismisses it.
- Mobile navigation expands and collapses after selecting Work.
- Original classroom video plays: readyState 4, duration 128.25 seconds, paused false, advancing currentTime.
- All image checks returned no broken images.
- Browser console check returned no warnings/errors during tested states.
- Resume URLs and source-link destinations were inspected. The resume asset is present; clipboard copy relies on browser permissions and was not exercised to avoid changing the user's clipboard.
- Production build and four bundled worker/package tests pass. The repository-path build uses `/Portfolio_FullStack/`.

## Follow-up polish

- [P3] Some original screenshots contain captured browser/editor chrome and a thin bottom edge. These are authentic development captures. Re-recording clean project media would improve the presentation further.
- The bracelet case study links the resume brief until a verified source-code repository is supplied. Original photos are included now.

## Implementation checklist

- [x] Original media and verified source links
- [x] Accessible gallery/dialog controls
- [x] Video playback
- [x] Responsive layout and navigation
- [x] Resume and contact
- [x] Content rationale and application guide
- [x] Build and packaging validation
