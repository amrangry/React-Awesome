# DESIGN.md — Agentic Curation Guide for React-Awesome

> Machine-readable rules for AI agents (and humans) curating this awesome-list.
> Source of truth for taxonomy, entry schema, and validation. `CONTRIBUTING.md` is the human summary — this file is normative.

## 1. Repo architecture

- Single-file list: `README.md` is the database. No per-category files.
- `README.md` sections are fixed taxonomy (see §2). Do not create new top-level `##` sections without a PR explaining why.
- `CONTRIBUTING.md` = human onboarding. `DESIGN.md` (this file) = agent execution spec.
- No code, no build step. Validation is: markdown format + link integrity + taxonomy correctness.

## 2. Taxonomy (where entries go)

Decide placement by this decision tree, in order:

1. **React Native-only?** (imports `react-native`, uses native modules) → `React Native — UI Kits / Navigation / Core Utilities`
2. **Works on both Web (react-dom) + Native (react-native) from same API?** (Tamagui, NativeWind, Dripsy, Solito) → `Cross-Platform (Web + Native)`
3. **Expo-specific module / router / EAS?** → `Expo Ecosystem`
4. **Web-only React?** → matching `React — *` section:
   - Full themed component set → `UI / Design Systems`
   - Unstyled behavior/a11y only → `Headless / Primitives`
   - CSS solution → `Styling`
   - Table/grid, charts, forms, state, fetching, routing, animation, testing → respective section
5. **Bundler/framework/linter/formatter** → `Build / Tooling`

If two sections fit, pick the primary use-case. Never list the same repo in two sections — cross-link with `(see X)` instead.

Current section anchors (keep TOC in sync):
`react--ui--design-systems`, `react--styling`, `react--headless--primitives`,
`react--data-tables--data-grid`, `react--charts--visualization`, `react--forms`,
`react--state-management`, `react--data-fetching--server-state`, `react--routing`,
`react--animation--motion`, `react--testing--devtools`,
`react-native--ui-kits`, `cross-platform-web--native`, `react-native--navigation`,
`react-native--core-utilities`, `expo-ecosystem`, `build--tooling`

## 3. Entry schema

Exact format, one line per entry:

```md
- [Name](https://github.com/org/repo) — One-line factual description.
```

Rules agents MUST enforce:

- `Name`: canonical repo name, preserve casing (`shadcn/ui`, `MUI X Data Grid`). No emojis, no version numbers.
- URL: prefer `https://github.com/org/repo` (no trailing `/`, no `/tree/...` except monorepo subpaths like `expo/expo/tree/main/packages/expo-router`). No URL shorteners, no blog mirrors.
- Separator: em-dash `—` (U+2014), not `-` or `--`.
- Description: 8–20 words, factual, no marketing (`blazing`, `best`, `ultimate`). Say what it does + who it's for. End with period.
- Ordering: alphabetical by Name within section (case-insensitive). `Elastic EUI` sorts under E.
- Max ~10 entries per section. If section exceeds 10, propose split or prune weakest in PR description — don't silently delete.

Good:
```md
- [Zustand](https://github.com/pmndrs/zustand) — Minimal, hook-based state store for React.
```

Bad:
```md
- [awesome zustand stuff](https://bit.ly/xyz) - The BEST state manager ever!! check it out
```

## 4. Acceptance / verification (agent pre-flight)

Before editing `README.md`, verify each candidate:

1. **Exists:** URL returns 200. If GitHub API available, confirm repo is public and not archived (archived → reject unless historically significant + marked).
2. **Maintained or canonical:** last commit ≤12 months AGO, OR (>1k stars AND widely depended upon, e.g. Formik). Note which condition passed in PR body.
3. **In-scope:** library/tool/framework for React or React Native devs. Reject: tutorials, courses, boilerplates, dotfiles, personal demos.
4. **No duplicate:** grep `README.md` for `org/repo` and for case-insensitive Name. Duplicates across sections → reject.
5. **License sanity:** must be OSI-approved or source-available with free use for the stated purpose. Flag Elastic-license / commercial (e.g. AG Grid Enterprise, MUI X Pro) inline if relevant — don't exclude, just don't mislabel as MIT.

If any check can't be performed (no network), state `UNVERIFIED: <reason>` in PR and add at most 3 entries.

## 5. Agent workflows

### A. Add 1–3 entries
1. Read `README.md` target section + TOC.
2. Run pre-flight (§4).
3. Insert alphabetically, keep dash/emdash/description style.
4. Verify TOC anchor still matches heading (GitHub slug: lowercase, spaces→`-`, remove `—`, `/`→``). If heading changed, update TOC.
5. Summarize: what added, where, which acceptance condition met.

### B. Batch audit (max 20 URLs per run)
1. Check each URL status + last-commit freshness.
2. Report table: `| Name | Status | Last commit | Action (keep/flag/remove) |`.
3. Do NOT mass-delete. Mark stale as PR suggestion, remove only if 404/archived + replacement noted.

### C. New section proposal
Only if ≥3 candidates don't fit existing taxonomy. Open PR with: proposed heading, placement, 3 seed entries passing §4, and TOC diff.

## 6. Forbidden

- Do not reformat the entire file (whitespace-only diffs rejected).
- Do not add badges, screenshots, or multi-paragraph reviews.
- Do not change `##` headings casing/punctuation without updating TOC in same edit.
- Do not invent stars, versions, or compatibility claims. If unsure, omit.
- Do not commit directly to `main` — branch + PR.

## 7. Quick checklist (paste into PR)

```text
- [ ] Format: - [Name](url) — Description.
- [ ] Alphabetical in section, TOC in sync
- [ ] URL 200, official repo/docs
- [ ] Maintained (commit ≤12mo) or canonical (>1k★ stable)
- [ ] Grepped for duplicates, correct taxonomy (§2)
```
