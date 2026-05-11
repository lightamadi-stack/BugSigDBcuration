# Blood Bacterial 16S rRNA Gene Alterations in Women with Polycystic Ovary Syndrome

## Full Citation
Wang Q., Wang Q., Zhao L., Bin Y., Wang L., Wang L., Zhang K., Li Q. (2022). *Blood Bacterial 16S rRNA Gene Alterations in Women with Polycystic Ovary Syndrome*. Frontiers in endocrinology Volume 13, Article 81452 
DOI: https://doi.org/10.3389/fendo.2022.814520

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/35282443)

---

## 📘Study Overview
This study investigated the blood microbiome profile of women with polycystic ovary syndrome (PCOS) compared to healthy controls using 16S rRNA gene sequencing. It is the first study to characterize the circulating (blood) microbiome in PCOS, as previous microbiome research in this condition focused primarily on the gut and saliva. The study measured alpha and beta diversity, identified differentially abundant taxa using Mann-Whitney U-test and LEfSe, and performed KEGG functional pathway prediction at the genus level.

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

### 🦠 Differentially Abundant Taxa
- Increased in Abnormal sperm results (Case)
      - *Peptoniphilus coxii*
- Increased in Normal sperm results (Control)
      - *Staphylococcus hominis*

### ⚗️Experiment 2
- Comparison: Normal sperm motility vs. abnormal sperm motility (n = 46 vs. n = 27)
- Sample size: 46 vs 27
    * Group 0 (normal sperm motility) n = 46
    * Group 1 (abnormal sperm motility) n = 27
- Statistical method: ANCOM-BC

### 🦠 Differentially Abundant Taxa
- Increased in Abnormal Sperm motility (Case)
      - *Lactobacillus iners*
- Increased in Normal sperm motility (Control)
      - No taxa met the significance threshold in this direction

### ⚗️Experiment 3
- Comparison: Normal sperm concentration vs. abnormal sperm concentration (n = 53 vs. n = 20)
- Sample size: 53 vs 23
    * Group 0 (normal sperm concentration) n = 53
    * Group 1 (abnormal sperm concentration) n = 20
- Statistical method: ANCOM-BC

### 🦠 Differentially Abundant Taxa
- Increased in Abnormal sperm concentration (Case)
      - *Pseudomonas fluorescens*
      - *Pseudomonas stutzeri*
      - *Paraburkholderia phenazinium*
- Increased in Normal sperm concentration (Control)
      - *Pseudomonas putida*

---

## 🔢Statistical Analyses
- Primary tests used for curation: ANCOM-BC (Analysis of Composition of Microbiomes with Bias Correction) for differential abundance
- Significance threshold: p < 0.05 (unadjusted)
- Multiple testing correction: None applied to ANCOM-BC output p-values. The authors explicitly stated: "less stringent parameters were used to maximize detection of possible discriminatory taxa (no p-value correction)

---

## 🗂️Data Sources
- Figure 3A-C and Supplementary Table 5

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Beta diversity results.
- Relative abundance bar charts: Figures 2, Supplementary Figures 3 and 4,  descriptive visualizations of top 30 species with no significance annotations; no taxa meet the significance threshold in these figures.
- Canonical Correlation Analysis: Table 2 and Figure 4. CCA is a community-level continuous association method, not a discrete differential abundance test. Results do not constitute curatable group-level signatures.
- Supplementary Tables 1–4 and 6: Participant demographics, sequence depth statistics, and CCA constraining variables, no taxon-level differential abundance results.

---

## ✏️Curation Notes
- Study design: Labeled as cross-sectional because no longitudinal follow-up or intervention occurred.
- Data transformation: ANCOM-BC takes raw count data as input by convention; the paper does not explicitly state the input format. Raw counts were recorded as the data transformation per the standard default mapping for ANCOM-BC, with a note that this was inferred rather than explicitly confirmed.
- Alpha diversity metric mapping: Hill1 diversity was mapped to Shannon (Hill q=1 = exp(Shannon entropy)); phylogenetic Hill1 diversity has no direct BugSigDB equivalent and was flagged for reviewer verification.

---

## 🗃️Metadata
- Host: Homo sapiens
- Disease/Condition: Male infertility (Abnormal semen parameters: mobility and/or concentration)
- Environment: Semen
- Sequencing platform: Illumina MiSeq (16S rRNA gene, V1–V2)

---

## 🧾Curation Summary
This curation involved a cross-sectional semen microbiome study with three distinct group comparisons derived from the same participant cohort. Key learning points included:
- Mapping non-standard alpha diversity metrics (Hill numbers) to BugSigDB-recognized equivalents.
- Recognizing that canonical correlation analysis results, while biologically informative, do not qualify as curatable differential abundance signatures.

The study contributes **seven species-level signatures** across **three semen microbiome** comparisons to BugSigDB, representing the largest semen microbiome dataset curated to date and the first BugSigDB entries linking *Lactobacillus iners* and *Pseudomonas* species to male sperm parameter abnormalities.

