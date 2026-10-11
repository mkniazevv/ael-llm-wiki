# Log

Every operation on this wiki, **newest first**. New entries go directly under the line below.
The format is fixed so that `grep "^## \[" wiki/log.md | head` lists the most recent ten:

    ## [YYYY-MM-DD] operation | title

Operations: `ingest`, `query`, `lint`, `synthesis`, `schema`, `fix`. A `query` entry lists the pages
that were read, so a wrong answer can be traced to what it was built on.

---

## [2026-10-11] lint | after the first three ingests

- Script: 0 errors, 0 warnings (an orphan warning for the synthesis was fixed by linking it from two concept pages).
- By hand: no unrecorded contradictions found. Gaps: no source on whether AI saves time or keeps quality; no agency-specific source; no source on tool data terms or GDPR.
- Suggested next sources: Autoriteit Persoonsgegevens guidance on generative AI; KVK guidance on an AI policy; a documented case of a small Dutch or EU agency.

## [2026-10-11] synthesis | Where should a small agency start with AI?

- Filed: [[where-should-a-small-agency-start-with-ai]]
- From the query below.

## [2026-10-11] query | Which part of a small marketing agency's work should it test AI on first?

- Asked by: Maksim (via Claude)
- Read: [[index]], [[generative-ai-use-in-smes]], [[ai-for-marketing-and-sales]], [[complexity-of-ai-use]], [[ai-adoption-barriers]], [[ai-spending-by-small-firms]], [[ai-adoption-by-sector]]
- Checked in sources: [[2025-12-12-cbs-bedrijven-gebruiken-ai-vaakst-voor-marketing-of-verkoop]], [[2025-oecd-ai-adoption-by-small-and-medium-sized-enterprises]], [[undated-jpmc-understanding-the-use-of-ai-among-small-businesses]]
- Not answerable from the wiki: whether AI saves time without hurting quality; agency-specific practice; tool data terms.

## [2026-10-11] ingest | JPMorganChase Institute: Understanding the use of AI among small businesses

- Added by: Samsul (chosen and appraised in agent run RUN-003, 27 Sep 2026)
- New: [[undated-jpmc-understanding-the-use-of-ai-among-small-businesses]], [[jpmorganchase-institute]], [[ai-spending-by-small-firms]]
- Updated: [[ai-adoption-by-firm-size]] (source_count 2 → 3), [[ai-adoption-by-sector]] (source_count 2 → 3, confidence 0.75 → 0.8), [[generative-ai-use-in-smes]] (source_count 1 → 3 together with OECD; definition debate recorded)
- Debates: none new
- Raw: copied word for word from the agent's capture; only chart descriptions were captured.
- Lint: clean

## [2026-10-11] ingest | OECD: AI adoption by small and medium-sized enterprises

- Added by: Maksim (chosen and appraised in agent run RUN-002, 27 Sep 2026)
- New: [[2025-oecd-ai-adoption-by-small-and-medium-sized-enterprises]], [[oecd]], [[complexity-of-ai-use]]
- Updated: [[ai-adoption-by-firm-size]] (source_count 1 → 2), [[ai-adoption-by-sector]] (1 → 2), [[ai-adoption-barriers]] (1 → 2, confidence 0.7 → 0.75), [[generative-ai-use-in-smes]] (1 → 2)
- Debates: [[ai-adoption-by-firm-size]]: OECD 11.9 percent (10 to 49 employees) against the CBS table reading of 27 percent (10 to 50 persons employed); scope, year and definitions differ.
- Raw: PDF text extracted by the agent (pypdf), copied word for word; the PDF itself is still to be added beside it.
- Lint: clean

## [2026-10-11] ingest | CBS: Bedrijven gebruiken AI vaakst voor marketing of verkoop

- Added by: Maksim (first ingested in agent run RUN-001, 26 Sep 2026; appraised 7/10 Tier B in RUN-004 and RUN-006)
- New: [[2025-12-12-cbs-bedrijven-gebruiken-ai-vaakst-voor-marketing-of-verkoop]], [[cbs]], [[ai-adoption-by-firm-size]], [[ai-adoption-by-sector]], [[ai-for-marketing-and-sales]], [[ai-adoption-barriers]], [[generative-ai-use-in-smes]]
- Debates: none (first source)
- Raw: fetch_article.py could not reach cbs.nl from the cloud environment, so the text was copied word for word from the agent's capture of 27 Sep 2026, with the five frontmatter fields filled in.
- Go-ahead: Maksim asked Claude to build the wiki for Monday (11 Oct). The takeaways used are the evidence the team already approved in the agent; the team still needs to read the pages.
- Lint: clean
