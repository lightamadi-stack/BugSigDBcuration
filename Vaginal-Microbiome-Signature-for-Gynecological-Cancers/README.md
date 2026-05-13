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
- Comparison: All gynecological cancer vs. healthy controls
- Sample size: 348 vs 181
- Statistical method: Wilcoxon rank-sum test (ASV level; P < 0.01 and log fold-change > 2.0) + LEfSe (phylum and genus level; LDA score > 2)
- Source figures/tables: Figure 2i (LEfSe, phylum level), Figure 2j (LEfSe, genus level)

### 🦠 Differentially Abundant Taxa
- Increased in PCOS (Case)
      - *Proteobacteria*, *Prevotella*, *Staphylococcus* etc.
- Increased in Healthy Controls
      - *Firmicutes*, *Lactobacillus*, *Atopobium* etc

### ⚗️Experiment 2 - 4
- Comparison: Three-way: CC vs. OC vs. EC (each cancer type treated as case against the other two combined as reference) 
- Sample size:
      - CC (n = 161) vs. OC + EC (n = 172)
      - OC (n = 71) vs. CC + EC (n = 262)
      - EC (n = 101) vs. CC + OC (n = 232)
- Statistical method: Wilcoxon rank-sum test (ASV level; P < 0.01 and log fold-change > 2.0) + LEfSe (phylum and genus level; LDA score > 2)
- Source figures/tables: Figure 5g (LEfSe, phylum level), Figure 5h (LEfSe, genus level)

### 🦠 Differentially Abundant Taxa
*(see the full list in: https://bugsigdb.org/38633411)*

---

## 🔢Statistical Analyses
- Primary tests used for curation:
      - LEfSe (phylum and genus level)
- Significance threshold:
    - p < 0.05 and LDA > 2 
- Multiple testing correction: Not reported for any differential abundance analysis

---

## 🗂️Data Sources
- Figure 2i, 2j, 5g, 5h

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Figure 1 (pre- vs. post-menopausal comparison)No significant taxa, all results marked "NotSig" (green dots) in Wilcox plot (Figure 1g).
- Figure 4 + Table 2 (random forest model)Machine learning feature importance scores not differential abundance statistics; not curatable per BugSigDB policy.
- Figure 6 (co-abundance network)Spearman correlation network topology, not taxon-level differential abundance; not curatableAll PCA / beta diversity plots.
- Figures 1e–f, 2f–g, 3d–f, 5e–f)Beta diversity results explicitly excluded per BugSigDB curation policyFigure.

---

## ✏️Curation Notes
- Study design decision logic: The study pools raw 16S rRNA-seq data from 10 independent public BioProjects and re-analyzes them as a single dataset. This was classified as *meta-analysis* under BugSigDB controlled vocabulary, as it synthesizes multiple primary studies. In this study, the authors re-analyze raw data (rather than synthesizing reported results).
- Sequencing platform: Not explicitly named in the paper despite searching all Methods sections. Thus, papers (the 10 source BioProjects) used in this meta analysis were checked individually and I found that Illumina was the sequencing platform used.
- Confounder handling: Menopausal status was the only variable examined analytically (sub-analysis, Figure 1), and found non-significant (P = 0.611). It was not adjusted for in any model. No other variables were controlled for. Hence, no confounders was controlled.
- Three-group LEfSe (Experiment 2): BugSigDB expects pairwise case/control contrasts. The three-group LEfSe in Figure 5g/5h produces one-vs-others enrichments rather than strict pairwise comparisons. Each cancer type's enriched taxa were treated as a separate sub-experiment with the other two cancer types combined as reference.
- Alpha diversity direction (Experiment 2): For OC and EC sub-experiments, the significant bracket (EC vs. OC, **) shows a clear direction between those two groups, but neither is significantly different from CC. This creates an inconsistent direction when the two reference groups are combined. I raised a question with the reviewer for guidance on how to record this. And i was told to leave all alpha diversity blank in the case of meta analysis.

---

## 🗃️Metadata
- Host: Homo sapiens
- Disease/Condition: Gynecological cancer (pooled: cervical cancer, ovarian cancer, endometrial cancer, and other gynecological cancers)
- Body site: Vagina
- Environment: Clinical (hospital-based recruitment, First Affiliated Hospital of Xi'an Jiaotong University, China)
- Sequencing platform: Illumina MiSeq (16S rRNA gene, V2–V5)

---

## 🧾Curation Summary
This curation involved a methodologically complex study due to its pooled secondary analysis design, multi-cancer scope, and three-group comparisons. Key learning points included: 
- Distinguishing between primary cohort studies and secondary pooled analyses for study design classification.
- Applying careful judgment about which figures contain statistically significant taxon-level results versus descriptive composition plots.
- Curating numerous taxa from three-group LEfSe comparisons.
- Identifying when alpha diversity directions are ambiguous due to inconsistent pairwise significance and escalating that appropriately to a reviewer rather than making an unsupported inference.
