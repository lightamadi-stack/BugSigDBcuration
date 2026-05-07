# Age Related Gut Microbiome and Links to Police Performance in Kunming Dogs

## Full Citation
Xu L., Liu C., Chen S., Mao A., Zi X., Li J., Ge X., Liu Q., Wang S., Li X., Wu Q., Wan J., Zhang Z., Xu H., Li J., Lin Q., Cao Z. (2026). *Characterization of age-related changes in the gut microbiome and metabolome of Kunming dogs and their associations with police performance*. Microbiome. 14:121 DOI: https://doi.org/10.1186/s40168-026-02388-8

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/41840712)

---

## 📘Study Overview
This study investigated how gut microbiome composition, metabolome, and functional pathways vary across age groups in Kunming Police dogs: Puppy dogs (6 months), Young dogs (18 months), Adult dogs (48 months), Elderly dogs (108 months), and examine their associations with police performance metrics. Using a multi-omics approach combining 16S rRNA sequencing, shotgun metagenomics, metagenome-assembled genomes (MAGs), and Spearman correlation analyses, the authors identified age-related shifts in bacterial species and metabolic pathways, especially those linked to nervous system function. They also reported bacterial taxa positively or negatively correlated with police work performance. This is the first study to investigate the longitudinal changes in the gut microbiome and metabolome of Kunming dogs at different life stages and analyze their associations with police performance.

---

## 🧪Study Design
- Design: Cross-sectional observational study, not case-control. Dogs were sampled at a single time point, stratified into four fixed age groups; no individual animal was followed over time despite the authors describing the design as longitudinal in places.
- Population: 48 dogs total (12 per age group, evenly split by sex: 6 male, 6 female per group)
- Groups compared: Puppies / Young dogs / Adult dogs / Eldery dogs.

## 🗂️ Curation Approach
- The experiments were curated as one-vs-all comparision, where each age group was compared against all other groups combined (e.g., Puppy vs Young/Adult/Elderly), rather than pair wise.
- Although four experiments were expected from these comparisions, ony two were statistically significant, resulting in two curatble experiments from this comparison.
- Eeach police performance indicator was curated separately, resulting in eight (8) additional experiments. This brings the total number of curated experiments to ten (10). 

---

## 🔬Experiments Curated

### ⚗️Experiment 1 - 2
- Comparison: Puppies vs Young/Adult/Elderly dogs; Elderly vs Puppy/Young/Adult (fecal microbiota composition)
- Sample size: 12 per group
- Statistical method: Wilcoxon rank-sum test

### ⚗️Experiment 6 (Spearman correlation)
- Comparison: Positive vs Negative correlation between bacterial species and each police performance indicators (crowd crossing, environmental adptation, led performance, possessive desire, object attention, object holding bite, searching desire, and searching capability)
- Statistical method: Spearman correlation

---

## 🔢Statistical Analyses
- Primary tests used for curation: Wilcoxon rank-sum, Spearman correlation for species–performance associations
- Significance threshold: p < 0.05
- Multiple testing correction: Bonferroni correction for abundance comparisons

---

## 🗂️Data Sources
- Figure S1A and S1B (Experiment 1 - 2)
- Figure 4D (Experiment 3 - 10)

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Beta diversity analyses (PCoA, ANOSIM)
- Functional pathway analyses (KEGG, neurotransmitter metabolism)
- Metabolomic results (neuroactive ligand-receptor interactions)
- Non-significant taxa

---

## 🦠 Differentially Abundant Taxa

### See ➤ :[https://bugsigdb.org/41840712]

---

## ✏️Curation Notes
- Antibiotic exclusion time frame: The paper states "no medications administered prior to the trial" — satisfies antibiotic exclusion criteria. No specific washout window was defined; time frame left blank per policy.
- Policy decisions: Each police performance indicator was curated separately, and the groups contrasted were **positive correlation** versus **negative correlation**.
- Only taxa meeting p < 0.05 were curated  
- Taxa names standardized using NCBI Taxonomy Browser  
- Signatures created following BugSigDB rules (no empty signatures)
- Condition term selection: No BugSigDB controlled vocabulary term maps cleanly to *police dog working performance.* Therefore, **Behaviour** was selected as the most accurate available term, defined as "the set of actions and mannerisms made by systems in response to stimuli or inputs," which directly maps to the scored behavioral traits (olfactory search, obedience, aggression, environmental adaptation) for experiment 3 - 10.

---

## 🗃️Metadata
- Host: Canis lupus familiaris (Kunming dog, Wolf Cyan breed)
- Disease/Condition: Behavior; Age-related variation (healthy dogs)
- Environment: Police dog training base, Kunming, China
- Sequencing platform: Illumina NextSeq 2000 (16S rRNA), Illumina NovaSeq X Plus (metagenomics)

---

## 🧾Curation Summary
- This curation involved navigating several non-standard challenges that extended well beyond routine case–control entry. One of the most important decisions was correctly identifying the study as cross-sectional, despite the authors’ own use of “longitudinal” terminology. Another key step was determining that Fig. S1A and S1B used a one-against-all statistical design, rather than pairwise comparisons. This is because the authors applied a Kruskal–Wallis omnibus test followed by Wilcoxon post-hoc testing, comparing each age group against all other groups combined. As a result, only two comparisons—Puppies vs. all others and Elderly vs. all others—produced statistically significant taxa, yielding two curatable experiments, while the Young and Adult group comparisons were non-significant.

- Splitting Fig. 4D into eight separate per-indicator experiments required direct, cell-by-cell extraction from the heatmap to identify taxa significantly associated with each individual police performance metric. This process also revealed several species present in the figure but not mentioned in the manuscript text, including *Romboutsia ilealis*, *Romboutsia sp. CE17*, *Blautia hansenii* etc, all of which were incorporated in the curation.

- Choosing an appropriate condition term was another challenge. After considering “psychomotor performance,” “cognition,” and other options, the most defensible mapping within the available ontology was **Behavior**, as no existing term adequately captured the composite occupational scoring system used to evaluate Kunming police dog performance.

Overall, this curation contributes a novel non-human working-animal microbiome dataset to BugSigDB, with high-resolution species-level metagenomic signatures linked to a behavioral performance phenotype relevant to the gut–brain axis. The final structure comprises ten curatable experiments—two from 16S rRNA one-against-all age-group comparisons and eight from metagenomic Spearman correlation analyses of individual police performance indicators—making it one of the more complex multi-experiment entries curated to date. This entry highlights age-related microbial shifts in Kunming dogs, identifies species associated with distinct dimensions of police performance, and provides a rich dataset for reproducible enrichment analysis within the broader microbiome research community.
