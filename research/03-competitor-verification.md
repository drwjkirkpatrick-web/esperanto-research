# 03 — Competitor Verification: The Gap Analysis's Landscape vs. Competitors' Own Pages

Audit of the eight competitors in `docs/gap-analysis-30-modules.md` (Competitive Landscape Context). All pages fetched 2026-10-30; quotes are verbatim from saved extracts in `extracts/competitor-*.txt`.

## Summary

All eight competitors are real products, and every "claims" column entry matches what their own pages publish. Seven of eight stated weaknesses verify CONSISTENT against vendor-owned pages; GX Sciences' "~120 genes" is UNVERIFIABLE as stated (only per-panel counts are published). Two material findings: "3MCor / MMIP" conflates two unrelated academic web servers, and named competitors Jona and Tiny Health are also supported ingest formats on Datapunk's ESPERANTO page — data sources as much as rivals. Competitor strengths are underweighted throughout: PromicsEdge imputes to 200M+ variants, Jona and Tiny Health have added stool-chemistry panels, and DeepCura is a full practice-automation suite, not a scribe alone.

## 1. Jona

**Offers:** a $495 clinical gut test pairing deep shotgun metagenomic sequencing with stool-chemistry biomarkers, AI interpretation trained on 220K+ peer-reviewed studies, Digital Twin simulation of diet/lifestyle/probiotic interventions, and personalized Action Plans.[^1]

> Jona combines shotgun metagenomic sequencing with clinical stool chemistry biomarkers[^1]

**Claims:** CONSISTENT. **Weakness (no native genomic integration; SNP data external):** CONSISTENT — nothing genomic appears in its materials; the stack is gut microbiome plus stool chemistry.[^1] **Wrong/omitted:** the Advanced tier's stool biomarkers (calprotectin, secretory IgA, lactoferrin, pancreatic elastase) edge into ESPERANTO's KINESIS territory; Jona is also an ESPERANTO ingest format (Gaps).[^1][^16]

## 2. PromicsEdge

**Offers:** white-labeled practitioner DNA platform — 1,500+ genetic reports with ancestry-adjusted PRS, PGx, carrier-status and methylation reports, lab and lifestyle data integration; free to doctors, with kit commissions.[^2][^3]

> Analyze over 1500 conditions with ancestry-informed polygenic risk scores.[^2]

**Claims:** CONSISTENT. **Weakness (no metabolome instrument; gut data limited):** CONSISTENT with nuance — no owned metabolome assay or microbiome product exists, but it ingests lab biomarkers (4,000+ per its comparison table) and markets "multiomics analysis" over uploaded data.[^2] **Omitted:** a genomic-scale advantage the analysis never engages —

> Thanks to our advanced genetic imputation technology, our system transforms ~750,000 SNPs from standard genotyping chips[^2]

— into over 200 million data points.[^2]

## 3. Tiny Health PRO

**Offers:** shotgun-metagenomic gut and vaginal tests for consumers and practitioners; the PRO tier adds stool chemistry to the sequencing.[^4]

> shotgun metagenomics strain-level microbial and functional insights[^4]

> additional stool chemistry markers like Secretory IgA, Calprotectin, Beta-glucuronidase[^4]

**Claims (strain-level gut + vaginal):** CONSISTENT. **Weakness (no genetic or metabolomic reasoning layer):** CONSISTENT — the catalog is microbiome-only; no genomic ingest, systemic metabolomics, or cross-omics reasoning appears anywhere.[^4] **Omitted:** PRO's stool-chemistry panel (secretory IgA, calprotectin, elastase, occult blood) partially blurs "no metabolomic"; Tiny Health is also an ESPERANTO ingest source (Gaps).[^4][^16]

## 4. GX Sciences

**Offers:** provider-only nutrigenomic testing under the Fagron Genomics US brand — 17 panel categories plus the seven-area Pro7 comprehensive report; cheek-swab collection, white-label custom panels.[^5][^6]

**Claims (turn-key nutrigenomic panels):** CONSISTENT. **Weakness (~120 genes; no microbiome):** the figure is UNVERIFIABLE as stated — no consolidated count is published; per-panel numbers run 7–74 (21 genes methylation, 30 immune, 34 developmental, 74 athletic markers), e.g.:

> Seven key genes have been chosen by our experts to be analyzed for SNPs in the area of Detoxification.[^5]

The magnitude is plausible but unconfirmable. "No microbiome" is CONSISTENT — no stool product exists on the site.[^5][^6] **Omitted:** the Fagron rebrand.[^5]

## 5. DeepCura

**Offers:** a $129/provider-month "Electronic Health Workforce" — ambient scribe, AI receptionist, unified inbox, coding — with IFM Matrix and Timeline templates plus functional-medicine lab-interpretation support.[^7][^8]

> DUTCH/GI-MAP/OAT integration via DeepEvidentia[^7]

**Claims:** CONSISTENT. **Weakness (generic LLM; not grounded to a curated SNP database):** CONSISTENT — its own site names the general-purpose frontier model behind its deepest review agent,

> Claude Fable 5.1 at maximum effort works through the evidence: about 10 minutes and 25 credits per review.[^8]

while the DeepEvidentia evidence engine searches the literature (PubMed, Cochrane, IFM textbooks, NIH ODS), not any curated SNP base.[^7] **Omitted:** DeepCura does interpret uploaded genomics (MTHFR, COMT, CBS, MTRR, GST, CYP) in templates — genomics-aware, if not genome-grounded — and is a broader workflow suite than "AI scribe" conveys.[^7][^8]

## 6. Metabolon IBP

**Offers:** the enterprise Integrated Bioinformatics Platform for research teams — metagenomic, metabolomic and phenotypic data unified no-code; DIABLO multi-omics integration; Circos and microbe–metabolite correlation analyses.[^9]

> The Microbiome Analysis Tool unifies metagenomic, metabolomic, and phenotypic data within a codeless, accessible platform[^9]

**Claims (enterprise metagenome + metabolome):** CONSISTENT. **Weakness (research-oriented; no clinical decision support):** CONSISTENT — every workflow targets study groups and investigators:

> This lets researchers do what they do best: form hypotheses and let the data lead them to biological conclusions[^9]

No patient-level reporting, intervention logic or practitioner decision support appears.[^9] **Wrong/omitted:** nothing material.

## 7. 3MCor / MMIP

**Offers:** the slash-entry is two unrelated academic servers. 3MCor (*Bioinformatics* 2022) runs metabolome–microbiome correlation pipelines under phenotype/confounder instruction, returning CSV/PDF research outputs.[^10]

> 3MCor is the first platform developed specifically for the correlation analysis of metabolome and microbiome[^10]

MMIP (*Briefings in Bioinformatics* 2023) predicts community metabolic potential from 16S amplicon data and scores it against uploaded metabolomics.[^12][^13]

> a web-based analytical and predictive tool that can be used to compare the taxonomic content, diversity variation and the metabolic potential[^12]

**Claims (academic microbiome-metabolome correlation):** CONSISTENT. **Weakness (no genome; no practitioner-facing reports):** CONSISTENT for both — inputs are study cohorts, outputs are hypothesis-generating figures.[^10][^12] **Errors/omissions:** two distinct tools conflated; and 3mcor.cn now fronts an amino-acid age clock, not the described server:

> Biological age reflects the combined influence of genetic, environmental, and lifestyle factors[^11]

## 8. FunctionalDX

**Offers:** UK practitioner blood-chemistry service — 120+ biomarkers across pre-built and custom panels, algorithm-interpreted against "functional" optimal ranges and delivered as the Functional Health Report.[^14][^15]

> We use ranges that are based on optimal physiology and not the “normal” population.[^14]

**Claims:** CONSISTENT. **Weakness (no genetics or microbiome):** CONSISTENT — the entire catalog is blood chemistry; no genetic or microbiome product, ingest or interpretation appears anywhere.[^14][^15] **Wrong/omitted:** nothing material; it is a lab-plus-software bundle, not pure software.[^15]

## Gaps and errors found in the gap analysis's landscape

1. **"3MCor / MMIP" is a category error** — two independent academic tools (different teams, journals, inputs) presented as one competitor.[^10][^12]
2. **GX Sciences' "~120 genes" is unverifiable** against public pages; per-panel counts run 7–74, no published total.[^5][^6]
3. **Jona and Tiny Health are also ESPERANTO data sources** — Datapunk's landing page lists both as ingest formats; framing them purely as competitors misses that ESPERANTO absorbs their output:

> Tiny Health | Gut Health Test, shotgun metagenomic (.pdf)[^16]

> Jona Health | Clinical Gut Microbiome Analysis, shotgun metagenomic (.pdf)[^16]

4. **Strengths underweighted:** Jona added clinical stool-chemistry biomarkers;[^1] Tiny Health PRO likewise;[^4] PromicsEdge imputes chip SNPs to 200M+ variants and ingests 4,000+ lab biomarkers;[^2] DeepCura spans practice automation with EHR write-back.[^7][^8]
5. **The weaknesses column held up well** — seven of eight CONSISTENT, none INCONSISTENT.

## Key sources

- Jona — Clinical Gut Microbiome Analysis Advanced — https://jona.health/products/jona-clinical-gut-microbiome-analysis-advanced
- PromicsEdge — Medical Doctors platform — https://promicsedge.com/medical-doctors/
- PromicsEdge Lite — https://promicsedge.com/lite/
- Tiny Health — Store — https://www.tinyhealth.com/store
- Fagron Genomics US (GX Sciences) — Core Panels — https://gxsciences.com/nutrigenomics/
- Fagron Genomics US — Pro7 Panel — https://gxsciences.com/nutrigenomics/pro7-panel/
- DeepCura — AI Scribe for Functional Medicine — https://www.deepcura.com/resources/best-ai-scribe-for-functional-medicine
- DeepCura — Homepage — https://www.deepcura.com/
- Metabolon — Microbiome Analysis Software — https://www.metabolon.com/bioinformatics-software/microbiome-software/
- 3MCor paper (preprint) — https://pdfs.semanticscholar.org/e7bc/6cd38db249ae0f9448dc29195d3c8ef52cb5.pdf
- AmiAge Clock (current 3mcor.cn) — https://3mcor.cn/
- MMIP abstract — PubMed 37771003 — https://pubmed.ncbi.nlm.nih.gov/37771003/
- MMIP server — https://bioinfo.jisiasr.org/mmip/index.html
- FunctionalDX — FDX Method — https://functionaldx.com/fdx-method/
- FunctionalDX — Home — https://functionaldx.com/
- Datapunk — OPUS23 | ESPERANTO — https://www.datapunk.net/

## Open questions

- GX Sciences' consolidated Pro7 gene list sits behind a provider portal; the true SNP total — NOT FOUND — could not verify from public pages.
- Whether Jona plans genomic ingest on its roadmap — NOT FOUND — could not verify.
- Whether DeepCura intends a curated genomic knowledge base beyond template-level variant interpretation — NOT FOUND — could not verify.
- 3MCor's original server status after the 3mcor.cn content change — NOT FOUND — could not verify (R backend persists on GitHub per the paper).

[^1]: Jona Clinical Gut Microbiome Analysis Advanced — https://jona.health/products/jona-clinical-gut-microbiome-analysis-advanced (accessed 2026-10-30)
[^2]: DNA Testing & Precision Medicine Platform for Medical Doctors — https://promicsedge.com/medical-doctors/ (accessed 2026-10-30)
[^3]: Lite - OmicsEdge — https://promicsedge.com/lite/ (accessed 2026-10-30)
[^4]: Store - Tiny Health — https://www.tinyhealth.com/store (accessed 2026-10-30)
[^5]: Core Panels | Fagron Genomics US — https://gxsciences.com/nutrigenomics/ (accessed 2026-10-30)
[^6]: Pro7 Panel | Fagron Genomics US — https://gxsciences.com/nutrigenomics/pro7-panel/ (accessed 2026-10-30)
[^7]: Best AI Scribe for Functional Medicine (2026) | DeepCura Resources — https://www.deepcura.com/resources/best-ai-scribe-for-functional-medicine (accessed 2026-10-30)
[^8]: DeepCura — Beyond the EHR: The Electronic Health Workforce — https://www.deepcura.com/ (accessed 2026-10-30)
[^9]: Microbiome Analysis Software - Metabolon — https://www.metabolon.com/bioinformatics-software/microbiome-software/ (accessed 2026-10-30)
[^10]: 3MCor: An Integrative Web Server for Metabolome-Microbiome-Metadata Correlation Analysis (preprint) — https://pdfs.semanticscholar.org/e7bc/6cd38db249ae0f9448dc29195d3c8ef52cb5.pdf (accessed 2026-10-30)
[^11]: AmiAge Clock — https://3mcor.cn/ (accessed 2026-10-30)
[^12]: Microbiome Metabolome Integration Platform (MMIP) — PubMed PMID 37771003 — https://pubmed.ncbi.nlm.nih.gov/37771003/ (accessed 2026-10-30)
[^13]: MMIP — Microbiome Metabolome Integration Platform — https://bioinfo.jisiasr.org/mmip/index.html (accessed 2026-10-30)
[^14]: FDX Method - Functional DX — https://functionaldx.com/fdx-method/ (accessed 2026-10-30)
[^15]: Home Functional DX — https://functionaldx.com/ (accessed 2026-10-30)
[^16]: OPUS23 | ESPERANTO · Datapunk Bioinformatics — https://www.datapunk.net/ (accessed 2026-10-30)
