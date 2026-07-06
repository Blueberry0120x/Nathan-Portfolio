## [2026-07-06T23:42:06Z] Design replacement + GitHub Pages enabled -- CONTROLLER-MADE @claude-cli

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
