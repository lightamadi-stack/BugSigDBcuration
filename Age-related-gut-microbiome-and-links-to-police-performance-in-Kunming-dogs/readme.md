# Age Related Gut Microbiome and Links to Police Performance in Kunming Dogs

## Full Citation
Xu L., Liu C., Chen S., Mao A., Zi X., Li J., Ge X., Liu Q., Wang S., Li X., Wu Q., Wan J., Zhang Z., Xu H., Li J., Lin Q., Cao Z. (2026). *Characterization of age-related changes in the gut microbiome and metabolome of Kunming dogs and their associations with police performance*. Microbiome. 14:121 DOI: https://doi.org/10.1186/s40168-026-02388-8

## BugSigDB Entry
🔗 Curated record: https://bugsigdb.org/41840712

---

## Study Overview
This study investigated how gut microbiome composition and functional pathways vary across age groups in Kunming dogs (Puppy, Young, Adult, Elderly), and how bacterial species correlate with police performance scores. Using a multi-omics approach combining 16S rRNA sequencing, shotgun metagenomics, metagenome-assembled genomes (MAGs), and Spearman correlation analyses, the authors identified age-related shifts in bacterial species and metabolic pathways, especially those linked to nervous system function. They also reported bacterial taxa positively or negatively correlated with police work performance. This is the first study to investigate the longitudinal changes in the gut microbiome and metabolome of Kunming dogs at different life stages and analyze their associations with police performance.

---

## Study Design
- Design: Cross-sectional observational study, not case-control 
- Population: 48 dogs total (12 per age group, evenly split by sex: 6 male, 6 female per group) 

---

## Experiments Curated

### Experiment 1 - 5
- Comparison: Puppies vs Young; Puppies vs Adult; Puppies vs Elderly dogs; Young vs Adult; Young vs Elderly (fecal microbiota composition)
- Sample size: 12 per group
- Statistical method: Wilcoxon rank-sum test

### Experiment 6 (Spearman correlation)
- Comparison: Positive vs Negative correlation between bacterial species and police performance indicators
- Statistical method: Spearman correlation

---

## Statistical Analyses
- Primary tests used for curation: Wilcoxon rank-sum, Spearman correlation for species–performance associations
- Significance threshold: p < 0.05
- Multiple testing correction: Bonferroni correction for abundance comparisons

---

## Data Sources
- Figure S1A and S1B (Experiment 1 - 5)
- Figure 4D (Experiment 6)

---

## Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Beta diversity analyses (PCoA, ANOSIM)
- Functional pathway analyses (KEGG, neurotransmitter metabolism)
- Metabolomic results (neuroactive ligand-receptor interactions)
- Non-significant taxa

---

## 🦠 Differentially Abundant Taxa

### See ➤ :[https://bugsigdb.org/41840712]

---

## Curation Notes
- Antibiotic exclusion time frame: The paper states "no medications administered prior to the trial" — satisfies antibiotic exclusion criteria. No specific washout window was defined; time frame left blank per policy.
- Policy decisions: Combined all performance indicators into one experiment (Experiment 6) to avoid redundant entries.
- Only taxa meeting p < 0.05 were curated  
- Taxa names standardized using NCBI Taxonomy Browser  
- Signatures created following BugSigDB rules (no empty signatures)  

---

## Metadata
- Host: Canis lupus familiaris (Kunming dog, Wolf Cyan breed)
- Disease/Condition: Behavior; Age-related variation (healthy dogs)
- Environment: Police dog training base, Kunming, China
- Sequencing platform: Illumina NextSeq 2000 (16S rRNA), Illumina NovaSeq X Plus (metagenomics)

---

## Curation Summary
This curation involved navigating several non-standard challenges that extended well beyond routine case-control entry. The most significant decisions were the correct identification of the cross-sectional design despite the authors' own "longitudinal" framing, the inversion correction of Group 0 and Group 1 assignments, and the policy-justified decision to curate Fig. 4D as a single experiment rather than fragmenting it into eight per-indicator entries. The consistent directional pattern of species across all performance indicators was the key biological observation that justified this approach, and it was confirmed through direct heatmap inspection rather than relying solely on the paper's narrative text.

Overall, this curation contributes a novel non-human working animal microbiome dataset to BugSigDB, with rich species-level metagenomic signatures linked to a behavioural phenotype via a gut-brain axis framework. It helped organize the study’s taxonomic, functional, and correlation-based microbiome findings into a standardized structure suitable for reproducible analysis. It highlights age-related microbial shifts in Kunming dogs and identifies species linked to police performance, offering insights into the gut–brain axis in working animals.



