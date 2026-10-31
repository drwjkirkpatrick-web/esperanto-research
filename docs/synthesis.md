# Synthesis — OPUS23 | ESPERANTO: the platform, the gap analysis, and the author's review

Date: 2026-10-30 · Dossiers: `research/01–05` · Artifacts: `docs/` · Ledger: `citations/ledger.json` (51 sources; platform sources carry verbatim evidence quotes)

## What the platform verifiably is

OPUS23 | ESPERANTO is the successor to Opus23 Pro: three instruments (COGENT genome, FLORIAN gut microbiome, KINESIS metabolome/labs) over one client record, with a dedicated background language model producing cited Brief/Ask/Next Steps outputs and a nightly literature agent (Opie).[1]
Its published numbers — 4,500+ curated SNPs, 389 multi-SNP algorithms, 22,800 microbial taxa, 3,200+ metabolites, 81 ingestible report formats — are documented on the landing page and verified here with verbatim quotes against saved page text.[1]
It descends from a suite written by D'Adamo at the COEGM for University of Bridgeport patients, is restricted to licensed professionals, priced per-use in tokens, and is explicitly not a diagnostic device.[4][5]

## The two artifacts, and their complementary blind spots

**The gap analysis was written outside-in**, from public pages only — its own footer says so. Its reading of the public platform was exact: every number it quotes matches the landing page, and its "unified reasoning layer powered by a dedicated large language model" matches the page's own language almost word for word.[1]
What it could not see: which capabilities already exist inside, and whether its proposed composite scores were scientifically defensible.

**D'Adamo's review was written inside-out**, generated from ESPERANTO's internals. (The verbatim reply text was withdrawn from this public repo on 2026-10-30; its analysis is retained here and in `research/04`.) It identified two of the thirty modules as already built — Module 1 (PGx) and Module 5 (ABO/secretor/Lewis) — which is publicly consistent: COGENT documents drug–gene interactions, ClinVar findings, and "ABO, secretor (FUT2) and Lewis status."[1]
It rejected the 30-module frame as violating the platform's single-record rule — corroborated publicly ("one client, every instrument... every report sees the others").[1]
And it flagged false precision and three specific biology errors.

## Audit result 1 — platform claims (research/01, 02, 04)

Every claim in either document that touches public documentation verifies exactly. Insider-only identifiers (O23PGx, O23ClinPGx, Sherlock, secretor_call internals) appear on no public page and are carried as attributed insider statements — in the record, never promoted to verified fact.

## Audit result 2 — competitive landscape (research/03)

Seven of the eight stated competitor weaknesses held CONSISTENT against the vendors' own pages; none verified false. Three material findings: "3MCor / MMIP" conflates two unrelated academic web servers (different teams, journals, inputs); GX Sciences' "~120 genes" is not publicly verifiable; and Jona and Tiny Health — framed as competitors — are simultaneously supported ESPERANTO ingest formats on Datapunk's own page, meaning ESPERANTO absorbs their output.[1]
The analysis also underweights competitor strengths: PromicsEdge's 200M+ imputation, Jona's and Tiny Health PRO's stool-chemistry panels, DeepCura's full practice-automation suite.

## Audit result 3 — the science flags (research/05)

Five of D'Adamo's seven flags are literature-**SUPPORTED**. The "zonulin producers" attribution is wrong twice over: zonulin is host pre-haptoglobin-2, neither taxon produces it, and both are associated with improved barrier function (→ 05 §1). HLA-DQ2/DQ8 chip typing needs six tag SNPs and is an exclusionary test per ESPGHAN (→ §2). VDR effects are trivially small at n=26,242 and VDR is absent from major 25(OH)D GWAS loci (→ §4). Composite MTHFR "methylation capacity" scores have no validated existence, and ACMG states MTHFR testing has minimal clinical utility (→ §5). Tight-junction-SNP permeability scores have no validated clinical use — in UC patients with objectively elevated permeability, none of the barrier-gene variants associated (→ §7).
Two flags are **PARTIAL**. The mtDNA caution holds for chip data, but Module 4's stated input is a whole-genome VCF — and WGS ingest is documented, so the flag applies only to array-sourced clients.[1]
And APOA2 rs5082 was genuinely replicated by its discoverers in three cohorts — the fair verdict is that post-2019 evidence is judged insufficient for genotype-guided prescribing, not that the finding never existed (→ §6).
The overall "false precision" verdict is supported: these 2–8-SNP composites sit below the calibration bar that even genome-wide polygenic scores are still struggling to meet (→ 05 §Overall verdict).

## The merged verdict

Three very different documents triangulate to the same structure. The vault is real, large, and matches its marketing numbers — now documented with verbatim quotes rather than asserted. Cross-instrument reasoning over one client record is the genuine moat, and two of the proposed modules merely rediscover shipped features. Numeric indices built from a handful of small-effect SNPs read as measured when they are not — the critique survives every literature check we ran.
What survives contact with evidence: a *small* set of engines over guideline-grade genotype–phenotype relationships (PGx dosing, HLA-DQ2/DQ8 rule-out, the well-powered single-gene diet/liver effects), computed across genome, gut, and labs, presented as ranges and evidence chains — not thirty named scores. Offered as analysis, not a build prescription.

## Outstanding questions

Inherited from the dossiers (see `research/03` and `research/05` Open questions): GX Pro7 consolidated gene count (provider-portal only); Jona/DeepCura genomics roadmaps; 3MCor server status after the 3mcor.cn content change; vendor chip-level mtDNA manifests; later APOA2 replications meeting multiplicity thresholds; zonulin family assay resolution for KINESIS values; whether any functional-medicine vendor has published calibration data for composite multi-gene pathway scores (grey literature at best).

## Sources

[1] https://www.datapunk.net — OPUS23 | ESPERANTO · Datapunk Bioinformatics (platform landing page)
[4] https://www.datapunk.net/opus23/docs/index.pl?WELCOME — Opus23 Pro Help Docs — Welcome
[5] https://datapunk.net/opus23blog/about_opus23 — Opus23 Developer Blog — About Opus 23
