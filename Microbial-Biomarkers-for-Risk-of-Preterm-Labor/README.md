# Defining Microbial Biomarkers for Risk of Preterm Labor

## Full Citation
de Freitas A.S., Dobbler P.C.T., Mai V., Procianoy R.S., Silveira R.C., Corso A.L., Roesch L.F.W. (2020). *Defining microbial biomarkers for risk of preterm labor*. Brazilian Journal of Microbiology 51:151–159   DOI: https://doi.org/10.1007/s42770-019-00118-

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/31332740)

---

## 📘Study Overview
This study investigated the association between vaginal microbiota composition and spontaneous preterm labor in a Brazilian cohort of 69 pregnant women. Using 16S rRNA sequencing of vaginal swabs collected up to 4 hours before labor, the authors aimed to identify microbial biomarkers that distinguish spontaneous preterm from term delivery outcomes, and evaluate potential confounders affecting microbial variation. The study is notable for its focus on a highly miscegenated Brazilian population, which had not previously been characterized for vaginal microbiome-preterm birth associations.

---

## 🧪Study Design
- Design type: Cross-sectional observational study, not case-control.
- Host species: Homo sapiens
- Sample size: 69 pregnant women
- Groups compared:
    - Spontaneous term labor (control) vs. spontaneous preterm labor (case)
    - Non-spontaneous preterm labor (control) vs. spontaneous preterm labor (case)
- Confounders reported/controlled: Intrapartum penicillin use (significant by PERMANOVA, R² = 0.034, p = 0.043; mitigated by removing affected samples before differential abundance analysis); maternal age, previous pregnancies, gestational age, chorioamnionitis, preeclampsia, GBS infection, and delivery mode were tested via PERMANOVA and found non-significant

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Spontaneous term labor (control) vs spontaneous preterm labor (case)
- Sample size: 29 vs 23
    * Group 0 (spontaneous term labor) n = 29
    * Group 1 (spontaneous preterm labors) n = 23; *Note: 15 spontaneous preterm labor cases received intrapartum penicillin and were removed before DESeq2 analysis thus, effective preterm n = 8, but the original sample size was curated*
- Statistical method: DESeq2 and Wald test with FDR correction
- Source: Table 3 


### ⚗️Experiment 2
- Comparison: Non-spontaneous preterm labor (control) vs spontaneous preterm labor (case)
- Sample size: Group 0 (non-spontaneous preterm) n = 17; Group 1 (spontaneous preterm) n = 23
- Statistical method: DESeq2 and Wald test with FDR correction
- Source: Table 3
*Note: Figure 1 and Figure 2 not curated because they do not provide species-level significant taxa under DESeq2*

---

## 🔢Statistical Analyses
- Primary tests used for curation: DESeq2 (negative binomial model) and Wald test for differential abundance analysis
- Significance threshold: FDR-adjusted p ≤ 0.05
- Multiple testing correction: FDR (Benjamini-Hochberg method) applied via DESeq2

---

## 🗂️Data Sources
- Table 3

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
