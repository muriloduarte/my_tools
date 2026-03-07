You are helping me write a GitHub Pull Request.

Task:
1) Compare the current branch against `master` and understand what changed.
   - Use the git diff context available in the editor.
   - If you do NOT have the diff in context, ask me to paste the output of: `git diff master...HEAD`
2) Based on the diff, produce:
   a) A SUGGESTED PULL REQUEST TITLE (in ENGLISH)
   b) A PR description (in ENGLISH) using the exact markdown template below
3) Keep it ESSENTIAL: focus on what changed and why (no fluff).
4) VERY IMPORTANT: Do NOT change the markdown layout below.
   - Do not rename headings.
   - Do not reorder sections.
   - Do not add/remove sections.
   - Keep checkbox lines exactly as-is.
   - Only change the CONTENT inside the sections (e.g., replace placeholder sentences; tick checkboxes when appropriate).

Rules for the PR title:
- Provide one concise, descriptive title in English.
- Prefer an action-oriented summary (e.g., "Fix ...", "Add ...", "Refactor ...").
- If there is evidence of a Linear issue key in the diff/branch name/context, prefix it at the beginning of the title; otherwise do not invent it.

Rules for checkboxes:
- In "PR type": tick exactly ONE that best matches the change. If uncertain, tick "Other".
- In "Checklist": only tick items you can confidently assert from evidence (diff, tests shown, my confirmation). If unsure, leave unchecked.

Content guidelines:
- "Describe your changes": 3–6 concise bullet points. Mention key files/modules affected. Call out any behavior change, config change, migration, or risk.
- If there are tests added/updated, mention them (names/paths if visible).
- If there is any follow-up needed, mention it briefly.
- "Relevant links": include links only if they exist in the diff/context (issues, docs, Linear ticket, rollout dashboard). Otherwise write "N/A".

Output (STRICT):
- Return ONLY:
  1) A first line: `Suggested PR title: <title>`
  2) Then the final markdown content using the exact template below
- No extra commentary.

Template markdown (KEEP THE SAME LAYOUT; ONLY UPDATE CONTENT):
## Describe your changes
Your message goes here, be as descriptive as possible

## Relevant links
- Relevant links go here

## PR type
- [ ] Feature
- [ ] Refactor
- [ ] Bug Fix
- [ ] Documentation
- [ ] Infrastructure
- [ ] Other

## Checklist
- [ ] Extended the README / documentation, _if necessary_
- [ ] Created tests that fail without the change, _if possible_
- [ ] **_(Required)_** Tests passing locally
- [ ] **_(Required)_** Rebase/Merge latest `master`
- [ ] **_(Required)_** Deployed to **_dev_** environment
- [ ] **_(Required)_** Requested PR review
- [ ] Insert Linear issue number at the beginning of PR title
