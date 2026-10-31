# 01 — OPUS23 | ESPERANTO: Platform Overview

## Summary

OPUS23 | ESPERANTO is Datapunk Bioinformatics' successor to the legacy Opus23 genomic-analysis suite: a browser-based clinical decision-support workstation for licensed health professionals that unifies three instruments — COGENT (genome), FLORIAN (gut microbiome) and KINESIS (metabolome/labs) — behind one client record, with a dedicated large language model producing cited case summaries, a question-answering mode and integrated next-step plans.[1]
It is pay-as-you-go (tokens), requires nothing installed, and is explicitly positioned as education and decision support, not a diagnostic test.[1]
The platform descends directly from Opus23 Pro, written by Dr. Peter D'Adamo at the Center of Excellence in Generative Medicine for use with patients at the University of Bridgeport.[4][5]

## Identity and lineage

The landing page describes OPUS23 | ESPERANTO as "the new generation of Opus23, the genomic exploration platform practitioners have relied on for years," keeping the curated SNP interpretations, multi-SNP algorithms and drug–gene work, and adding the microbiome (FLORIAN) and metabolomics (KINESIS) instruments on one shared client record and reasoning layer.[1] Legacy Opus23 Pro claims "over 200 clinicians worldwide" as users.[2] The platform's own published numbers on the landing page: 4,500+ curated SNPs, 389 multi-SNP algorithms, 22,800 microbial taxa, 3,200+ metabolites, three omics, one client record.[1]

A useful detail for tracking D'Adamo's curation over time: the multi-SNP algorithm count was marketed as "over 250" on the legacy splash page.[2]
The help docs and developer blog say "over 300,"[4][5] and the ESPERANTO landing page now states 389 — consistent with a living, growing curated library rather than a fixed artifact.[1]

## The reasoning layer

ESPERANTO's differentiating claim is a "dedicated large language model, in the background": it is given a de-identified case file ("the patient's actual data and nothing else") and is held to account with a clickable citation behind every claim.[1] Its outputs are three products — a written *Brief* per case, *Ask* (a conversational interface that looks up SNPs, markers, taxa and metabolites in the patient's own data and states plainly when the data don't cover a question), and *Next Steps* (an integrated start-of-care plan, weighing value against cost and exposing checkpoints where care could change direction).[1] The FAQ adds that the model is instructed to rule out "food, supplement and medication explanations before a pathological reading," and that clinical judgment remains with the practitioner.[1]

A fourth LLM system, **Opie**, is described as a nightly literature agent: every night it reads PubMed and ClinVar against what each patient has — diagnoses, carried variants, out-of-range microbes, flagged labs, supplements — keeps only human evidence bearing on care, writes one plain line with the reference, and can email the practitioner about ClinVar reclassifications or matching trials; alert emails carry no names or health details, only a sign-in link.[1]

## Positioning, access and pricing

Access is by account request; the platform is restricted to licensed health professionals (physicians, NDs, nutritionists, chiropractors and similar) and is "decision support for the professional, not a consumer product."[1]
It runs in any modern browser with nothing to install.[1]
Pricing is token-based pay-as-you-go: uploading a genome, microbiome sample or lab panel costs tokens, as do Brief, Ask and Next Steps; browsing, the Case File and reference libraries are free, client-record creation is free, and there is no subscription.[1]
Legacy Opus23 instead required a day-long training webinar with competency-based certification plus per-client upload licenses; original-Opus23 accounts can be linked and clients imported with genomes intact into ESPERANTO-era COGENT.[1][2]

Privacy posture per the landing page and FAQ: the patient's name and ID never leave the platform — the language model reads a de-identified case file — genome files stay on Datapunk's own server, never sold or shared, and outgoing LLM requests are checked for identifiers.[1] The legacy help docs describe SSL in transit plus AEM (Authenticated Encryption Methodologies) encryption at rest "that actually exceeds HIPAA standards."[4]

## Provenance and backing data

The platform describes itself as "curated, not scraped": built on decades of work in biochemical individuality — hand-curated SNP interpretations, algorithms and agent lists — backed by HMDB, ClinVar, KEGG, PGS Catalog and PubMed.[1] The legacy suite's mega-data mashups similarly cite GWAS, dbSNP, Interactome, Etiome, PubMed and HapMap as inputs.[2][4]

## Regulatory posture

The FAQ states plainly OPUS23 | ESPERANTO is not a diagnostic test: it interprets data patients already obtained, "for education and clinical decision support," and "does not diagnose, treat or prescribe."[1]

## Sources

[1] https://www.datapunk.net — OPUS23 | ESPERANTO · Datapunk Bioinformatics (platform landing page)
[2] https://www.datapunk.net/opus23 — Datapunk Opus23 Pro (legacy splash)
[4] https://www.datapunk.net/opus23/docs/index.pl?WELCOME — Opus23 Pro Help Docs — Welcome
[5] https://datapunk.net/opus23blog/about_opus23 — Opus23 Developer Blog — About Opus 23
