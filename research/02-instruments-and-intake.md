# 02 — Instruments and Intake Formats

## Summary

ESPERANTO is organized as three instruments over one client record: COGENT reads consumer genotyping chips and whole-genome VCFs against a curated 4,500+ functional-SNP panel; FLORIAN reads stool reports against a 22,800-taxon knowledge base; KINESIS reads organic acids, hormones, amino acids, fatty acids, elements, food-antibody panels and routine blood work against 390 explained markers and 3,200+ metabolites.[1] The landing page's client vault lists **81 named report formats** that are "read exactly," plus a model-assisted fallback for other lab PDFs in which values are checked against the page after de-identification.[1]

## COGENT (genome)

Upload a consumer chip (23andMe, AncestryDNA, MyHeritage, and similar services) or a whole-genome VCF (Dante, Nebula / DNA Complete, Sequencing.com, Veritas, and others — by download link or upload, processed in the background).[1]
COGENT reads the file against more than 4,500 functional SNPs, hundreds of multi-SNP algorithms and polygenic risk scores, offering: a SNP viewer with plain-language interpretation; diagnoses traced back to the patient's own variants; drug–gene interactions and ClinVar findings; and ABO, secretor (FUT2) and Lewis status.[1]
Whole-genome uploads retain every variant, are screened against ClinVar, and fill sites a chip cannot answer.[1]
The genome intake list also covers FamilyTreeDNA, Living DNA, SelfDecode, two discontinued services' exports (Genos; DSL's Opus Chip) and Illumina array final reports.[1]

## FLORIAN (gut microbiome)

FLORIAN is built on a 22,800-taxon knowledge base and reads 16S reports (Thryve, BiomeSight, legacy uBiome JSON) and Diagnostic Solutions' GI-MAP stool qPCR, among others.[1] It identifies organisms that matter, sets remodeling targets, ranks foods, nutraceuticals and diets by how they act on those organisms, lists indicated agents/substrates/growth factors, and tracks antibiotic-resistance genes.[1] The vault's microbiome intake list further includes shotgun-metagenomic PDFs from Tiny Health and Jona Health, Viome Gut Intelligence, Genova GI Effects, Vibrant Gut Zoomer, Doctor's Data Comprehensive Stool Analysis, BioHealth SIBO breath tests, DiagnosTechs GI/parasitology panels, and generic stool culture-and-sensitivity reports.[1]

## KINESIS (metabolome and labs)

KINESIS reads organic acids, hormones, amino acids, fatty acids, elements, food antibodies and routine blood work, explaining 390 markers against a 3,200+-metabolite library; every marker opens a full metabolite page with the genes behind it checked against the patient's own genome, and gut-related markers are cross-checked against FLORIAN.[1]
Named intake panels include: Mosaic OAT/MOAT/TOXDetect/MycoTOX and the Omega-3 Index; DUTCH hormone tests; Genova NutrEval, Metabolomix+, Organix, Cardio Check, IgE/IgG food antibodies, Thyroid Plus and One Day Hormone Check; DiagnosTechs ASI and expanded hormone/bone/food panels plus elemental testing; ZRT saliva, blood-spot and dried-urine assays; Vibrant Wheat and Cellular Zoomer; Boston Heart CVMap; Viome recommendation reports; the Mitome mitochondrial cheek-swab analysis; Quicksilver Mercury Tri-Test; Sabre Sciences HPA-4; Cyrex Arrays 2, 3X, 4, 5, 8, 10, 11, 12 and 20; the Diagnostic Solutions OAp organic-acids profile; Doctor's Data RBC elements; and the Precision Point P88 dietary antigen test.[1]
Routine chemistry flows in from Quest, Labcorp, Epic MyChart and Cerner portal PDFs, plus FHIR JSON from portals, Apple Health or an EHR.[1]
The FAQ confirms the same list and adds that any unlisted report "is read by the AI, which reports back what it found."[1]

## Reading quality and trending

The landing page claims the exact reader parses supported formats "line by line in about a second — no typing, no transcription errors, no guesswork," while unlisted labs' PDFs go through model-assisted extraction with the patient's details removed first and every value verified against the report before saving.[1] KINESIS tracks every marker across draws and across labs — "the direction of travel is part of the reasoning, and a single draw is treated as a single draw."[1]

## Cross-omics connections (marketing examples)

The landing page gives concrete examples of automatic cross-instrument links: a low 2-OH/4-OH estrogen ratio shown beside the patient's CYP1B1 variants; a high DHPPA checked against the bacteria that make it; urinary arsenic lined up with the energy-cycle markers it blocks.[1] KINESIS pathway maps display flagged metabolites beside the patient's variant genes.[1]

## Sources

[1] https://www.datapunk.net — OPUS23 | ESPERANTO · Datapunk Bioinformatics (platform landing page)
