# Shared Functional Microbiome Signatures in Parkinson's Disease and Constipation-Predominant Irritable Bowel Syndrome Despite Taxonomic Divergence

## Full Citation
 Hoedt E.C., Burns G.L., Hedley K.E., Waller S., Sanchez T.C., Chisolm O., MacCallum H., Richardson S., Suthers B., Pepper E., Keely S., Talley N.J. (2026). *Shared Functional Microbiome Signatures in Parkinson's Disease and Constipation-Predominant Irritable Bowel Syndrome Despite Taxonomic Divergence.* Brain, behavior, & immunity - health, DOI: https://doi.org/10.1016/j.bbih.2026.101218


## BugSigDB Entry
🔗 Curated record: https://bugsigdb.org/41993915

---

## 📘Study Overview
This study investigated the gut microbiome composition, peripheral immune profiles, and gastrointestinal (GI) symptom associations in early-to-mid stage Parkinson's disease (PD) patients, healthy controls, and individuals with constipation-predominant irritable bowel syndrome (IBS-C).

Using shotgun metagenomics and PBMC flow cytometry, the study aimed to determine:
1. Whether circulating gut-homing T cells are altered in PD  compared to healthy controls
2. Which gut microbial species correlate with immune markers and GI symptoms within PD
3. Whether taxonomic or functional microbiome profiles overlap between PD and IBS-C

For BugSigDB curation, only analysable, taxon-level, group-based results were extracted. The only curatable components of this study are the **Spearman correlation analyses** linking microbial species to gastrointestinal (GI) symptoms within PD patients.

---

## 🧪Study Design
- Design: **Case–control**
- Host species: Homo sapiens
- Cases: Individuals diagnosed with Parkinson’s disease
- Groups compared:
  * PD patients vs. healthy controls (microbiome + immune correlations)
  * IBS-C vs. healthy controls and vs. PD (beta diversity and functional pathways only — no taxon-level differential abundance performed for this comparison; therefore not curated)
  * PD patients with vs. without specific GI symptoms - **the only curated experiments (5 within-PD Spearman correlation analyses across 5 GI symptom domains)**

---

## 🔬Curated Experiments

Important structural note:
This study contains no traditional case-vs-control differential abundance.
All curatable results come from within Parkinson’s disease (PD) Spearman correlations between microbial species abundance and Gastrointestinal (GI) symptoms in PD patients. Each GI symptom column in **Figure 3D** (PD panel only) matched with **Supplementary Table 4** constitutes a separate experiment.
Only taxa with **asterisks** (significant after BH-FDR correction) in Table S4 were included.
Direction determined by Rho:
•	Positive Rho → Increased in symptom-positive group **(Group 1)**
•	Negative Rho → Increased in symptom-negative group **(Group 0)**


- **Non-curated sources:**  
  - Figure 3C (species-immune marker correlations was assessed and excluded, it it does not represent a group-contrast differential abundance analysis appropriate for BugSigDB. 
  - No alpha diversity is recorded for any of the five experiments, as no alpha diversity analysis was conducted for symptom-based within-PD comparisons. 
  - IBS-C comparisons (no taxon-level differential abundance performed)  




### ✔️ Experiment 1
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


