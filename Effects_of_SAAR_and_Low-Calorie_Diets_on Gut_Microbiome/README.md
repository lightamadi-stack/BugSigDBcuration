# Differential Effects of Sulfur Amino Acid-Restricted and Low-Calorie Diets on Gut Microbiome Profile and Bile Acid Composition in Male C57BL6/J Mice

## Full Citation
Nichenametla, S. N., Mattocks, D. A. L., Midya, V., & Shneyder, J. (2021). *Differential Effects of Sulfur Amino Acid-Restricted and Low-Calorie Diets on Gut Microbiome Profile and Bile Acid Composition in Male C57BL6/J Mice*. Journals of Gerontology: Biological Sciences, 76(11) DOI: https://doi.org/10.1093/gerona/glaa270

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/33106871)

---

## 📘Study Overview
This study investigated whether sulfur amino acid restriction (SAAR) — specifically methionine restriction in the absence of cysteine alters the gut microbiome composition in male C57BL/6J mice, and whether any such changes are distinct from those induced by a mild caloric restriction. Three diet groups were compared: a control diet (CD; 0.86% methionine, ad libitum), an SAAR diet (0.12% methionine, ad libitum), and a low-calorie diet (LCD; same formula as CD but pair-fed to match SAAR caloric intake). Fecal microbiome profiles were determined after 10 weeks on the respective diets using 16S rRNA amplicon sequencing (V4 region). The study also measured plasma bile acid profiles as a marker of microbial metabolism, though bile acid data were not curated into BugSigDB (metabolic/functional data, not taxon-level signatures).

---

## 🧪Study Design
- Design type: Lab experiment (controlled dietary intervention in inbred laboratory mice; single terminal endpoint)
- Host species: Mus musculus (C57BL/6J, male, 21 weeks old at diet start)
- Sample size: 7–9 per group (exact per-group n not reported; range given uniformly across all figures)
- Groups compared:
    - Control diet (CD): 0.86% methionine, no cysteine, ad libitum
    - Sulfur amino acid-restricted diet (SAAR): 0.12% methionine, no cysteine, ad libitum
    - Low-calorie diet (LCD): CD formula, pair-fed to ~88% of CD caloric intake
Matching variables: Age (21 weeks at randomization), sex (all male), strain (C57BL/6J), housing conditions (individual polycarbonate cages, same room, controlled humidity/temperature/light cycle)

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: Low-calorie diet (Group 0) vs. Sulfur amino acid-restricted diet (Group 1)
- Sample size: Group 0 (LCD): n = 7–9; Group 1 (SAAR): n = 7–9
- Statistical method: One-way ANOVA + Tukey's multiple comparison test (phylum/family/species)
- Source figures/tables: Figure 3A - 3I, and Text description (Results)

### 🦠 Differentially Abundant Taxa
*see https://bugsigdb.org/33106871*

### ⚗️Experiment 2
- Comparison: Control diet (Group 0) vs. Sulfur amino acid-restricted diet (Group 1)
- Sample size: Group 0 (CD): n = 7–9; Group 1 (SAAR): n = 7–9
- Statistical method: One-way ANOVA + Tukey's multiple comparison test (phylum/family/species)
- Source figures/tables: Figure 3D, 3G, and Text description (Results)

### 🦠 Differentially Abundant Taxa
*see https://bugsigdb.org/33106871*

### ⚗️Experiment 3
- Comparison: Control diet (Group 0) vs. Low-calorie diet (Group 1)
- Sample size: Group 0 (CD): n = 7–9; Group 1 (SAAR): n = 7–9
- Statistical method: One-way ANOVA + Tukey's multiple comparison test (phylum/family/species)
- Source figures/tables: Figure 3E, 3H, and Text description (Results)

### 🦠 Differentially Abundant Taxa
*see https://bugsigdb.org/33106871*

---

## 🔢Statistical Analyses
- Primary tests used for curation: One-way ANOVA followed by Tukey's multiple comparison test — applied to percent abundance of OTUs at phylum, family, and species level (GraphPad Prism 8)
- Significance threshold: p < 0.05 
- Multiple testing correction: Benjamini-Hochberg FDR correction applied to robust linear regression p-values (OTU level)

---

## ✏️Curation Notes
- Two separate experiments were created despite both statistical test comparing the same groups (PCOS vs. controls) and were not fully overlapping, per BugSigDB policy.
    - Mann-Whitney and LEfSe use distinct statistical frameworks and report at different taxonomic resolutions — Mann-Whitney stops at family level while LEfSe resolves to genus level in several chains
    - Antibiotic use within 3 months was an explicit exclusion criterion for all participants recorded as "yes" for both experiments per BugSigDB curation policy.

---

## 🗃️Metadata
- Host: Mus musculus (C57BL/6J, male)
- Body site: Feces
- Environment: Controlled laboratory animal facility (conventional housing, individual cages)
- Sequencing platform: Illumina MiSeq (16S rRNA gene, V4)

---

## 🧾Curation Summary
This curation involved a three-arm dietary intervention study in male C57BL/6J mice, generating three pairwise curatable experiments from a single study design. Key learning points from this curation included: 
- Distinguishing pairwise from one-vs-all designs; correctly inferring study design from the actual analytical approach rather than author self-labeling.
- Applying the distinction between actual and potential confounders; understanding that percentage abundance is a compositional rescaling and not a log transformation.
The study contributes three sets of microbial signatures associated with methionine restriction and caloric restriction in a mouse model, with the SAAR vs. LCD comparison being the most data-rich experiment and the primary contribution to BugSigDB from this paper
