# D'Adamo's Review of the 30-Module Gap Analysis (via PM, 2026-10-30)

> **Provenance:** Walker sent the gap analysis (`docs/gap-analysis-30-modules.md`) to Dr. Peter D'Adamo; D'Adamo fed it into ESPERANTO's internals and returned the generated review below. Pasted verbatim by Walker via Telegram, 2026-10-30. The opening voice-transcription line is preserved as received. Our audit of this review's claims is in `research/04-dadamo-review-audit.md`.

---

"I opened up the thorax of Esperanto feed in your PM and got this :

It’s a useful list. My short verdict: build a few of these as one engine, not 30 separate modules, and be careful with the science in several of them.

What it gets right

The data really is there. I checked the SNP index on the platform: the genes these modules need are all present, for example HFE, DIO2, FADS1, LCT, ALDH2, CYP1A2, AOC1, AGXT, FUT2, VDR and HLA-DQA1.
The cross-division idea matches your own rule: a finding should combine genome, gut and labs, not report one division alone.

What it doesn’t know (it was written from public pages, not the code)

Module 1 (PGx) is already built. Metabolizer status and guideline advice are in O23PGx and O23ClinPGx and show on every client.
Module 5 (ABO, secretor, Lewis) is your core work and is already in COGENT (secretor_call, Lewis-negative logic).
The whole-client digest, the Brief, Sherlock, KEGG maps and organ systems already do much of the “what is the bottleneck” reasoning the closing note promises.

Where it is weak

Many of the scores would show false precision. VDR polymorphisms, composite MTHFR “methylation scores”, APOA2, tight-junction SNPs and most single-SNP gluten or bone scores have small or inconsistent effects. A number like “Methylation Capacity Index 62” reads as measured when it isn’t.
Some biology is wrong. For example, Akkermansia and Faecalibacterium are not zonulin producers. HLA-DQ2/DQ8 typing needs several tag SNPs together and is only meaningful as “cannot rule out / effectively rules out”. The mitochondrial haplogroup module needs mtDNA calls that most chips don’t carry.
Thirty separate modules violate your single-source rule and would mean maintaining thirty things."
