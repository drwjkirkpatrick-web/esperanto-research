# 04 — D'Adamo's Review Audited Against Public Documentation

## Summary and provenance limits

`docs/dadamo-review-response.md` is Dr. Peter D'Adamo's reply to the 30-module gap analysis, generated — per its own (voice-transcribed) opening line — by feeding the PM into ESPERANTO's internals. *(The verbatim artifact was withdrawn from this public repo on 2026-10-30; its analysis is retained below.)* It therefore combines insider platform knowledge with LLM-authored prose. **Treatment rule for this project: every claim in it is an attributed insider statement; only what public documentation corroborates is marked CONFIRMED. Absence from public pages is noted, not treated as refutation.**

## 1. Claims corroborated by public pages

**"The data really is there"** — the platform advertises a curated panel of more than 4,500 functional SNPs; the specific per-gene presence D'Adamo reports checking (HFE, DIO2, FADS1, LCT, ALDH2, CYP1A2, AOC1, AGXT, FUT2, VDR, HLA-DQA1) is insider information, but a curated functional-SNP panel of this size exists on public record.[1] *Status: consistent with public docs; gene-level detail insider-only.*

**Module 5's premise** — the gap analysis says "COGENT already reports ABO, FUT2, Lewis," and the landing page confirms COGENT reports "ABO, secretor (FUT2) and Lewis status."[1] D'Adamo's claim that this is "already in COGENT (secretor_call, Lewis-negative logic)" is thus directionally confirmed publicly; the internal flag names are insider-only. *Status: CONFIRMED (capability); internals unattested.*

**Module 1's data premise** — the gap analysis proposes a PGx dosing calculator from COGENT's drug–gene and ClinVar data; the landing page lists "Drug–gene interactions and ClinVar findings" as COGENT features[1], and the legacy suite already shipped a pharmacogenomics app (DRUGGIE, ">350 potential adverse reactions").[4] D'Adamo says PGx is "already built" as O23PGx and O23ClinPGx showing on every client — plausible evolution of documented capability; the names appear on no public page. *Status: capability CONFIRMED; O23PGx/O23ClinPGx names insider-only.*

**The reasoning-layer promise** — D'Adamo: "the whole-client digest, the Brief, Sherlock, KEGG maps and organ systems already do much of the 'what is the bottleneck' reasoning." Public corroboration: the Brief, Ask and Next Steps exist and are LLM-generated, and the Case File is "an overview of the whole case, grouped by theme."[1] Next Steps is explicitly "one integrated plan for the start of care," KEGG appears as a named backing resource ("backed by HMDB, ClinVar, KEGG, PGS Catalog and PubMed"), and "pathways that join the data" places flagged metabolites beside variant genes on maps.[1] The name **Sherlock** appears on no fetched public page (search returned nothing). *Status: PARTIAL — Brief/Next Steps/KEGG corroborated; Sherlock insider-only.*

**Single-source rule** — D'Adamo's closing argument ("thirty separate modules violate your single-source rule and would mean maintaining thirty things") matches the platform's own public positioning — "one client, every instrument... every report sees the others."[1] *Status: consistent; structural opinion, flagged as opinion not fact.*

## 2. Gap-analysis platform numbers vs public record

| Gap-analysis claim | Public record | Verdict |
| --- | --- | --- |
| 4,500+ curated SNPs | "4,500+ curated SNPs" (landing)[1] | ✓ exact match |
| 389 multi-SNP algorithms | "389 multi-SNP algorithms" (landing)[1] | ✓ exact match (legacy pages say 250+/300+ — a growing library)[2][4] |
| 22,800 microbial taxa | "22,800 microbial taxa" (landing)[1] | ✓ exact match |
| 3,200+ metabolites | "3,200+ metabolites" (landing)[1] | ✓ exact match |
| "unified reasoning layer powered by a dedicated large language model" | "A dedicated large language model, in the background."[1] | ✓ confirmed |
| COGENT reports ABO, FUT2, Lewis | "ABO, secretor (FUT2) and Lewis status"[1] | ✓ confirmed |
| "ClinVar PGx annotations" | COGENT lists "ClinVar findings" + drug–gene interactions[1] | Partial — PGx-specific ClinVar use not stated publicly |
| Three instruments, one client record | "3 omics · 1 client record"[1] | ✓ confirmed |
| Implementation-complexity estimates (Low/Medium/High) | not publicly measurable | Analyst-derived — unverifiable externally |
| Phased roadmap effort (weeks) | not publicly measurable | Analyst-derived — unverifiable externally |

## 3. Insider-only identifiers with zero public attestation

O23PGx · O23ClinPGx · Sherlock · the internal names `secretor_call` and "Lewis-negative logic" · the claim that mtDNA calls "most chips don't carry" is platform-knowledge rather than public documentation (its scientific plausibility is checked in `research/05-science-flags-check.md`). None of these occur on any fetched page; all remain attributed insider statements.

## 4. Science flags

D'Adamo's "false precision" list (VDR polymorphisms, composite MTHFR scores, APOA2, tight-junction SNPs, single-SNP gluten/bone scores) and his three biology corrections (Akkermansia/Faecalibacterium are not zonulin producers; HLA-DQ2/DQ8 needs multiple tag SNPs and is a rule-out test; chip mtDNA coverage) are literature questions, audited with citations in `research/05-science-flags-check.md`.

## 5. What this audit means for the artifacts

The gap analysis accurately read the *public* platform (all numeric and architectural claims exact-matched), and D'Adamo's review accurately identifies its blind spot: written from public pages, it could not know which capabilities already exist (PGx, ABO/secretor, bottleneck reasoning) — precisely the failure mode it admits in its own footer ("independent analysis of public platform documentation"). The two documents are complementary: the gap analysis's value is the candidate list and competitive framing; D'Adamo's reply supplies the insider filter. Neither is alone sufficient as a build plan.

## Sources

[1] https://www.datapunk.net — OPUS23 | ESPERANTO · Datapunk Bioinformatics (platform landing page)
[2] https://www.datapunk.net/opus23 — Datapunk Opus23 Pro (legacy splash)
[4] https://www.datapunk.net/opus23/docs/index.pl?WELCOME — Opus23 Pro Help Docs — Welcome
