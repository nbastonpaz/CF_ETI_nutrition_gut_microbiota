# CF_ETI_nutrition_gut_microbiota

**Paper:** “Beyond Weight Gain: Dietary Intake, Body Composition, and the Gut Microbiome After One Year of Elexacaftor-Tezacaftor-Ivacaftor in Children and Adolescents with Cystic Fibrosis”

## Overview

This repository contains the code and data used to reproduce the analyses of nutritional status and gut microbiome changes in children and adolescents with cystic fibrosis (CF) after one year of treatment with elexacaftor–tezacaftor–ivacaftor (ETI).

The study integrates dietary intake, anthropometry, body composition, pancreatic function and fat absorption markers, serum lipid profiles, shotgun metagenomics, fecal metaproteomics, and targeted metabolomics of short-chain fatty acids (SCFAs). The analyses were designed to explore what lies beyond changes in BMI-for-age z-score after ETI and whether individual BMI responses were associated with changes in dietary intake, body composition, fat absorption, serum lipids, or the gut microbiome.

## Cohort & sampling

This prospective longitudinal study includes **9 clinically stable children and adolescents with CF**, aged 7–17 years, with complete paired 3-day dietary records and bioimpedance measurements at baseline (T0) and after 12 months of ETI treatment (T12).

The subgroup included both participants who were CFTR modulator-naïve and participants previously treated with other CFTR modulators before ETI initiation.

Fecal samples were collected from each participant at both study time points:

* **T0:** before starting ETI
* **T12:** after 12 months of ETI treatment

**Total number of fecal samples = 18**

* T0 = 9
* T12 = 9

For outcomes with incomplete paired data availability, analyses were restricted to the corresponding paired subgroups:

* Sweat test measures: **n = 8**
* Pancreatic enzyme replacement therapy (PERT), expressed as lipase units: **n = 8**
* Fat absorption markers [fecal fat and coefficient of fat absorption (CFA)]: **n = 6**
* Total cholesterol and triglycerides: **n = 8**
* HDL and LDL cholesterol: **n = 7**

All longitudinal analyses were performed using paired comparisons, with each participant serving as their own reference.

## Contents of the repository

In this repository you will find the data, metadata, and R scripts used for the following analyses:

1. **Clinical and anthropometric analysis**

   * Lung function
   * Sweat chloride
   * Fecal calprotectin
   * Fecal elastase
   * Pancreatic enzyme replacement therapy (PERT)
   * BMI-for-age z-score
   * Weight-for-age z-score
   * Height-for-age z-score

2. **Dietary intake analysis**

   * Total energy intake
   * Macronutrient intake
   * Macronutrient density
   * Fiber intake
   * Longitudinal changes from T0 to T12

3. **Body composition analysis**

   * Fat mass (%)
   * Fat mass index (FMI)
   * Lean mass (%)
   * Total body water (TBW)

4. **Fat absorption analysis**

   * Fecal fat
   * Coefficient of fat absorption (CFA)
   * Associations between changes in absorption markers and BMI-for-age z-score

5. **Serum lipid profile**

   * Total cholesterol
   * LDL cholesterol
   * HDL cholesterol
   * Non-HDL cholesterol
   * Triglycerides
   * LDL/HDL ratio

6. **Gut microbiome compositional analysis**

   * Shotgun metagenomics
   * Taxonomic profiling
   * Alpha diversity
   * Beta diversity
   * Differential abundance analysis

7. **Gut microbiome functional analysis**

   * Fecal metaproteomics

8. **Targeted metabolomics**

   * Short-chain fatty acids (SCFAs)

9. **Associations with BMI-for-age z-score**

   * Dietary intake
   * Body composition
   * Fat absorption markers
   * Serum lipid profile
   * Fecal microbial taxa
     

## Sequencing and proteomics data

Shotgun metagenomic sequencing data are publicly available in the **European Nucleotide Archive (ENA)**: PRJEB103799

Proteomics data are publicly available through **ProteomeXchange/PRIDE**: PXD070696


## Statistical approach

Longitudinal analyses were based on paired T0–T12 measurements. Depending on the analysis, the repository includes:

* Paired statistical comparisons between T0 and T12
* False discovery rate (FDR) correction for multiple testing
* Spearman correlation analyses using within-participant changes (ΔT12–T0)
* Linear mixed-effects models for longitudinal microbiome association analyses

The sample size varies across some analyses because not all clinical and biochemical measurements were available for every participant.

## Limitations

The main limitation of this study is the small pediatric sample size, which reduces statistical power and means that association analyses should be considered exploratory. Some outcomes, particularly fat absorption and serum lipid markers, were available only in smaller paired subsets.

Dietary intake was estimated from 3-day dietary records and may not fully represent habitual intake. Body composition was estimated using bioimpedance, which provides an indirect measure and may be influenced by hydration status.

The cohort was clinically stable at baseline, which may have limited the magnitude of detectable clinical and microbiome changes. In addition, microbiome and functional analyses were based on two time points, baseline and 12 months, and therefore transient changes occurring during the first months after ETI initiation may not have been detected.

Finally, the differentially abundant taxa identified in the longitudinal microbiome analysis were uncommon and present at low relative abundance. These findings should therefore be interpreted cautiously, particularly given the limited sample size.

## License

This repository is distributed under the **GNU General Public License v3.0 (GPL-3.0)**.

## Contact

For any issues or questions, please contact: **[natalia.baston.paz@gmail.com](mailto:natalia.baston.paz@gmail.com)**.
