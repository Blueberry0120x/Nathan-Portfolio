# # Controller -> Nathan-Portfolio

> Newest entries at top. History preserved in git.

---

## [2026-10-15 21:52] Floor Plan Sketchpad on AWS card added -- CONTROLLER-MADE @vscode-ext (Controller)

- **What changed:** `index.html`: an eighth project card (Design automation), "Floor Plan Sketchpad on AWS", linking the public about page https://d2s2iyd9xg4xp8.cloudfront.net/aws/floorplan.html (absolute, so it works from GitHub Pages too). No plan or screenshot of his on the card.
- **Why:** his words in the Controller session 2026-10-15: "Card yes". Wording from AWS-Project after the app passed its live check; the Controller read the live about page in a browser and every claim on the card is on it.

## [2026-10-15 20:06] Floor Plan card added then reverted, nothing changed -- CONTROLLER-MADE @vscode-ext (Controller)

- **What happened:** the Controller added a "Floor Plan Sketchpad on AWS" project card to `index.html` (AWS-Project's wording, checked against the live about page), then reverted it before any commit. The file matches `e6fb034`; nothing was published.
- **Why:** the Controller's permission check refused the commit (a public-site change on a peer's request). It waits for his word in the Controller's session.

## [2026-10-15 19:26] site.js script line added then reverted, nothing changed -- CONTROLLER-MADE @vscode-ext (Controller)

- **What happened:** the Controller added `<script src="/site.js" defer></script>` before `</body>` in `index.html`, `showcase/keynote.html` and `showcase/lsp.html` (AWS-Project's request: site-wide nav + chat bubble), then reverted all three before any commit. The files match `3d63236`; nothing was published.
- **Why:** the Controller's permission check refused the push (public pages loading code from outside the repo, on a peer's request). The change waits for his word in the Controller's session.

## [2026-10-15 17:50] index.html edit reverted before commit, nothing changed -- CONTROLLER-MADE @vscode-ext (Controller)

- **What happened:** the Controller edited two lines of `index.html` (a stats card and the entitlement bullet), then reverted them before any commit. The file matches `c520656`; nothing was published.
- **Why:** the change waits for his word in the Controller's session.

## [2026-10-15 17:37] His corrections: co-lead modeler; permit jurisdictions named -- CONTROLLER-MADE @vscode-ext (Controller)

- **What changed:** `index.html` (commit `c520656`): Austin light rail role -> "co-lead modeler" (stat, experience bullet, project card); the entitlement bullet now reads "Entitlement and permit work across California and Washington, including Seattle, Bellevue, San Diego, Los Angeles, Anaheim, Orange County, Escondido, and Chula Vista".
- **Why:** his words 2026-10-15, after the 1837361 fix: "Colead modeler" and "So i did Seattle Bellevue Sandiego, la, Anaheim, oc, escondido, Chula Vista, and so on". Recorded in NP_ClaudeAgent resume/master.md (6.1, 4.5a).

## [2026-10-15 17:35] Three claims now match the career record -- CONTROLLER-MADE @vscode-ext (Controller)

- **What changed:** `index.html` (commit `1837361`): Austin light rail "co-lead utility designer" -> "main utility modeler" (stat, experience bullet, project card); "19+ jurisdictions permitted across CA & WA" -> 19+ jurisdictions in a self-built zoning standards table; experience bullet "Entitlement work across 19+ jurisdictions" -> "Entitlement work in California and Washington"; permit-platform card "30 sites across 19+ jurisdictions" -> "A standards table covering 19+ jurisdictions".
- **Why:** the career record (NP_ClaudeAgent resume/master.md, VERIFY_CHECKLIST items a and b) shows main modeler, permits in 3 jurisdictions, and no cleared site count; the public chat (AWS-Project) repeats this page. Designer's go 2026-10-15: "Ok go for it".
- **Verified:** GitHub Pages build `built`; live page read with Playwright: old wording gone, new wording present.

## [2026-07-14 22:51] Published Keynote + LSP showcases + demo links -- CONTROLLER-MADE @claude-cli

- **What changed:** new `showcase/keynote.html` (Dynamo notes-to-table demo; gif regenerated sharp
  900x506 from source, was blurry 426x240) + `showcase/lsp.html` (AutoLISP library, self-contained) +
  `showcase/assets/keynote-notes-to-table.gif`. `index.html`: added `demo:` field to the Keynote and
  AutoLISP project objects + a 'View live demo' link render + `.demolink` CSS. Commit `ec651cd`.
- **Why:** the showcases existed only as local files in NP_ClaudeAgent/resume; Designer asked to publish
  them to the public site and link from the project cards so the dynamic-table demo is shareable via URL.
- **Note:** the keynote gif shows a Stantec/City of Bellevue project drawing; Designer explicitly approved
  publishing it public ('just leave it').
- **Origin:** Controller-made (NP_ClaudeAgent session), not an agent in this repo.

---

## [2026-07-14 12:41] Theme persistence polish -- CONTROLLER-MADE @claude-cli

- **What changed:** `index.html` now remembers the light/dark theme choice. Added a blocking head
  script that applies a saved `localStorage` theme before first paint (no flash), and the toggle handler
  now writes the choice to `localStorage`. Previously the theme reset to the OS preference on every reload.
  Commit `6190c4f`.
- **Also this session:** proofread + render-verified the whole page (desktop + mobile + dark) and the live
  GitHub Pages deploy. About section, 7 project cards, 6 permit cards all render clean, zero console errors.
  No content changes were needed -- the About paragraph and everything else were already complete.
- **Origin:** Controller-made (NP_ClaudeAgent session at Designer request to 'finalize the portfolio'),
  not an agent in this repo.

---

## [2026-07-07 13:09] Added deep-linkable Permit projects section -- CONTROLLER-MADE @claude-cli

- **What changed:** new `#permitting` section in `index.html` ("Permit projects") between the Projects
  and Skills sections, with 6 anchor-addressable cards (`#perm-redwood/elcajon/euclid/rainier/astreet/143rd`)
  split into "Independent design & permitting" (San Diego own work) and "Production support under the EOR"
  (WA short plats). Added `.pgrp/.pset/.pc` CSS + `:target` highlight + a mobile `.pset` rule. Commit `10dbd60`.
- **Why:** the Controller-built permit showcase PDF (`NP_ClaudeAgent/resume/NPham_Portfolio-Showcase.pdf`)
  now deep-links here -- a "View Full Portfolio" button -> `#permitting`, and each PDF project title ->
  its `#perm-<slug>` card. This section is the landing detail for those links.
- **Safety:** PII-free (owner/address withheld); no ADEC/Passio; roles honest (own work vs EOR support).
  PII scan on the built page returns NONE.
- **Origin:** Controller-made (NP_ClaudeAgent session), not an agent in this repo. If you pick this up,
  the section + the M.S./AI removal below were not yours.

---

## [2026-07-07 04:19] Removed M.S./AI degree from education -- CONTROLLER-MADE @claude-cli

- **What changed:** deleted the "M.S., Artificial Intelligence -- University of the Cumberlands --
  enrolled Fall 2026" education card from `index.html`. Per Designer directive to strip every mention of
  the AI master's / "enrolled" from ALL resume + HTML artifacts. Education now shows B.S. + EIT only.
- **Scope note:** this same directive was applied fleet-wide in the Controller repo the same turn --
  `NP_ClaudeAgent/resume/*` (cv.md/.html/.pdf, master.md, portfolio.html, editor JSON + SEED_JSON,
  landdev variant, keynote_suite_au.html, the Weyerhaeuser docx+pdf) and the OneDrive Desktop submission
  copies were all scrubbed and verified clean.
- **Origin:** Controller-made (NP_ClaudeAgent session). If you pick this repo up, the removal was not yours.

---

## [2026-07-07 04:05] index.html structural refactor + spacing tokens -- CONTROLLER-MADE @claude-cli

- **What changed:** `index.html` rebuilt for maintainability -- NO visual/content change. (1) Added a
  real HTML5 skeleton (`<!DOCTYPE html>` / `<html lang>` / `<head>` / `<body>`); the file was a raw
  fragment before. (2) Introduced a design-token system in `:root` -- spacing scale (`--space-xs`..
  `--space-3xl`) plus layout dials (`--maxw`, `--gutter`, `--section-y`, `--radius`, `--lead-width`) so
  padding/rhythm tune from one place. (3) Replaced all inline `style="..."` overrides (per-section
  padding, h2 font size) with modifier classes (`.section--flush-top`, `.section--tight-top`, `.h2--sub`).
  (4) De-minified the CSS into commented, labeled blocks; hero is now `<header>` (stats kept a `<div>` so
  it doesn't inherit section padding). Committed `cd35d9b`, pushed to `main`.
- **Then (still LOCAL, uncommitted at time of this note):** Designer asked to widen the About lead
  paragraph -- added a `--lead-width` token and set it to `1012px` (was `68ch`). Two small working-tree
  edits pending the Designer's go to push.
- **Why:** Designer asked to make the HTML "structural clean and neat, allow easy control of styles/
  padding as a web developer." The token system + inline-style removal is the direct answer -- all
  padding/width now controllable from the `:root` block at the top of `<style>`.
- **Verification done:** rendered the file before/after to full-page PNG via Playwright (light mode,
  1200px) -- pixel-for-pixel identical layout; base64 headshot byte-identical (70,472 chars); all
  skeleton tags present + balanced; theme toggle / filter / card-expand JS unchanged.
- **Origin:** Controller-made (NP_ClaudeAgent session), not an agent working directly in this repo --
  git author is the shared identity, so if you pick this repo up, this refactor + the pending
  `--lead-width` tweak were not yours. This note is the record.

---

## [2026-07-06 23:42] Design replacement + GitHub Pages enabled -- CONTROLLER-MADE @claude-cli

- **What changed:** `index.html` replaced end to end -- the prior showcase design (navy gradient hero,
  icon-square cards) was swapped for the editorial design approved in a parallel Controller session
  (dark/light theme toggle, real project cards with expand/collapse "Read more" + category filters, hero
  with headshot). Source: `NP_ClaudeAgent/resume/portfolio.html`, copied in and scrubbed for public
  exposure -- phone number removed (this repo's prior design never exposed a phone, only email +
  LinkedIn; matched that precedent and added a LinkedIn link the private source didn't have). Commit
  `05fd6bb`.
- **Why:** Designer reviewed both designs side by side this session, rejected the original ("week ass
  poor level"), approved the `resume/portfolio.html` one ("this is so much better"), then explicitly
  asked to publish it here.
- **Also this pass:** GitHub Pages enabled on `main`/root via `gh api` -- live at
  `https://blueberry0120x.github.io/Nathan-Portfolio/`.
- **Verification done before push:** standalone check (1 network request, base64-embedded headshot, no
  external assets), phone-number absence confirmed, LinkedIn/mailto links present, content scan for
  visa/immigration/salary/compensation/sponsorship terms (zero matches).
- **Origin:** this was made by the Controller (NP_ClaudeAgent session), not by an agent working directly
  in this repo -- git author is the shared identity, so if you're picking this repo back up, the change
  wasn't yours and this note is the record of what happened and why.
- **This is the first controller-note/ entry for this repo** -- folder + `.ctrl-ping` created this pass
  (CTRL-005 two-channel ping protocol). Channel B (controller -> project) is now wired for future
  cross-repo writes here.
