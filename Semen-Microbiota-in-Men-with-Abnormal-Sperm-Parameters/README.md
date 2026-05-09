# Semen Microbiota are Dramatically Altered in Men with Abnormal Sperm Parameters

## Full Citation
Vadim Osadchiy, Andre Belarmino, Reza Kianian, John T. Sigalos, Jacob S. Ancira, Trisha Kanie, Sarah F. Mangum, Craig D. Tipton, Tung-Chin M. Hsieh, Jesse N. Mills & Sriram V. Eleswarapu (2024). *Semen microbiota are dramatically altered in men with abnormal sperm parameters*. Scientific Reports volume 14, Article number: 1068 DOI: https://doi.org/10.1038/s41598-024-51686-4

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/38212576)

---

## 📘Study Overview
This study investigated the relationship between the semen microbiome and alterations in sperm parameters in men presenting for fertility evaluation or vasectomy consultation. Using 16S rRNA sequencing (V1–V2) and ANCOM-BC differential abundance testing, the authors compared semen microbial communities across three a priori defined group contrasts: overall semen analysis parameters, sperm motility, and sperm concentration. The study is the largest semen microbiome study published to date (n = 73) and identified a small set of microbial species — notably Lactobacillus iners and members of the genus Pseudomonas — as potentially associated with abnormal sperm parameters.

---

## 🧪Study Design
- Design type: Cross-sectional observational study, not case-control.
- Host species: Homo sapiens
- Sample size: 73 total participants (men)
- Groups compared:
    - Group 1: Normal SA parameters vs. abnormal SA parameters (n = 42 vs. n = 31)
    - Group 2: Normal sperm motility vs. abnormal sperm motility (n = 46 vs. n = 27)
    - Group 3: Normal sperm concentration vs. abnormal sperm concentration (n = 53 vs. n = 20)

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Normal sperm results vs. abnormal sperm results
- Sample size: 42 vs 21
    * Group 0 (normal sperm results) n = 42
    * Group 1 (abnormal sperm results) n = 31
- Statistical method: ANCOM-BC

### ⚗️Experiment 2
- Comparison: Normal sperm motility vs. abnormal sperm motility (n = 46 vs. n = 27)
- Sample size: 46 vs 27
    * Group 0 (normal sperm motility) n = 46
    * Group 1 (abnormal sperm motility) n = 27
- Statistical method: ANCOM-BC

### ⚗️Experiment 3
- Comparison: Normal sperm concentration vs. abnormal sperm concentration (n = 53 vs. n = 20)
- Sample size: 53 vs 23
    * Group 0 (normal sperm concentration) n = 53
    * Group 1 (abnormal sperm concentration) n = 20
- Statistical method: ANCOM-BC

---

## 🔢Statistical Analyses
- Primary tests used for curation: ANCOM-BC (Analysis of Composition of Microbiomes with Bias Correction) for differential abundance
- Significance threshold: p < 0.05 (unadjusted)
- Multiple testing correction: None applied to ANCOM-BC output p-values. The authors explicitly stated: "less stringent parameters were used to maximize detection of possible discriminatory taxa (no p-value correction)

### Alpha Diversity
- Metrics reported:
    - OTU richness (mapped to Richness)
    - Hill1 diversity (mapped to Shannon)
    - Phylogenetic Hill1 diversity (has no direct BugSigDB equivalent; was flagged for reviewer verification)
- Direction of change: No significant differences across all three group comparisons
- Significance: All p > 0.10 across all groups and all three alpha diversity metrics

---

## 🗂️Data Sources
- Figure 3A-C and Supplementary Table 5

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Figure 1 (Kruskal–Wallis/Dunn test): Genus-level abundance summaries; not the primary DA test.
- Correlation analysis (SparCC): Did not report taxa-level differential abundance. 
- Non-significant taxa. For example, *Prevotella bivia* (Experiment 2, p adj = 0.353), explicitly does not meet FDR ≤ 0.05 threshold despite borderline raw p value of 0.050; excluded per curation policy
- Beta diversity results

---

## 🦠 Differentially Abundant Taxa

### See ➤ :[https://bugsigdb.org/31332740]

---

## ✏️Curation Notes
- Statistical test entry: Both DESeq2 and Wald test were entered as statistical tests. DESeq2 was named in the methods section; Wald test was explicitly named in Table 3 footnote ("Wald test p value"). BugSigDB curation policy permits multiple statistical test entries and both are directly stated in the paper.
- Intrapartum penicillin handling: 15 of 23 spontaneous preterm participants received intrapartum penicillin and were removed analytically before DESeq2 analysis. This is recorded as a confounder mitigation step, not as the enrollment antibiotic exclusion criterion. 

---

## 🗃️Metadata
- Host: Homo sapiens
- Disease/Condition: Premature birth
- Environment: Vagina (vaginal swab)
- Sequencing platform: Ion PGM (Thermo Fisher Scientific); 16S rRNA V4 region; primers 515F/806R; OTU clustering at 97% similarity; taxonomy assigned against SILVA database v128

---

## 🧾Curation Summary
This curation involved careful application of **BugSigDB curation policy** across several genuinely ambiguous decisions. Key learning points included: 
- Distinguishing between study design labels using precise policy definitions rather than how authors self-describe their study.
- Correctly applying FDR-adjusted versus raw p value thresholds for taxon inclusion.
- Understanding when to enter multiple statistical test entries.
- Handling analytical antibiotic exclusions separately from enrollment exclusions; and converting trimester-based antibiotic exclusion criteria to numeric entries with appropriate documentation.
 
This study contributes **two curatable experiments** to BugSigDB characterizing vaginal microbial signatures of spontaneous preterm birth in a Brazilian cohort, adding to the global evidence base for *Prevotella* as a risk-associated taxon and *Lactobacillus iners* and *Lactobacillus jensenii* as protective taxa in preterm birth microbiome research.

