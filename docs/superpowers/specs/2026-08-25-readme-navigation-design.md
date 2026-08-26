# ScientificWriting README navigation design

## Goal

Make the repository structure and worked examples visible without moving or
duplicating the main writing guide.

## Approved structure

- Keep the complete concise guide in the root `README.md`.
- Add a short opening that explains the two repository surfaces: the README
  states the guidelines, and `Examples/` shows individual guidelines applied
  to real papers.
- Link the current example from that opening.
- Add a `Pages` badge to the header.
- Add a `Pages` table near the end, following the neighboring public modules.
- Add a `What's in This Repo` directory tree after the Pages table.
- Add matching light and dark banners for the opening, Pages, and repository
  layout sections using the neighboring module pattern.
- Keep the existing `See Also` section last.
- Rename the current example from `01-SelfAlignedPDCS.md` to
  `01-IntroductionAsScenario.md` so its filename describes the guideline.
- Keep the paper title, authors, arXiv record, PDF, and DOI inside the example.

## Resulting layout

```text
ScientificWriting/
├── README.md
├── Examples/
│   └── 01-IntroductionAsScenario.md
└── assets/
```

## README order

1. Header and navigation badges.
2. Short repository introduction and link to the current example.
3. Existing writing guide, unchanged except for required navigation links.
4. Pages table.
5. Repository layout.
6. See Also.

## Scope

This change does not add more examples, move the guide into another file, or
edit Notion. The existing GitHub workflow will mirror the updated root README.

## Verification

- All README links resolve after the rename.
- The Pages badge targets the Pages anchor.
- Light and dark banner assets exist for any new banner sections.
- The README and example contain no em dashes.
- The local branch matches `origin/main` after publication.
