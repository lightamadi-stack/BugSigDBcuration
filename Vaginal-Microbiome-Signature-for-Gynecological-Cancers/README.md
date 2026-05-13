# Highly Specific Vaginal Microbiome Signature for Gynecological Cancers

## Full Citation
Han M., Wang N., Han W., Liu X., Sun T., Xu J. (2024). *Highly Specific Vaginal Microbiome Signature for Gynecological Cancers*. Open life sciences  19: 2022085 DOI: https://doi.org/10.1515/biol-2022-0850

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/38633411)

---

## 📘Study Overview
This study investigated vaginal microbiome differences between women with gynecological cancers (cervical, ovarian, and endometrial) and healthy controls. The authors pooled publicly available 16S rRNA-seq data from 10 independent BioProjects (total N = 529), re-processed all raw sequencing data uniformly using VSEARCH and QIIME2, and performed differential abundance analysis, alpha/beta diversity comparisons, random forest classification, and co-abundance network analysis. The study aimed to identify a vaginal microbial signature specific to gynecological cancer and evaluate its potential as a non-invasive diagnostic biomarker.

---

## 🧪Study Design
- Design type: Meta-analysis (secondary pooled re-analysis of 10 published BioProjects).
- Host species: Homo sapiens
- Sample size: N = 529 total (*Gynca group*: n = 348; *Normal/Control group*: n = 181). Cancer subtypes: *cervical cancer* (CC, n = 161), *ovarian cancer* (OC, n = 71), *endometrial cancer* (EC, n = 101)
- Groups compared:
    - Group 1: All gynecological cancer (Gynca) vs. healthy controls (Normal)
    - Group 2: Three-way comparison: CC vs. OC vs. EC. 
Confounders reported/controlled: None statistically controlled. **Menopausal status** was the only variable examined — a sub-analysis (Figure 1) showed no significant difference in alpha or beta diversity between pre- and post-menopausal women within the Gynca group (P = 0.611), so all samples were pooled without adjustment. Age, BMI, HPV status, geographic origin, ethnicity, antibiotic use, and batch effects across the 10 BioProjects were not controlled for and are acknowledged as limitations.

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Polycystic Ovary Syndrome (PCOS) vs Healthy Controls 
- Sample size: 24 vs 24
- Statistical method: Mann–Whitney U-test
- Source figures/tables: Figure 2A, 2B, and Supplementary Figure S2 (phylum, order and family-level)

### 🦠 Differentially Abundant Taxa
- Increased in PCOS (Case)
      - *Intrasporangiaceae*, *Nocardioidaceae*, *Comamonadaceae* etc.
- Increased in Healthy Controls
      - *Burkholderiaceae*, *Lachnospiraceae*, *Lactobacillaceae* etc

### ⚗️Experiment 2
- Comparison: Polycystic Ovary Syndrome (PCOS) vs Healthy Controls 
- Sample size: 24 vs 24
- Statistical method: LEfSe (LDA > 3.0) 
- Source figures/tables: Figure 3A (LDA barplot)

### 🦠 Differentially Abundant Taxa
- Increased in PCOS (Case)
      - *Skermanella*, *Acinetobacter*, *Nocardioidaceae* etc
- Increased in Healthy Controls
      - *Burkholderia*, *Lactobacillus*, *Faecalibacterium*, etc

---

## 🔢Statistical Analyses
- Primary tests used for curation:
      - Mann–Whitney U-test (Experiment 1)
      - LEfSe (LDA > 3.0) (Experiment 2)
- Significance threshold:
    - p < 0.05 for Mann–Whitney
    - LDA > 3.0 and p < 0.05 for LEfSe
- Multiple testing correction: None

## Alpha Diversity
- Metrics reported: Faith’s PD, Chao1, Observed OTUs
- Direction of change: Significantly decreased in PCOS
- Significance: All metrics p < 0.001
- *Note: Alpha diversity was recorded as metadata for both experiments and was not curated as a separate experiment*

---

## 🗂️Data Sources
- Figure 2A, 2B, Figure 3A and Supplementary Figure S2

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Figure 3B: Cladogram visualization of the same LEfSe results shown in Figure 3A; no unique taxa.
- KEGG pathway analysis: Excluded — functional pathways are not curated in BugSigDB.
- Alpha and Beta diversity analyses: Not curatable
- Supplementary Figure S1: Overall sequencing proportion by taxonomic level, excluded; no significant taxon-level contrast shown, descriptive only.

---

## ✏️Curation Notes
- Two separate experiments were created despite both statistical test comparing the same groups (PCOS vs. controls) and were not fully overlapping, per BugSigDB policy.
    - Mann-Whitney and LEfSe use distinct statistical frameworks and report at different taxonomic resolutions — Mann-Whitney stops at family level while LEfSe resolves to genus level in several chains
    - Antibiotic use within 3 months was an explicit exclusion criterion for all participants recorded as "yes" for both experiments per BugSigDB curation policy.

---

## 🗃️Metadata
- Host: Homo sapiens
- Disease/Condition: Polycystic ovary syndrome (PCOS)
- Body site: Blood
- Environment: Clinical (hospital-based recruitment, First Affiliated Hospital of Xi'an Jiaotong University, China)
- Sequencing platform: Illumina MiSeq (16S rRNA gene, V3–V4)

---

## 🧾Curation Summary
This curation required carefully distinguishing between overlapping analyses and taxonomic levels. I applied BugSigDB rules to separate the study into two valid experiments: one based on Mann–Whitney family-level results and one based on LEfSe biomarker results. The process strengthened my understanding of hierarchical taxonomy decisions, experiment definition rules, and recognizing that uncontrolled confounders (age, BMI) are noted but not entered in the BugSigDB confounders field unless they were actually adjusted for in the model. The study also reinforced the importance of cross-referencing figure panels against text descriptions when discrepancies arise, as seen with Oxalobacteraceae and Bacteroidaceae. 

This curation contributes a clean, policy-compliant record of blood microbiome signatures associated with PCOS. This curation contributed to BugSigDB by adding the first blood microbiome study in PCOS, a body site and condition combination not previously represented in the database.

