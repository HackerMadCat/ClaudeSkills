---
name: "content-style"
description: "Structure rules for any written text: Slack drafts, YouTrack issues/comments, commit messages, docs, notes, project markdown. Use whenever writing or editing prose for Sergei."
---

## Content Style

How to structure any written artifact: Slack drafts, YouTrack issues and comments, commit messages, Google Docs, scratch notes. Structure only — markup syntax follows each tool's own conventions.

1. **Brevity.** Minimum words per fact. Prose only where rules 6–7 allow it.
2. **Point first.** The first line says what happened or what is needed; everything else supports it.
   - Bad: `Yesterday we started looking into the flaky tests and after some digging…`
   - Good: `Nightly build is red because of a race in IndexCache` + sub-bullets
3. **Lists and headers, not paragraphs or tables.** Content goes into flat or nested lists, one header per topic when the text covers several.
4. **One thought per line.** Independent facts go into nested sub-bullets, not chained with dashes and semicolons.
   - Bad: `Rolled back the release — migration locks the users table, ~5% of requests affected, fix in review, ETA tomorrow`
   - Good: top line — what happened; sub-bullets — cause, impact, next step
   - Rule of thumb: a line longer than two screen lines almost always splits
5. **Comparable items within a category.** Items of one kind are described with the same fields in the same order.
   - Named field goes in bold at the start of the line: `- **Cost:** 2 days`
   - Comparable: each option in a proposal → what it is, cost, risk
   - Not comparable: one option has a risk field, another doesn't; one cost is a number, another a paragraph
6. **Uncategorizable but important → note or conclusion.** A fact that fits no field goes into a `>` note above the list or into a conclusion, not forced into a field it doesn't belong to.
7. **Notes and conclusions — 1–2 simple sentences max.** No reasoning chains, filler words or hedging.
8. **One level of abstraction per text.** A text about X contains facts about X, not conclusions about using X elsewhere.
   - Issue: bug, repro, expected vs actual; impact on the roadmap goes to the planning doc
   - Commit message: what changed and why; the investigation story goes to the issue
   - Code comment: why this code is the way it is; the migration plan goes to the issue
9. **No meta about the writing process.** No "double-checked", "updated after discussion", edit history.
   - An open question on substance is data — keep it
   - How and when the text was revised is not — version history covers that

## Applying

- Don't copy the wording of the request or source verbatim — the job is to structure and research, not to retell.
- Not enough data for a field — say so and ask, don't fill in guesses.
- No context/root-cause/expected essay structure in YouTrack issues. Keep them terse: 2–4 short paragraphs or a short list.
