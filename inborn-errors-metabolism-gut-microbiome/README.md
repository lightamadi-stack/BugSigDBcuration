# Gut Microbiota in Children with Intoxication-Type Inborn Errors of Metabolism (IEMs)

## Full Citation
 Gokalp S., Dinleyici E.C., Muluk C., Inci A., Aktas E., Okur I., Ezgu F., Tumer L., (2026). *Alterations in gut microbiota composition in children with methylmalonic acidemia, propionic acidemia, and maple syrup urine disease.* European journal of clinical nutrition, DOI: https://doi.org/10.1038/s41430-026-01720-7*

---

## Study Overview
This study examined gut microbiota composition in children diagnosed with intoxication-type inborn errors of metabolism (IEMs), specifically:
- Methylmalonic acidemia (MMA)
- Propionic acidemia (PA)
- Maple syrup urine disease (MSUD)

These were compared with age-matched healthy controls. The study is notable for being the first to characterize gut microbiota in MMA and MSUD patients.

---

## Study Design
- Design: **Case–control**
- Cases: Children with MMA, PA, or MSUD (pooled)
- Controls: Age-matched healthy children  
- Matching variable: **Age**
- Confounders controlled for: **None reported**

The authors labeled the study as “cross-sectional,” but the correct BugSigDB term is **case–control**, because participants were deliberately recruited based on disease status.

---

## Curated Experiments

### Experiment 1
- **Comparison:** IEM patients (MMA + PA + MSUD) vs. healthy controls  
- **Source of curatable results:** Figure 4 (LEfSe bar plot)

No disease-specific subgroup analyses were performed; therefore only one experiment was curatable.

---

## Statistical Analyses
- **LEfSe** (only curatable statistical test)
- DESeq2 mentioned in methods but **excluded** because no significant taxon-level results were published
- Significance level: **α = 0.05**

---

## Data Sources
- **Included:**  
  - Figure 4 (LEfSe biomarkers)

- **Excluded (non-curatable):**  
  - Figures 1–3 (alpha diversity boxplots, relative abundance bar charts)  
  - No tables or supplementary files with per-taxon statistics  

These figures did not report p-values or statistical tests for specific taxa.

---

## Alpha Diversity
Curated as **part of the experiment**, not a separate experiment.

- **Chao1:** decreased in IEM patients (p = 0.041)  
- **Observed OTUs:** decreased in IEM patients (p = 0.047)  
- **Shannon index:** unchanged (p = 0.184)

---

## Differentially Abundant Taxa

### Signature 1 — Increased in IEM Patients  
(18 taxa from LEfSe; *Acinetobacter lwoffii*, *Alcaligenaceae*, *Betaproteobacteria*, *Burkholderiales*, *Castellaniella*, *Castellaniella defragrans*, *Enterobacterales*, *Enterobacteriaceae*, *Lactobacillus iners*, *Providencia*, *Providencia stuartii*, *Pseudoalteromonas piscicida*, *Sphingobacteriaceae*, *Sphingobacteriales*, *Sphingobacteriia*, *Streptococcus anginosus*, *Thomasclavelia saccharogumia*, *[Clostridium] piliforme*)

### Signature 2 — Decreased in IEM Patients  
(7 taxa from LEfSe; *Coprobacillus*, *Coprobacillus cateniformis*, *Faecalibacterium*, *Faecalibacterium prausnitzii*, *Hungatella hathewayi*, *Thomasclavelia spiroformis*, *Erysipelotrichaceae Clostridium*)

*Note:* These signatures include multiple ranks (species, genus, family, order, class).

---

## Taxonomy Notes
- Updated legacy phylum names using current NCBI terminology:  
  - **Pseudomonadota**  
  - **Bacillota**  
  - **Bacteroidota**
- Corrected deprecated species name:  
  - *Clostridium hathewayi* → **Hungatella hathewayi**
- Preserved one unresolvable GreenGenes label:  
  - **g_Erysipelotrichaceae_Clostridium**  
  Following BugSigDB policy, it was entered exactly as reported since no NCBI match exists.

---

## Curation Notes
- Determined correct study design despite author mislabeling.  
- Identified only one valid curatable experiment.  
- Carefully applied LEfSe-only rules.  
- Excluded non-statistical or purely descriptive figures.  
- Ensured taxonomy correctness and handled legacy database artifacts.  
- Followed BugSigDB policies for signature creation, including preserving invalid but reported taxa.

---

## Metadata
- **Host:** Human (children)  
- **Condition:** Intoxication-type inborn errors of metabolism (MMA, PA, MSUD)  
- **Control group:** Age-matched healthy children  
- **Environment:** Clinical pediatric cohort  
- **Sequencing:** 16S rRNA sequencing  

---

## Curation Summary
This curation strengthened my ability to:
- Apply BugSigDB study design criteria independently of author terminology  
- Distinguish curatable from non-curatable figures  
- Apply LEfSe-specific curation rules  
- Handle taxonomy inconsistencies from legacy databases  
- Ensure accuracy in reporting statistical significance and taxonomy  

This contribution fills an important gap by documenting microbial signatures in rare pediatric metabolic disorders.

