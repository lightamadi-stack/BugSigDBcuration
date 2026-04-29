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
- Body site:	Feces
- Groups compared:
  * PD patients vs. healthy controls (microbiome + immune correlations)
  * IBS-C vs. healthy controls and vs. PD (beta diversity and functional pathways only — no taxon-level differential abundance performed for this comparison; therefore not curated)
  * PD patients with vs. without specific GI symptoms - **the only curated experiments (5 within-PD Spearman correlation analyses across 5 GI symptom domains)**

---

## 🔬Curated Experiments
*Important structural note*: This study contains no traditional case-vs-control differential abundance. All curatable results come from within Parkinson’s disease (PD) Spearman correlations between microbial species abundance and Gastrointestinal (GI) symptoms in PD patients. Each GI symptom column in **Figure 3D** (PD panel only) matched with **Supplementary Table 4** constitutes a separate experiment.
- Only taxa with **asterisks** (significant after BH-FDR correction) in Table S4 were included.
- Direction determined by Rho:
  - Positive Rho → Increased in symptom-positive group **(Group 1)**
  - Negative Rho → Increased in symptom-negative group **(Group 0)**

**🚫Non-curated sources:**
- Figure 3C (species-immune marker correlations was assessed and excluded, it it does not represent a group-contrast differential abundance analysis appropriate for BugSigDB.
- No alpha diversity is recorded for any of the five experiments, as no alpha diversity analysis was conducted for symptom-based within-PD comparisons.
- Beta diversity was recorded but excluded
- IBS-C comparisons (no taxon-level differential abundance performed)
- Non-asterisk taxa | Not significant after BH correction
- MetaCyc pathway results (Figure 4D)

---

### ✔️ Experiment 1: Difficulty Swallowing
Group 1: Parkinson's disease (PD) patients **with difficulty swallowing**
Group 0: Parkinson's disease (PD) patients **without difficulty swallowing**

#### 🦠Signature 1 — Increased in Group 1
- *Mediterraneibacter gnavus*	
#### 🦠Signature 2 — Decreased in Group 1
- No significant taxa decreased in Group 1.

### ✔️ Experiment 2: Vomiting or Nausea
Group 1: Parkinson's disease (PD) patients **with vomiting or nausea**
Group 0: Parkinson's disease (PD) patients **without vomiting or nausea**

#### 🦠Signature 1 — Increased in Group 1
- *Veillonella atypica*
- *Allisonella histaminiformans*
- *Alistipes sp. An31A* etc
#### 🦠Signature 2 — Decreased in Group 1
- *Intestinimonas massiliensis*
- *Alistipes finegoldii* etc

### ✔️ Experiment 3: Constipation (Last Month)
Group 1: Parkinson's disease (PD) patients **with constipation within the last month**
Group 0: Parkinson's disease (PD) patients **without constipation within the last month**

#### 🦠Signature 1 — Increased in Group 1
- *GGB9788_SGB15411* (Unamed taxon)
- *GGB9637_SGB15111* (Unamed taxon)
#### 🦠Signature 2 — Decreased in Group 1
- *GGB9818_SGB15459* (Unamed taxon)

### ✔️ Experiment 4: Incomplete Bowel Emptying
Group 1: Parkinson's disease (PD) patients **with incomplete bowel emptying**
Group 0: Parkinson's disease (PD) patients **without incomplete bowel emptying**

#### 🦠Signature 1 — Increased in Group 1
- *Intestinimonas massiliensis*
- *Alistipes finegoldii*
#### 🦠Signature 2 — Decreased in Group 1
(Extensive list) includes:
- *Allisonella histaminiformans*
- *Phocaeicola coprophilus*
- *Odoribacter laneus* etc

### ✔️ Experiment 5: Bowel Pattern (Last 12 Months)
Group 1: Negative correlation in Parkinson's disease (PD) patients with **constipated or alternating bowel pattern** in the last 12 months
Group 0: Positive correlation in Parkinson's disease (PD) patients with **normal bowel pattern** in the last 12 months

#### 🦠Signature 1 — Increased in Group 1
- *Pseudoflavonifractor gallinarum*
- *GGB9788_SGB15411* (Unnamed taxon)
#### 🦠Signature 2 — Decreased in Group 1
No significant taxa decreased in Group 1

---

## 📊Statistical Analyses
- **Spearman Correlation** + **Benjamini–Hochberg False Discovery Rate** correction (BH-FDR) for species-symptom and species-immune analyses etc
- Data transformation: Total Sum Scaling followed by **Centered Log-Ratio transformation**
- Significance level: **α = 0.05**

---

## 📝 Curation Notes
- Study type classified as case–control, but curated experiments are within-PD symptom correlations.
- Each GI symptom column in Figure 3D = one experiment.
- Asterisk system used as authoritative significance marker due to errors in Supplementary Table S4 p-values.
- Antibiotic exclusion confirmed (3 months prior).
- Unnamed SGBs treated according to BugSigDB unresolved-taxon policy. 

---


## 🧾 Summary
This study required non-standard BugSigDB curation due to its absence of case–control taxon-level differential abundance. Instead, all curatable results were species–GI symptom correlations within PD, producing five valid experiments.
Key takeaways:
1. Correct identification of non-standard experimental structures
2. Use of symptom columns as independent experiments
3. Accurate handling of unnamed SGBs
4. Detecting supplementary p-value alignment errors
5. Applying Rho direction rules consistently 
Hence, this curation adds five unique microbiome–symptom signatures in Parkinson’s disease — a context currently underrepresented in BugSigDB.




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


