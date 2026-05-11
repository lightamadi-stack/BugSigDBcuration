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
- Design type: Case-control.
- Host species: Homo sapiens
- Sample size: 48 total (24 PCOS, 24 healthy controls)
- Groups compared:
    - Group 1: Women with newly diagnosed PCOS (Rotterdam criteria)
    - Group 2: Healthy women without history of PCOS 
Confounders reported/controlled: Age and BMI differed significantly between groups but were not adjusted for in any differential abundance analysis. No covariate adjustment was performed

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Polycystic Ovary Syndrome (PCOS) vs Healthy Controls 
- Sample size: 24 vs 24
- Statistical method: Mann–Whitney U-test
- Source figures/tables: Supplementary Figure S2 (family-level boxplots)
      - *Note: Figure 2A/B (phylum/order results) was not curated because Supplementary Figure S2 provides lower (more specific) family-level data, as required by BugSigDB policy.* 


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
      - *Note: Only the lowest (i.e. most specific) taxonomic rank was curated from figure 3A

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
- Figure 2A and Supplementary Figure S2

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Figure 2A/B: Not curated due to higher-level taxonomy (phylum/order). Supplementary S2 provided more specific family-level results for the same taxa.
- Figure 3B: Cladogram visualization of the same LEfSe results shown in Figure 3A; no unique taxa.
- KEGG pathway analysis: Excluded — functional pathways are not curated in BugSigDB.
- Alpha and Beta diversity analyses: Not curatable
- Supplementary Figure S1: Overall sequencing proportion by taxonomic level — excluded; no significant taxon-level contrast shown, descriptive only.

---

## ✏️Curation Notes
- Two separate experiments were created despite both statistical test comparing the same groups (PCOS vs. controls) and were not fully overlapping, per BugSigDB policy:
    - Mann-Whitney and LEfSe use distinct statistical frameworks and report at different taxonomic resolutions — Mann-Whitney stops at family level while LEfSe resolves to genus level in several chains
    - The resulting taxon lists are not fully overlapping *Veillonellaceae* for example, appear only in Mann-Whitney; *Skermanella*, *Rhodospirillales*, *Rhizobiales*, *Micrococcaceae*, and genus-level taxa appear only in LEfSe Per BugSigDB curation policy: *Curate as two different experiments when results are different (not fully overlapping) between the tests*.
- Family-level taxa in Supplementary Figure S2 were curated instead of phylum or order-level data from Figure 2, following the requirement to curate the lowest specific taxonomic rank.
- Antibiotic use within 3 months was an explicit exclusion criterion for all participants — recorded as "yes" for both experiments per BugSigDB curation policy.

---

## 🗃️Metadata
- Host: Homo sapiens
- Disease/Condition: Polycystic ovary syndrome (PCOS)
- Body site: Blood
- Environment: Clinical (hospital-based recruitment, First Affiliated Hospital of Xi'an Jiaotong University, China)
- Sequencing platform: Illumina MiSeq (16S rRNA gene, V3–V4)

---

## 🧾Curation Summary
This curation required carefully distinguishing between overlapping analyses and taxonomic levels. I applied BugSigDB rules to separate the study into two valid experiments: one based on Mann–Whitney family-level results and one based on LEfSe biomarker results. The process strengthened my understanding of hierarchical taxonomy decisions, experiment definition rules, and the use of the lowest available taxonomic level. and recognizing that uncontrolled confounders (age, BMI) are noted but not entered in the BugSigDB confounders field unless they were actually adjusted for in the model. The study also reinforced the importance of cross-referencing figure panels against text descriptions when discrepancies arise, as seen with Oxalobacteraceae and Bacteroidaceae. 

This curation contributes a clean, policy-compliant record of blood microbiome signatures associated with PCOS. This curation contributed to BugSigDB by adding the first blood microbiome study in PCOS, a body site and condition combination not previously represented in the database.
