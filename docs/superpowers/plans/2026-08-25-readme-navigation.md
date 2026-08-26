# ScientificWriting README Navigation Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Make the root guide, worked examples, and repository layout immediately visible while keeping the existing concise guide in `README.md`.

**Architecture:** The root README remains the canonical guide and gains navigation around its existing content. Worked examples remain separate Markdown files named after the guideline they demonstrate. New light and dark SVG banners follow the existing module treatment.

**Tech Stack:** Markdown, SVG, Git, GitHub README-to-Notion workflow.

## Global Constraints

- Keep the complete guide in the root `README.md`.
- Each example covers one guideline.
- Rename the example according to the guideline, not the paper.
- Do not edit Notion.
- Do not use em dashes in the README or example.
- Preserve unrelated files and remote history.

---

### Task 1: Rename the worked example

**Files:**
- Rename: `Examples/01-SelfAlignedPDCS.md` to `Examples/01-IntroductionAsScenario.md`

**Interfaces:**
- Consumes: The existing annotated self-aligned PDCS example.
- Produces: The guideline-based path used by the README links.

- [ ] **Step 1: Rename the file with Git history preserved**

Run:

```bash
git mv Examples/01-SelfAlignedPDCS.md Examples/01-IntroductionAsScenario.md
```

- [ ] **Step 2: Verify the example content and relative guide link**

Run:

```bash
test -f Examples/01-IntroductionAsScenario.md
test ! -e Examples/01-SelfAlignedPDCS.md
rg -n '\[main guide\]\(\.\./README\.md\)' Examples/01-IntroductionAsScenario.md
```

Expected: The renamed file exists, the former path is absent, and the relative README link remains valid.

### Task 2: Add README navigation and repository overview

**Files:**
- Modify: `README.md`
- Create: `assets/banner-forewords.svg`
- Create: `assets/dark/banner-forewords.svg`
- Create: `assets/banner-pages.svg`
- Create: `assets/dark/banner-pages.svg`
- Create: `assets/banner-repo-layout.svg`
- Create: `assets/dark/banner-repo-layout.svg`
- Modify: Existing banner SVG numbers to preserve section order.

**Interfaces:**
- Consumes: The neighboring wiki module pattern and the renamed example path.
- Produces: Header navigation, a repository introduction, a Pages table, and a repository tree.

- [ ] **Step 1: Add the Pages badge and opening**

Insert a `PAGES` badge targeting `#pages`. Add a Forewords section explaining:

```markdown
This repository is the group's concise guide to writing a scientific paper.
The README states the guidelines. The worked examples show how one guideline
appears in a real paper through short excerpts and direct annotations.

Read the guide first, then use the examples to see each rule applied. The
current example is [The introduction is a scenario](Examples/01-IntroductionAsScenario.md).
```

- [ ] **Step 2: Add the Pages table before the repository layout**

Use:

```markdown
| Page | What it covers |
|------|-----------------|
| [Main guide](README.md) | Purpose, narrative, selection, figures, sentence-level writing, and consistency |
| [Example 1: The introduction is a scenario](Examples/01-IntroductionAsScenario.md) | Annotated introduction from the self-aligned PDCS paper |
```

- [ ] **Step 3: Add the repository tree before See Also**

Use:

```text
ScientificWriting/
├── README.md
├── Examples/
│   └── 01-IntroductionAsScenario.md
└── assets/
    └── dark/
```

- [ ] **Step 4: Add and renumber the banner assets**

Create matching light and dark Forewords, Pages, and What's in This Repo banners. Use section numbers `00` through `09` in README order: Forewords, Purpose, Introduction, Write Only What Matters, Figures, Strunk and White, Consistency, Pages, Repository Layout, See Also.

- [ ] **Step 5: Verify README structure and links**

Run:

```bash
git diff --check
rg -n 'href="#pages"|id="pages"|01-IntroductionAsScenario.md|banner-forewords|banner-pages|banner-repo-layout' README.md
test -f Examples/01-IntroductionAsScenario.md
for f in forewords pages repo-layout; do test -f "assets/banner-$f.svg"; test -f "assets/dark/banner-$f.svg"; done
```

Expected: All navigation targets and files exist, with no whitespace errors.

### Task 3: Verify and publish

**Files:**
- Modify: `../WIKI_MEMORY.md`

**Interfaces:**
- Consumes: The completed README, example rename, and banner assets.
- Produces: A verified public commit and an updated local wiki handoff.

- [ ] **Step 1: Run final content checks**

Run:

```bash
git diff --check
! rg -n '—' README.md Examples/01-IntroductionAsScenario.md
git status --short
```

Expected: No whitespace errors, no em dashes, and only the approved files are changed.

- [ ] **Step 2: Update the wiki memory**

Record the guideline-based example filename and the README navigation structure in `../WIKI_MEMORY.md`.

- [ ] **Step 3: Commit and push**

Run:

```bash
git add README.md Examples assets docs/superpowers
git commit -m "Add ScientificWriting repository navigation"
git push origin main
```

- [ ] **Step 4: Verify the remote state**

Run:

```bash
git fetch origin main
test "$(git rev-parse HEAD)" = "$(git rev-parse origin/main)"
git status --short --branch
```

Expected: `HEAD` equals `origin/main` and the worktree is clean.
