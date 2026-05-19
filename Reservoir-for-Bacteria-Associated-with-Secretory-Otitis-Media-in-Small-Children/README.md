# The Adenoids but Not the Palatine Tonsils Serve as a Reservoir for Bacteria Associated with Secretory Otitis Media in Small Children

## Full Citation
Fagö-Olsen H., Dines L.M., Sørensen C.H., Jensen A. (2019). *The Adenoids but Not the Palatine Tonsils Serve as a Reservoir for Bacteria Associated with Secretory Otitis Media in Small Children*. mSystems Volume 4 Issue 1 e00169-18.  DOI: https://doi.org/10.1128/mSystems.00169-18

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/30801022)

---

## 📘Study Overview
Study Overview
This study investigated the association between gut microbiota composition and high-grade prostate cancer (PCa) in Japanese men. 152 men suspected of PCa undergoing prostate biopsy were recruited across three hospitals in Osaka, Japan. Rectal swab samples were collected before biopsy and analyzed using 16S rRNA gene sequencing (V1–V2 region). Participants were divided into a high-risk group (Grade Group ≥ 2 PCa) and a negative + low-risk group (negative biopsy or Grade Group 1 PCa). The study also developed a composite predictive index — the Fecal Microbiome Prostate Index (FMPI) — from 18 LASSO-selected bacterial genera, which outperformed PSA testing in detecting high-risk PCa.

---

## 🧪Study Design
- Design type: Cross-sectional observational, not case-control. *Although groups were defined by disease status, all participants were enrolled under the same criterion (suspected PCa, undergoing biopsy) at a single time point. Group membership was determined retrospectively after biopsy results, with no deliberate case/control recruitment, no matching, and no follow-up. The microbiome data were analyzed at one time point only*.
- Host species: Homo sapiens
- Sample size: 152 total (discovery cohort: n = 114; external test cohort: n = 38)
- Groups compared:
    - Men with prostate cancer (PCa) and positive biopsy *(Group 1)* VS Men without prostate cancer (PCa) and negative biopsy *(Group 0)*
    - Men with grade group 2 or higher risk prostate cancer (PCa) *(Group 1)* VS men with negative and low risk group *(Group 0)
Confounders reported/controlled: Age and PSA were significantly higher in the high-risk group (Table 1). BMI, family history, LUTS, smoking, alcohol consumption, dietary habits, diabetes, hypertension, and dyslipidemia did not differ significantly between groups. *The LEfSe differential abundance analyses did not adjust for age or PSA.*

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Group 2 or High risk prostate cancer (PCa) vs Negative and low risk group 
- Sample size: 58 vs 56
- Statistical method: LEfSe
- Source figures/tables: Figure 3A

### 🦠 Differentially Abundant Taxa
- Increased in PCOS (Case)
      - *Alistipes*, *Christensenellaceae*, *Lachnobacterium*, *Lachnospira* etc. 
- Increased in negative and low risk group
      - *None reported (all significant taxa were enriched in the high-risk group)*

### ⚗️Experiment 2
- Comparison: Prostate cancer (PCa) and positive biopsy vs No prostate cancer (PCa) and negative biopsy 
- Sample size: 72 vs 42
- Statistical method: LEfSe
- Source figures/tables: Supplementary Figure S2

### 🦠 Differentially Abundant Taxa
- Increased in PCOS (Case)
      - *Alistipes*, *Lachnospira*, *Odoribacteraceae* etc
- Increased in no prostrate cancer and negative biopsy
      - *None reported (all significant taxa were enriched in prostate cancer group)*

---

## 🔢Statistical Analyses
- Primary tests used for curation:
      - LEfSe (for differential abundance) for both Experiment 1 and Experiment 2
- Significance threshold:
    - p < 0.05
    - LDA > 2.0 for LEfSe
- Multiple testing correction: None

## Alpha Diversity
- Metrics reported: Shannon and Richness
- Direction of change: Unchanged (Not significant)

---

## 🗂️Data Sources
- Figure 3A and Supplementary Figure S2

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Figure S2B (metastasis vs. no metastasis dot plots): The paper explicitly states no significant difference was found between PCa patients with and without metastasis for Rikenellaceae, Alistipes, or Lachnospira. No p-values or significance markers appear on the figure. Not curatable.
- Table 2 (LASSO-selected taxa for FMPI): Excluded because LASSO is a predictive variable selection method, not a differential abundance test. No per-taxon p-values or significance thresholds were applied to the 18 selected genera individually. The FMPI composite score was statistically validated, but composite significance does not equal individual taxon significance. BugSigDB requires individually statistically significant taxa.
- Table 3 (logistic regression for FMPI): Reports FMPI as a composite predictor of high-risk PCa. Not a taxon-level result.
- Table 4 (summary of bacterial roles): Narrative classification of bacterial functions — not a results table with significance data.
- ROC/AUC analyses (Figure 4) were excluded because they assess predictive performance, not differential microbial abundance.
- Figure 3B and Figure S2C (KEGG pathway analyses): Functional/metabolic pathway results. BugSigDB captures taxon-level signatures only. Pathway findings were noted but fully excluded from all experiments and figures per curation policy.

---

## ✏️Curation Notes
- Discovery vs. test cohort: Only the discovery cohort produced curatable differential abundance experiments (LEfSe analyses). The test cohort was used for predictive validation only and generated no independently curatable experiments.
- Figure S2B deliberation: I initially flagged it as potentially curatable (metastasis comparison). But confirmed non-curatable after cross-checking both the figure (no significance markers) and the main text, which explicitly states no significant difference was found.
- Antibiotic exclusion: Confirmed — men who used antibiotics within 6 months or whose antibiotic history was unknown were excluded at enrollment. This satisfies BugSigDB's antibiotic exclusion criterion.
- Unannotated OTUs: Two OTUs in Figure 3A and one in Figure S2A had no taxonomic annotation. These were excluded from curation as BugSigDB requires valid taxon names resolvable in NCBI Taxonomy.

---

## 🗃️Metadata
- Host: Homo sapiens (Japanese men, urban Osaka)
- Disease/Condition: Prostate cancer
- Body site: Rectum
- Sequencing platform: Illumina MiSeq; 16S rRNA gene, V1–V2 variable region; 251-bp paired-end; OTU clustering at 97% similarity via UCLUST; annotated with RDP Classifier v2.2 against Greengenes 13_8

---

## 🧾Curation Summary
This curation required several rounds of careful decision-making that deepened my understanding of BugSigDB policy application. The most instructive challenge was distinguishing study design: the study appeared case-control at first glance but was correctly reclassified as cross-sectional observational after close reading of the enrollment and grouping methods. 

A second major decision involved the LASSO-derived Table 2, which went through two reversals before being firmly excluded — this process clarified a fundamental principle: composite model significance does not substitute for individual taxon-level significance, and BugSigDB strictly requires the latter. The metastasis comparison (Figure S2B) required cross-checking both the figure and the main text to confirm non-significance. This study also reinforced the importance of NCBI taxonomy modernization, as the Greengenes database used by the authors employs phylum names now replaced under current nomenclature. 

Overall, this curation contributed two experiments to BugSigDB capturing gut microbial signatures associated with high-grade prostate cancer in a Japanese cohort, a population and cancer type underrepresented in the existing database.

