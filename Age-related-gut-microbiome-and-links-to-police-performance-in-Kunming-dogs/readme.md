# Age Related Gut Microbiome and Links to Police Performance in Kunming Dogs

## Full Citation
Xu L., Liu C., Chen S., Mao A., Zi X., Li J., Ge X., Liu Q., Wang S., Li X., Wu Q., Wan J., Zhang Z., Xu H., Li J., Lin Q., Cao Z. (2026). *Characterization of age-related changes in the gut microbiome and metabolome of Kunming dogs and their associations with police performance*. Microbiome. 14:121 DOI: https://doi.org/10.1186/s40168-026-02388-8

## BugSigDB Entry
🔗 Curated record: https://bugsigdb.org/41840712

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
- Condition term selection: No BugSigDB controlled vocabulary term maps cleanly to *police dog working performance.* Therefore, **Behaviour** (SIO:001195) was selected as the most accurate available term, defined as "the set of actions and mannerisms made by systems in response to stimuli or inputs," which directly maps to the scored behavioral traits (olfactory search, obedience, aggression, environmental adaptation) for experiment 3 - 10.

---

## 🗃️Metadata
- Host: Canis lupus familiaris (Kunming dog, Wolf Cyan breed)
- Disease/Condition: Behavior; Age-related variation (healthy dogs)
- Environment: Police dog training base, Kunming, China
- Sequencing platform: Illumina NextSeq 2000 (16S rRNA), Illumina NovaSeq X Plus (metagenomics)

---

## 🧾Curation Summary
This curation involved navigating several non-standard challenges that extended well beyond routine case-control entry. The most significant decisions were the correct identification of the cross-sectional design despite the authors' own "longitudinal" framing, the inversion correction of Group 0 and Group 1 assignments, and the policy-justified decision to curate Fig. 4D as a single experiment rather than fragmenting it into eight per-indicator entries. The consistent directional pattern of species across all performance indicators was the key biological observation that justified this approach, and it was confirmed through direct heatmap inspection rather than relying solely on the paper's narrative text.

Overall, this curation contributes a novel non-human working animal microbiome dataset to BugSigDB, with rich species-level metagenomic signatures linked to a behavioural phenotype via a gut-brain axis framework. It helped organize the study’s taxonomic, functional, and correlation-based microbiome findings into a standardized structure suitable for reproducible analysis. It highlights age-related microbial shifts in Kunming dogs and identifies species linked to police performance, offering insights into the gut–brain axis in working animals.



