# context.md — the shared desk

version: 1.5
date: 2026-10-12
owner: product manager
change rule: bump the version and add a line under "Changes" for every edit; every part reads this file before acting; no part holds its own copy.

## 1. Who we write for

Primary reader: the owner or commercial manager of a Dutch trader in used commercial vehicles, trailers and machinery — 10 to 50 staff, no IT function, selling B2B and multilingual into mostly non-EU markets. They read one page to decide on one next step with AI.

Secondary reader: BAS World commercial and operations management, who host the case.

## 2. The case, and what it is not

BAS World (Veghel, BAS Group, 450+ staff, AI Search in production) is a frontier case: it shows what stays hard once budget and IT are no longer the limit. It does not describe the sector on average. Every claim carries a scope label: `case` or `sector`.

## 3. Quality bar: four baseline requirements + our six criteria

### 3a. Baseline requirements (handbook template floor)

These are the four things every page in the wider handbook must clear, before our own six criteria apply. Each is checked by a named part of the pipeline, not left implicit.

1. Clear to a non-technical reader. *(checked by: second reader — criterion 1 below covers step-naming; the second reader judges plain language overall)*
2. Accurate against appraised sources. *(checked by: tool — Check's per-claim quote/number/source-decision verification)*
3. Covers responsible use of AI. *(checked by: our criterion 3 below, plus the second reader)*
4. Useful to an owner. *(checked by: second reader — our criterion 6, one next step)*

### 3b. Our six criteria (PRD v2.1 §3 — verbatim)

1. Names a step in the sales or documentation chain (lead → quotation → contract → payment → export document), never a category of tool. *(checked by: reader)*
2. Keeps time-saving automation apart from automation that touches the customer, and says which each recommendation is. *(reader)*
3. Names the duty that applies (AI Act, GDPR, sanctions screening / Regulation 833/2014), the evidence for it, and any outside supplier's hosting location. *(tool: presence; reader: correctness)*
4. Labels every figure `company-reported` or `independently-verifiable`, and `case` or `sector`. *(tool)*
5. Labels every recommendation by complexity: `bought tooling`, `named process owner`, or `in-house build` (the last flagged as a warning). *(reader)*
6. Closes with one next step: an owner, a rough cost, and a three-month check. *(reader)*

### 3c. What a person checks — and what the tool checks alone

The tool checks every claim mechanically (`/verify-claims`, no model in the loop): the verbatim sentence is in the saved excerpt, the same sentence is in the live document at the source URL, every number in the translation is in the source, and the source is `decision: use`. A claim that clears all of that, from a trustworthy source, is marked `auto_verified: AUTO-PASS` and needs no person.

A person checks a source — once, covering every claim drawn from it — only when one of two triggers fires:

- **T1 less trustworthy:** credibility 1; or credibility 2 unless the source is of a primary or peer-reviewed type (regulation, statistics, vendor-contract-doc, peer-reviewed, think-tank) on a trusted host (`.claude/source-domains.txt`, sections REG, STAT, VEND, TT-*, Peer-reviewed; official suffixes such as europa.eu, overheid.nl, .gov, .edu) or cited at least 20 times; or it is rated 3 while its type cannot score 3; or the source file carries a `FLAG FOR HUMAN REVIEW` *and* the live check did not match (a flag about "possibly summarised text" is settled once the sentence is found character for character in the live document).
- **T2 document not found:** the live document cannot be fetched (blocked, gone, a PDF or script-rendered page the tool cannot read); or the quoted sentence is not in the live document or the saved excerpt; or a number sits in the source but not in the quoted sentence.

These sources are listed in `review_queue.md`. Mirrors of official texts (section MIRROR) are never trusted by host. The person opens each one, puts their name in `verified_by` for every claim that holds, and records the result in the queue. Appraise has no person gate any more: a person sees a rating only where it matters, in `review_queue.md`, next to the claims that rest on it. Find has none either: `gates.py intake` is the source gate (required fields, `published` date per gate G2, live document readable, every quoted excerpt passage found verbatim in it); a source that fails goes to `library/sources/incoming/_rejected/` with the reason.

What a person still always does: the second reader's criteria 1, 2, 5, 6 (§3b — the tool checks their form, a person judges whether the content is sound; the "Structure" section of `check.md` is where the reader starts); interview claims (§4); the final publish decision. A claim the tool fails outright (a number not in the source, malformed claim block, source discarded) goes back to Translate, not to a person — automatically, at most twice (`/run-page`), before it is reported.

## 4. Out of scope

- No screen or app beyond the command line.
- Nothing is published without a human check.
- English only.
- No AI model is trained on BAS World material.
- Interview material never reaches a model service (blueprint §6, the line).
- No claim enters a draft without a source and a quoted sentence.

## 5. House style

- Plain English, short sentences, no jargon an owner would have to look up.
- Every statement carries a `[claim-id]` that exists in `claims_en.md`.
- Every number: `company-reported` or `independently-verifiable`; every claim: `case` or `sector`.
- Recommendations name a step and a complexity label, never "use an AI tool".
- Each page states how much checking was done.
- Each page ends with one next step: owner, rough cost, three-month check.
- The disclaimer of the handbook template appears on every page: educational, not consultancy.

## Changes

- 1.0 (2026-09-17): first version, from PRD v2.1 and blueprint v1.0.
- 1.1 (2026-09-21): week-2 feedback — split §3 into the four handbook-template baseline requirements (3a) and our six criteria (3b), each baseline requirement now names whether Check (tool) or the second reader confirms it. No content of the six criteria changed.
- 1.2 (2026-10-01): added §3c — manual source checking reduced to two triggers (T1 less trustworthy, T2 document not found); everything else is verified mechanically and recorded in `auto_verified`. Replaces "a person verifies every number/quote" and the second reader's five random openings. Criteria 1–6 unchanged. Needs matching edits in PRD v2.1 §2/§6 and blueprint v1.1 §1a/§5 by their owners.
- 1.3 (2026-10-12): faster, fewer human steps. (1) Find gate "person checks URL and date" replaced by the mechanical source gate in `gates.py intake`. (2) Appraise gate removed; credibility ceiling and recency come from rules (`gates.py todo`), the appraiser judges relevance and the reason. (3) T1 narrowed: credibility 2 from a primary/peer-reviewed type on a trusted host (or 20+ citations) no longer needs a person; a FLAG only counts when the live check failed. (4) Check fills the duty table and a structure check for criteria 1, 2, 5, 6 itself. (5) Live checks run in parallel. Criteria 1–6 unchanged. Needs matching edits in PRD v2.1 §2/§6 and blueprint v1.1 §1a/§5 by their owners.
- 1.4 (2026-10-12): still fewer checks. (1) `review_queue.md` lists only claims cited in this week's draft (check on use). (2) A source stamped `verified_live: <date>` (set by `gates.py intake`, or by `gates.py stamp` for older sources whose excerpt is verbatim in the live page today) no longer goes to a person when the live page merely cannot be read later (403, script-rendered); a live page that is readable but no longer contains the sentence (NO MATCH) still does. (3) Years found in the excerpt are not "numbers not in the sentence". Criteria 1–6 unchanged.
- 1.5 (2026-10-12): quality moved upstream. `gates.py intake` now has a quality floor: a source enters only if it could later pass without a person (primary or peer-reviewed type on a trusted host, or 20+ citations); pointers (press, trader-channel) and unlisted hosts are rejected unless the finder writes `exception: <why>`, which then costs a person check. Finders must follow a pointer to the primary document and prefer trusted-host versions. `gates.py quality` reports how many saved sources the floor would have stopped. Criteria 1–6 unchanged.
