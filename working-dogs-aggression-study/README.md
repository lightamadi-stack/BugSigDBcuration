# Gut Microbiota and Aggressive Behavior in Working Dogs

## Full Citation
Sun N, Xie L, Chao J, Xiu F, Zhai H, Zhou Y, Yu X, Shui Y. (2025). *Study on the correlation between aggressive behavior and gut microbiota and serum serotonin (5-HT) in working dogs*. Veterinary Sciences. 12, 526 DOI: https://doi.org/10.3390/vetsci12060526

## BugSigDB Entry
🔗 Curated record: https://bugsigdb.org/40559763

---

## Study Overview
This study investigated the relationship between aggressive behavior, gut microbiota composition, and serum serotonin (5-HT) levels in working dogs. A total of 56 dogs from police K-9 units were classified into behavioral groups (aggressive vs. non-aggressive; offensive vs. defensive aggression) based on questionnaire-derived phenotypes.

---

## Study Design
- Design: Cross-sectional observational study  
- Population: Working dogs (n = 56)  
- Classification: Post-enrollment behavioral grouping using C-BARQ-based assessment  
- No intervention or follow-up  

---

## Experiments Curated

### Experiment 1
- Comparison: Aggressive Dogs vs Non-Aggressive Dogs  
- Sample size: n = 56  

### Experiment 2
- Comparison: Offensive Aggression Dogs vs Defensive Aggression Dogs  
- Sample size: n = 35  

---

## Statistical Analyses
- Welch’s t-test  
- Random Forest (Mean Decrease in Accuracy - MDA)  
- Significance threshold: p < 0.05 (study-wide, pre-specified)  
- No multiple hypothesis testing (MHT) correction applied  
- No LDA scores reported  

---

## Data Sources
- Figure 4b (phylum level, Experiment 1)  
- Figure 5b (genus level, Experiment 1)  
- Figure 8b (genus level, Experiment 2)  
- Figure 8c (Random Forest, supporting Experiment 2)  

---

## Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Shenyang subset analysis (no significant taxa)  
- Shanghai subset (beta diversity only)  
- All beta diversity analyses (PCA/PCoA)  
- Alpha diversity analyses (recorded as metadata only)  
- Serum 5-HT ELISA results (non-microbial)  

---

## Differentially Abundant Taxa

### Experiment 1

#### Increased Abundance in Aggressive Dogs
- *Pseudomonadota* (phylum)

#### Decreased Abundanced in Aggressive Dogs
- *Escherichia-Shigella*  
- *Erysipelotrichaceae UCG-003*  
- *Clostridium sensu stricto 1*  

---

### Experiment 2

#### Increased Abundance in Offensive Aggression Dogs
- *Turicibacter*  

#### Decreased Abundance in Offensive Aggression Dogs
- None (no significant taxa identified; no signature created)

---

## Alpha Diversity
- No significant differences observed across groups  
- Metrics assessed:
  - Chao1  
  - Shannon  
  - Simpson  
  - ACE  
- Source: Table 4 (page 9)  

---

## Confounders Considered
Controlled analytically through PCA and subgroup analyses:
- Breed  
- Sex  
- Geographic location  
- Diet  
- Age  

---

## Curation Notes
- Study design classified as cross-sectional based on sampling strategy and absence of pre-defined case/control recruitment.  
- Matching reported in the paper applies only to a non-curatable subset and was excluded.  
- Random Forest results were carefully evaluated:
  - *Lactobacillus* excluded due to non-significant p-value (p = 0.977)  
  - *Turicibacter* included due to independent statistical support (p < 0.01)  
- Only taxa meeting p < 0.05 were curated  
- Taxa names standardized using NCBI Taxonomy Browser  
- Signatures created following BugSigDB rules (no empty signatures)  

---

## Metadata
- Host: Dog (Canis lupus familiaris)  
- Condition: Aggressive behavior  
- Sequencing: 16S rRNA (Illumina MiSeq)  
- Environment: Veterinary / working dog cohort  

---

## Curation Summary
This curation involved critical evaluation of study design, statistical methodologies, and microbiome data interpretation. It required distinguishing between machine learning outputs and statistically validated results, correctly identifying curatable experiments, and applying BugSigDB policies in a veterinary context. The process strengthened my ability to standardize microbial signatures and interpret complex microbiome datasets beyond human studies.

