# Science-Flags Check: D'Adamo's Review of the 30-Module Gap Analysis vs. the Medical Literature

Date: 2026-10-30. Scope: Each of the seven scientific objections raised in Dr. Peter D'Adamo's review of `docs/gap-analysis-30-modules.md` is checked against PubMed-indexed literature fetched for this audit. Verdicts: SUPPORTED / CONTESTED / PARTIAL.

## Summary

D'Adamo's factual claims hold up remarkably well. Zonulin is a human protein (pre-haptoglobin-2), not a bacterial product — neither *Akkermansia muciniphila* nor *Faecalibacterium prausnitzii* is documented as a zonulin producer, and both are actually associated with improved barrier function. HLA-DQ2/DQ8 SNP-chip calling genuinely requires multiple tag SNPs (six for the standard method) and celiac guidelines explicitly frame HLA testing as exclusionary. VDR, MTHFR, and APOA2 scores rest on small, population-heterogeneous effects; ACMG explicitly states MTHFR testing has minimal clinical utility. No validated composite "methylation capacity" or tight-junction-SNP permeability score exists in the literature. D'Adamo's mtDNA caveat is right for chip-based data, though Module 4's stated WGS-VCF input blunts it. Overall, the "false precision" critique is supported: single/few-SNP composite scores lack the calibration evidence that clinical genomics bodies demand even of genome-wide polygenic scores.

## 1. Zonulin: "Akkermansia and Faecalibacterium are not zonulin producers"

**VERDICT: SUPPORTED.**

Module 28 lists *A. muciniphila* and *F. prausnitzii* as "FLORIAN zonulin producers." Human zonulin was identified as pre-haptoglobin-2, a host-encoded protein: proteomic analysis of human sera showed zonulin is "the precursor for haptoglobin-2 (pre-HP2)" whose EGF-like motif drives EGFR/PAR-2 transactivation and increases intestinal permeability [^1]. Fasano's group describes zonulin as "the only known physiologic modulator of intercellular TJs described so far" — a host secretion, with release stimulated from the intestinal epithelium (e.g., by gliadin exposure in celiac disease) [^2][^3]. No literature documents *A. muciniphila* or *F. prausnitzii* as zonulin producers; a broad PubMed search for that association returns only studies correlating these taxa with circulating zonulin as an outcome, not a production mechanism. The gap analysis also gets the sign wrong: the Akkermansia outer-membrane protein Amuc_1100 interacts with TLR2 and "improves the gut barrier," partially recapitulating the bacterium's anti-metabolic-disease effects in mice [^4]. *A. muciniphila* is characterized as "the mucin-degrading commensal bacterium" — it consumes mucins, not modulates host zonulin [^5]. *F. prausnitzii* is a major butyrate-producing, anti-inflammatory commensal whose supernatant abolished NF-κB activation in Caco-2 cells and whose abundance loss predicts Crohn's recurrence [^6][^7]. A further caution for Module 28: a widely used commercial zonulin ELISA "does not detect precursor of haptoglobin2... rather structural analog proteins... with properdin being the most likely possible candidate," so even KINESIS zonulin values are questionable [^8].

## 2. HLA-DQ2/DQ8 typing: SNP chips, tag SNPs, rule-out logic

**VERDICT: SUPPORTED.**

The specific SNPs cited in the gap analysis workflow are correct: rs2187668 and rs7454108 "accurately predict[ed]" DQ2.5 and DQ8 respectively as tagging SNPs [^9]. But single-SNP inference is population-limited; the validated chip-based method uses six tagging SNPs spanning DQ2.5, DQ2.2, DQ7, and DQ8, predicting risk haplotypes carried by ">95% of CD patients" via linkage disequilibrium [^10] and validated in Finnish, Hungarian, and Italian cohorts [^11]. This confirms D'Adamo's "several tag SNPs together" requirement. On clinical semantics, ESPGHAN states: "HLA-DQ2 and HLA-DQ8 testing is valuable because CD is unlikely if both haplotypes are negative" — an explicit rule-out framing; the 2020 update builds diagnosis on TGA-IgA serology, with HLA retained for exclusion or complex cases [^12][^13].

## 3. mtDNA panels: chip coverage vs. haplogroup assignment

**VERDICT: PARTIAL (supported for chip-based data; weaker against the module's stated WGS input).**

Purpose-built anthropology chips document the gap: "many commercial arrays exist for genome-wide SNP genotyping, they were designed for medical genetic studies," while the GenoChip had to be specially designed "to identify all known Y-chromosome and mtDNA haplogroups" [^14]. Studies that have extracted mtDNA haplogroups from standard Illumina GWAS arrays (e.g., HumanHap550/1M) note the arrays carry only limited mitochondrial markers and required bespoke "mitochondrial genome imputation" and HaploGrep pipelines to assign haplogroups [^15]; a large HumanExome-array schizophrenia study likewise worked from sparse mtDNA SNPs plus imputation and reported no survived associations [^16]. D'Adamo's caution is therefore accurate for chip-derived uploads. Caveat: Module 4 specifies "From WGS VCF data," and a true whole-genome VCF does carry full mtDNA calls — so the flag applies only if client records are array-sourced.

## 4. VDR polymorphisms (FokI/BsmI/ApaI/TaqI) for bone/vitamin-D scores

**VERDICT: SUPPORTED.**

The participant-level meta-analysis of 26,242 individuals (GENOMOS) found VDR genotype-BMD differences "less than 0.011 g/cm²," all nonsignificant, and fracture odds ratios "very close to 1.00 (range, 0.98 to 1.02)" [^17]. A 2011 fracture meta-analysis yielded only marginally significant small protective odds (e.g., BsmI bb, OR 0.87) [^18], while a 2022 men-only meta-analysis reported some significant BsmI/FokI-BMD associations — exactly the small-and-inconsistent picture across strata D'Adamo describes [^19]. For vitamin-D status itself, the SUNLIGHT GWAS (n=33,996) identified GC, DHCR7, CYP2R1, and CYP24A1 as the determinants of 25(OH)D; VDR variants were not among the genome-wide-significant loci [^20]. Modules 11/29's VDR-weighted scores would overstate these variants' contribution.

## 5. Composite MTHFR "methylation scores"

**VERDICT: SUPPORTED.**

Component effects are real but modest and context-dependent. A1298C alone is not associated with higher homocysteine or lower folate; only combined 677/1298 heterozygosity reduces enzyme activity measurably [^21]. The C677T TT genotype carried just a 16% higher odds of CHD overall (OR 1.16) in the Klerk *JAMA* meta-analysis, with null findings in North America (OR 0.87) vs. Europe — an interaction attributed to folate status [^22]. Guideline-level evidence opposes clinical use: ACMG states "MTHFR polymorphism testing has minimal clinical utility and... should not be ordered as a part of a routine evaluation for thrombophilia" [^23]. For a composite multi-gene "Methylation Capacity Index" (Module 2) that sums MTHFR/MTR/MTRR/BHMT/PEMT/COMT/MAT1A/SHMT1 into a numeric readout: NOT FOUND — no validated composite methylation-capacity score based on these SNPs could be located in the literature. This is precisely the "false precision" pattern; nutrigenetic-evidence frameworks stress that genotype-based advice must rest on "clear evidence of validity" [^24].

## 6. APOA2 rs5082 (-265T/C) saturated-fat sensitivity

**VERDICT: PARTIAL.**

The original interaction was real and multiply replicated by its discoverers: Corella et al. reported the APOA2 -265T>C × saturated-fat interaction on BMI in three independent populations (Framingham Offspring, GOLDN, Boston Puerto Rican), with CC homozygotes on high-SFA diets showing higher BMI [^25], later extending to dairy-food sources [^26]. But the same paper opens with the field's caveat: "Nutrigenetics studies... aiming to provide more personalized dietary advice... However, replication has been low" [^25]. A 2019–2025 PRISMA-ScR scoping review found the interaction in DIETFITS only nominal (p=0.035, failing a multiplicity benchmark), concluded the findings "do not constitute independent cross-cohort replication," and judged that the evidence "does not support routine genotype-guided dietary prescribing" [^27]. D'Adamo's grouping of APOA2 with small/inconsistent effects is broadly fair for clinical scoring purposes; calling the original finding absent would be wrong.

## 7. Tight-junction SNPs (CDH1/OCLN/TJP1) for a "Gut Mucosal Integrity Index"

**VERDICT: SUPPORTED.**

Direct counterevidence exists: in ulcerative colitis patients with objectively elevated intestinal permeability (lactulose/mannitol test), sequencing of barrier GWAS genes HNF4A, ECM1, CDH1, and LAMB1 found that "none of the studied variants... showed an association with" increased permeability [^28]. The best-known association, a CDH1 risk haplotype in Crohn's disease, is small (OR 1.2), and its documented mechanism is mis-localization of E-cadherin protein — not an individual-level permeability predictor [^29]. NOT FOUND — any validated clinical use of common CDH1, OCLN, or TJP1 genotypes to predict intestinal permeability or a composite mucosal-integrity phenotype. Candidate-gene associations of disease (Crohn's, UC) with barrier genes do not convert into SNP-based permeability scores.

## Overall verdict

D'Adamo's "false precision" critique is supported. Across all seven flags, the pattern is consistent: the variants and taxa exist, but their individual effects are small, population-dependent, or mechanistically attributed incorrectly — and in two cases ("zonulin producers," composite methylation/tight-junction scores), the constructs themselves have no documented validity. The pattern the gap analysis proposes — single- or few-SNP composite scores presented as numeric indices — sits well below the evidentiary bar that even genome-wide polygenic risk scores are held to. The American Heart Association's scientific statement on PRS notes that "despite advances, risk prediction remains imprecise" and frames current scores around unresolved clinical considerations and future challenges [^30], while portability work shows PRS "are several times more accurate in individuals of European ancestry than other ancestries," a calibration failure even for well-powered scores [^31]. If calibrated, genome-wide, empirically validated scores require this level of scrutiny, two-to-eight-SNP heuristic composites with stated-but-unmeasured effects clearly read as measured when they are not.

## Key sources

- Tripathi et al., *Identification of human zonulin as prehaptoglobin-2* (PNAS 2009) — https://pubmed.ncbi.nlm.nih.gov/19805376/
- Fasano, *Zonulin, regulation of tight junctions, and autoimmune diseases* (Ann NYAS 2012) — https://pubmed.ncbi.nlm.nih.gov/22731712/
- Review of celiac pathophysiology incl. gliadin-stimulated zonulin release (Curr Opin Gastroenterol 2009) — https://pubmed.ncbi.nlm.nih.gov/19122520/
- Plovier et al., *Akkermansia membrane protein improves gut barrier* (Nat Med 2017) — https://pubmed.ncbi.nlm.nih.gov/27892954/
- Ganesh et al., *A. muciniphila exacerbates Salmonella gut inflammation* (mucin-degrading commensal) — https://pubmed.ncbi.nlm.nih.gov/24040367/
- Sokol et al., *F. prausnitzii is an anti-inflammatory commensal* (PNAS 2008) — https://pubmed.ncbi.nlm.nih.gov/18936492/
- Rivière et al., *Bifidobacteria and butyrate-producing colon bacteria* (Front Microbiol 2016) — https://pubmed.ncbi.nlm.nih.gov/27446020/
- Scheffler et al., *Zonulin ELISA does not detect pre-haptoglobin2* (Front Endocrinol 2018) — https://pubmed.ncbi.nlm.nih.gov/29459849/
- Celiac HLA haplotype typing via rs2187668/rs7454108 (Methods Cell Biol 2023) — https://pubmed.ncbi.nlm.nih.gov/37625876/
- Monsuur et al., *Six tag SNPs detect celiac HLA risk alleles* (PLoS ONE 2008) — https://pubmed.ncbi.nlm.nih.gov/18509540/
- Koskinen et al., *Tag-SNP HLA typing validated in 3 populations* (Immunogenetics 2009) — https://pubmed.ncbi.nlm.nih.gov/19255754/
- Husby et al., ESPGHAN 2012 celiac diagnosis guidelines — https://pubmed.ncbi.nlm.nih.gov/22197856/
- Husby et al., ESPGHAN 2020 celiac diagnosis guidelines — https://pubmed.ncbi.nlm.nih.gov/31568151/
- Elhaik et al., *GenoChip designed to resolve all mtDNA haplogroups* (Genome Biol Evol 2013) — https://pubmed.ncbi.nlm.nih.gov/23666864/
- Gandal et al., mtDNA haplogroups from Illumina arrays + imputation (JAACAP 2024) — https://pubmed.ncbi.nlm.nih.gov/38072244/
- Goncalves et al., HumanExome mtDNA variants in schizophrenia (PLoS ONE 2018) — https://pubmed.ncbi.nlm.nih.gov/29370225/
- Uitterlinden et al., VDR participant-level meta-analysis (Ann Intern Med 2006) — https://pubmed.ncbi.nlm.nih.gov/16908916/
- Fang et al., VDR-fracture meta-analysis (Bone 2011) — https://pubmed.ncbi.nlm.nih.gov/20601302/
- Zheng et al., VDR-BMD in men meta-analysis (Ageing Res Rev 2022) — https://pubmed.ncbi.nlm.nih.gov/35063697/
- Wang et al., SUNLIGHT 25(OH)D GWAS (Lancet 2010) — https://pubmed.ncbi.nlm.nih.gov/20541252/
- van der Put et al., *MTHFR A1298C second common mutation* (Am J Hum Genet 1998) — https://pubmed.ncbi.nlm.nih.gov/9545395/
- Klerk et al., MTHFR 677C>T-CHD meta-analysis (JAMA 2002) — https://pubmed.ncbi.nlm.nih.gov/12387655/
- ACMG Practice Guideline, lack of evidence for MTHFR testing (Genet Med 2013) — https://pubmed.ncbi.nlm.nih.gov/23288205/
- Grimaldi et al., guidelines for genotype-based dietary advice validity (Genes Nutr 2017) — https://pubmed.ncbi.nlm.nih.gov/29270237/
- Corella et al., APOA2 × saturated-fat BMI replication (Arch Intern Med 2009) — https://pubmed.ncbi.nlm.nih.gov/19901143/
- Smith et al., APOA2-dairy interaction replication — https://pubmed.ncbi.nlm.nih.gov/24108135/
- Scoping review of APOA2/FTO/MC4R adiposity evidence 2019–2025 — https://pubmed.ncbi.nlm.nih.gov/42950483/
- Schröder et al., permeability-gene variants in UC (J Dig Dis 2016) — https://pubmed.ncbi.nlm.nih.gov/26512799/
- Muise et al., CDH1 haplotype in Crohn's (Gut 2009) — https://pubmed.ncbi.nlm.nih.gov/19398441/
- AHA Scientific Statement on polygenic risk scores (Circulation 2022) — https://pubmed.ncbi.nlm.nih.gov/35862132/
- Martin et al., PRS health-disparities critique (Nat Genet 2019) — https://pubmed.ncbi.nlm.nih.gov/30926966/

## Open questions

1. Does any later replication of APOA2 rs5082 × saturated fat outside the Corella group meet multiplicity thresholds? The scoping review says not yet, but newer cohorts may exist.
2. Whether 23andMe/Ancestry's custom mtDNA SNP sets (which exceed standard GWAS arrays) suffice for the sub-haplogroup resolution COGENT would need — requires vendor chip manifests, not in PubMed.
3. Fasano-group definitions of "zonulin family" peptides vs. properdin/MASP cross-reactivity: assay-level resolution for KINESIS zonulin values remains unsettled.
4. Whether any functional-medicine vendor has published calibration data for composite multi-gene pathway scores (none indexed; likely grey literature only).

[^1]: Identification of human zonulin, a physiological modulator of tight junctions, as prehaptoglobin-2 (PNAS 2009) — https://pubmed.ncbi.nlm.nih.gov/19805376/ (accessed 2026-10-30).
[^2]: Zonulin, regulation of tight junctions, and autoimmune diseases (Ann NY Acad Sci 2012) — https://pubmed.ncbi.nlm.nih.gov/22731712/ (accessed 2026-10-30).
[^3]: Celiac disease (Curr Opin Gastroenterol 2009) — https://pubmed.ncbi.nlm.nih.gov/19122520/ (accessed 2026-10-30).
[^4]: A purified membrane protein from Akkermansia muciniphila or the pasteurized bacterium improves metabolism in obese and diabetic mice (Nat Med 2017) — https://pubmed.ncbi.nlm.nih.gov/27892954/ (accessed 2026-10-30).
[^5]: Commensal Akkermansia muciniphila exacerbates gut inflammation in Salmonella Typhimurium-infected gnotobiotic mice (PLoS ONE 2013) — https://pubmed.ncbi.nlm.nih.gov/24040367/ (accessed 2026-10-30).
[^6]: Faecalibacterium prausnitzii is an anti-inflammatory commensal bacterium identified by gut microbiota analysis of Crohn disease patients (PNAS 2008) — https://pubmed.ncbi.nlm.nih.gov/18936492/ (accessed 2026-10-30).
[^7]: Bifidobacteria and Butyrate-Producing Colon Bacteria: Importance and Strategies for Their Stimulation in the Human Gut (Front Microbiol 2016) — https://pubmed.ncbi.nlm.nih.gov/27446020/ (accessed 2026-10-30).
[^8]: Widely Used Commercial ELISA Does Not Detect Precursor of Haptoglobin2, but Recognizes Properdin as a Potential Second Member of the Zonulin Family (Front Endocrinol 2018) — https://pubmed.ncbi.nlm.nih.gov/29459849/ (accessed 2026-10-30).
[^9]: A fast, cheap, and easy protocol for celiac disease HLA haplotype typing using buccal swabs (Methods Cell Biol 2023) — https://pubmed.ncbi.nlm.nih.gov/37625876/ (accessed 2026-10-30).
[^10]: Effective detection of human leukocyte antigen risk alleles in celiac disease using tag single nucleotide polymorphisms (PLoS ONE 2008) — https://pubmed.ncbi.nlm.nih.gov/18509540/ (accessed 2026-10-30).
[^11]: Cost-effective HLA typing with tagging SNPs predicts celiac disease risk haplotypes in the Finnish, Hungarian, and Italian populations (Immunogenetics 2009) — https://pubmed.ncbi.nlm.nih.gov/19255754/ (accessed 2026-10-30).
[^12]: ESPGHAN guidelines for the diagnosis of coeliac disease (J Pediatr Gastroenterol Nutr 2012) — https://pubmed.ncbi.nlm.nih.gov/22197856/ (accessed 2026-10-30).
[^13]: ESPGHAN Guidelines for Diagnosing Coeliac Disease 2020 (J Pediatr Gastroenterol Nutr) — https://pubmed.ncbi.nlm.nih.gov/31568151/ (accessed 2026-10-30).
[^14]: The GenoChip: a new tool for genetic anthropology (Genome Biol Evol 2013) — https://pubmed.ncbi.nlm.nih.gov/23666864/ (accessed 2026-10-30).
[^15]: Mitochondrial DNA Haplogroup K Is Protective Against Autism Spectrum Disorder Risk (JAACAP 2024) — https://pubmed.ncbi.nlm.nih.gov/38072244/ (accessed 2026-10-30).
[^16]: Examining the role of common and rare mitochondrial variants in schizophrenia (PLoS ONE 2018) — https://pubmed.ncbi.nlm.nih.gov/29370225/ (accessed 2026-10-30).
[^17]: The association between common vitamin D receptor gene variations and osteoporosis: a participant-level meta-analysis (Ann Intern Med 2006) — https://pubmed.ncbi.nlm.nih.gov/16908916/ (accessed 2026-10-30).
[^18]: BsmI, TaqI, ApaI and FokI polymorphisms in the vitamin D receptor (VDR) gene and risk of fracture in Caucasians: a meta-analysis (Bone 2011) — https://pubmed.ncbi.nlm.nih.gov/20601302/ (accessed 2026-10-30).
[^19]: Do Vitamin D receptor gene polymorphisms affect bone mass density in men? (Ageing Res Rev 2022) — https://pubmed.ncbi.nlm.nih.gov/35063697/ (accessed 2026-10-30).
[^20]: Common genetic determinants of vitamin D insufficiency: a genome-wide association study (Lancet 2010) — https://pubmed.ncbi.nlm.nih.gov/20541252/ (accessed 2026-10-30).
[^21]: A second common mutation in the methylenetetrahydrofolate reductase gene: an additional risk factor for neural-tube defects? (Am J Hum Genet 1998) — https://pubmed.ncbi.nlm.nih.gov/9545395/ (accessed 2026-10-30).
[^22]: MTHFR 677C-->T polymorphism and risk of coronary heart disease: a meta-analysis (JAMA 2002) — https://pubmed.ncbi.nlm.nih.gov/12387655/ (accessed 2026-10-30).
[^23]: ACMG Practice Guideline: lack of evidence for MTHFR polymorphism testing (Genet Med 2013) — https://pubmed.ncbi.nlm.nih.gov/23288205/ (accessed 2026-10-30).
[^24]: Proposed guidelines to evaluate scientific validity and evidence for genotype-based dietary advice (Genes Nutr 2017) — https://pubmed.ncbi.nlm.nih.gov/29270237/ (accessed 2026-10-30).
[^25]: APOA2, dietary fat, and body mass index: replication of a gene-diet interaction in 3 independent populations (Arch Intern Med 2009) — https://pubmed.ncbi.nlm.nih.gov/19901143/ (accessed 2026-10-30).
[^26]: Apolipoprotein A2 polymorphism interacts with intakes of dairy foods to influence body weight in 2 U.S. populations — https://pubmed.ncbi.nlm.nih.gov/24108135/ (accessed 2026-10-30).
[^27]: Adiposity-related evidence for APOA2, FTO, and MC4R: a PRISMA-ScR scoping review of recent human studies (2019-2025) — https://pubmed.ncbi.nlm.nih.gov/42950483/ (accessed 2026-10-30).
[^28]: Genes involved in the regulation of intestinal permeability and their role in ulcerative colitis (J Dig Dis 2016) — https://pubmed.ncbi.nlm.nih.gov/26512799/ (accessed 2026-10-30).
[^29]: Polymorphisms in E-cadherin (CDH1) result in a mis-localised cytoplasmic protein that is associated with Crohn's disease (Gut 2009) — https://pubmed.ncbi.nlm.nih.gov/19398441/ (accessed 2026-10-30).
[^30]: Polygenic Risk Scores for Cardiovascular Disease: A Scientific Statement From the American Heart Association (Circulation 2022) — https://pubmed.ncbi.nlm.nih.gov/35862132/ (accessed 2026-10-30).
[^31]: Clinical use of current polygenic risk scores may exacerbate health disparities (Nat Genet 2019) — https://pubmed.ncbi.nlm.nih.gov/30926966/ (accessed 2026-10-30).
