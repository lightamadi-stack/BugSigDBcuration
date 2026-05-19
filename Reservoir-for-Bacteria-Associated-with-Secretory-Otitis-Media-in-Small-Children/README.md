# The Adenoids but Not the Palatine Tonsils Serve as a Reservoir for Bacteria Associated with Secretory Otitis Media in Small Children

## Full Citation
Fagö-Olsen H., Dines L.M., Sørensen C.H., Jensen A. (2019). *The Adenoids but Not the Palatine Tonsils Serve as a Reservoir for Bacteria Associated with Secretory Otitis Media in Small Children*. mSystems Volume 4 Issue 1 e00169-18.  DOI: https://doi.org/10.1128/mSystems.00169-18

## BugSigDB Entry
🔗 Curated record: [Click here](https://bugsigdb.org/30801022)

---

## 📘Study Overview
This study investigated the combined role of the palatine tonsils and adenoids as reservoirs for potential pathogens associated with secretory otitis media (SOM) in small children aged 1–5 years. Using 16S rRNA gene pyrosequencing, the authors characterized and compared the crypt microbiomes of both anatomical sites in two clinical groups: children with adenoid/tonsil hyperplasia without prior infection (HP group) and children with SOM. The study demonstrated that the adenoids, but not the palatine tonsils, serve as the primary reservoir for the classical otitis media pathogens Streptococcus pneumoniae, Haemophilus influenzae, and Moraxella catarrhalis.

---

## 🧪Study Design
- Design type: Case-control (Experiments 1, 2, and 3).
- Host species: Homo sapiens
- Sample size: 28 children total (14 HP group, 14 SOM group); 56 samples analyzed (28 adenoid + 28 tonsil)
- Groups compared:
    - HP group (hyperplasia, no AOM/SOM in prior year) vs. SOM group (secretory otitis media)
    - Adenoids vs. palatine tonsils (pooled across both clinical groups)

---

## 🔬Experiments Curated

### ⚗️Experiment 1
- Comparison: HP group (control) vs. SOM group (case), adenoid samples
- Body site: Nasopharynx (adenoids)
- Sample size: 14 vs 14
- Statistical method: LEfSe
- Source figures/tables: Figure 7B

### 🦠 Differentially Abundant Taxa
- Increased in SOM, adenoids (Case)
      - *Neisseria flavescens*, *Haemophilus parainfluenzae*, *Granulicatella adiacens* etc. 
- Increased in HP adenoids (Control)
      - *Streptococcus pneumoniae*, *Porphyromonas pasteri*, *Fusobacterium periodonticum* etc

### ⚗️Experiment 2
- Comparison: HP group (control) vs. SOM group (case), palatine tonsil samples
- Body site: Palatine tonsil
- Sample size: 14 vs 14
- Statistical method: LEfSe
- Source figures/tables: Figure 7A 

### 🦠 Differentially Abundant Taxa
- Increased in SOM tonsils (Case)
      - *Prevotella nanceiensis*, *Prevotella salivae*, *Neisseria meningitidis/cinerea* etc
- Increased in HP tonsils (control)
      - *Neisseria flavescens*, *Fusobacterium periodonticum*, *Haemophilus parainfluenzae* etc.

### ⚗️Experiment 3
- Comparison: Palatine tonsils (Group 0) vs. adenoids (Group 1), collapsed across HP and SOM groups
- Body site: Palatine tonsil (Group 0) vs. nasopharynx/adenoids (Group 1)
- Statistical method: LEfSe
- Source figures/tables: Figure 7C 

### 🦠 Differentially Abundant Taxa
- Increased in Adenoids (Case)
      - *Streptococcus pneumoniae*, *Moraxella catarrhalis*, *Haemophilus influenzae* etc.
- Increased in Tonsils (control)
      - *Flavobacteriaceae*, *Capnocytophaga leadbetteri*, *Fusobacterium periodonticum* etc.

---

## 🔢Statistical Analyses
- Primary tests used for curation:
      - LEfSe (Linear Discriminant Analysis Effect Size) for differential abundance
- Significance threshold:
    - p < 0.05
    - LDA > 3.5 for LEfSe
- Multiple testing correction: None

---

## 🗂️Data Sources
- Figure 7A, 7B, and Figure 7C

---

## 🚫Excluded Analyses
The following were excluded based on BugSigDB curation rules:
- Beta diversity
- Fig S2 (correlation analysis): Not curatable — reports within-subject correlation between anatomical sites, not between-group differential abundance.
- Fig 2 (Venn diagram), Fig 3 (phylogenetic tree), Fig 4 (OTU box plots), Fig 5 (phylum/genus bar plots): Descriptive only; no formal taxon-level significance testing.
- Table S1–S5: Descriptive data tables or culture results; no taxon-level differential abundance statistics.
- Fig 8: Supporting visualization of the adenoids vs. tonsils pattern for three species (S. pneumoniae, H. influenzae, M. catarrhalis); results already captured via Fig 7C.

---

## ✏️Curation Notes
- Figure 7 panel labelling discrepancy: A discrepancy exists between the Results text and Figure 7 regarding panels A and B. The Results text describes Fig 7A as the tonsil comparison and Fig 7B as the adenoid comparison, but the taxa attributed to each panel in the text do not match the panel contents, S. pneumoniae, F. nucleatum subsp. vincentii, and Eikenella corrodens are described as adenoid taxa yet appear in the panel labelled 7A, while Actinobacteria is described as a tonsil taxon yet appears in the panel labelled 7B. The figure caption has been followed as the authoritative source, as it explicitly assigns *(A) tonsils, (B) adenoids.* Taxon directionality has been read directly from the figure bars. Reviewers should verify signatures against the figure panels directly.
- Alpha diversity directionality: Alpha diversity is reported relative to Group 1 (case/exposed group) per BugSigDB convention. For Experiment 2, HP adenoids have lower diversity than SOM adenoids, meaning alpha diversity is increased in Group 1 (SOM adenoids).
- Multiple unclassified Haemophilus OTUs in Fig 7A: Multiple unclassified Haemophilus OTUs appeared on both sides of the LEfSe plot. Since these cannot be distinguished at genus level in NCBI taxonomy, Haemophilus was entered once in the decreased signature only (decreased in Group 1, SOM tonsils), based on the higher LDA score of the OTU on that side.
- Multiple unclassified Streptococcus OTUs: Three unclassified Streptococcus OTUs appeared in Fig 7A. Since none could be resolved to species level, Streptococcus was entered once at genus level per signature direction.

---

## 🗃️Metadata
- Host: Homo sapiens (small children)
- Disease/Condition: Otitis media with effusion
- Body site: Upper respiratory tract (palatine tonsil crypts; nasopharyngeal adenoid crypts)
- Sequencing platform: 454 pyrosequencing (Roche454)
- Antibiotic exclusion: Yes — participants excluded if antibiotics used within 1 month prior to surgery

---

## 🧾Curation Summary
This curation involved a structurally complex study with two body sites, two clinical groups, and three distinct curatable experiments. Key learning points included: navigating a 2×2 multi-group design and decomposing it into pairwise comparisons per BugSigDB policy; handling a published figure panel labelling error and applying the figure caption as the authoritative source over the Results text; resolving ambiguous taxon entries where multiple unclassified OTUs of the same genus appeared on both sides of a LEfSe plot; correctly assigning alpha diversity directionality relative to Group 1; and distinguishing between rarefaction as a normalization step versus data transformation for BugSigDB entry. 

This study contributes three experiments to BugSigDB documenting microbial signatures in the upper respiratory tract of young children in the context of secretory otitis media and adenoid hyperplasia.
