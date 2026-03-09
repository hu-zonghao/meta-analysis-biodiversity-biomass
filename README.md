
---

# Meta-Analysis Full Code - Readme

This repository contains the complete R code for all meta-analyses conducted in a research paper, integrated within a single R Markdown (`.Rmd`) file. The code is organized with sections and comments detailing each analytical step, corresponding figure numbers, and data processing specifics. Running this Rmd file reproduces all figures and statistical results presented in the paper.

## Project Overview
This project automates the full meta-analysis for the paper using R Markdown, covering core analyses including global mapping, cumulative forest plots, subgroup forest plots, interaction analysis, factor analysis, biodiversity–biomass relationships, aboveground–belowground relationships, and publication bias tests. The code is clearly structured and thoroughly commented to facilitate result verification by reviewers and readers.

## File Description
- `manuscript_analysis.Rmd`: The main R Markdown file containing all R code.
- `README.md`: This documentation file.

## Rmd Internal Structure
The Rmd file is divided into sections following the paper's analytical flow, each corresponding to a set of figures and analyses. Section titles and corresponding figure numbers are as follows (see comments within the Rmd for details):

### 1. Global Map
- `# Global map for Fig. S2`: Generates the global sampling site distribution map for Supplementary Figure S2.

### 2. Cumulative Effect Size Forest Plots
- `# Fig.1 and Fig.S3`: Generates cumulative effect size forest plots for Main Figure 1 and Supplementary Figure S3.
- `# Cumulative effect size subgroup forest plots for Figs. S3–S8`: Generates cumulative effect size subgroup forest plots for Supplementary Figures S3 to S8.

### 3. Subgroup Forest Plots
- `# Forest plot by category`: Categorical forest plot.
- `## Stratified by biomes`: Subgroup forest plot stratified by biomes.

### 4. Interaction Analysis
- `# Interaction for Fig. 4ab and Figs. S15–S17`: Generates interaction analysis results for Figure 4a–b and Supplementary Figures S15–17.
- `## Interaction calculation`: Interaction calculations.
  - `### Calculation of plant richness–biomass interaction`: Calculation of plant richness–biomass interaction.
- `## Interaction plots`: Plotting interactions.
  - `### Number of plant interaction study cases`: Plot showing the number of plant interaction study cases.

### 5. Factor Analysis
- `# Factor analysis interpretation for Figs. 4cd and S18`: Generates factor analysis interpretation figures for Figure 4c–d and Supplementary Figure S18.
- `## Data preprocessing`: Data preprocessing steps.
  - `### Treatment intensity`: Processing related to treatment intensity.
- `## Factor analysis interpretation`: Factor analysis interpretation.
- `## Factor analysis plots`: Plotting factor analysis results.
  - `### Plant`: Factor plots related to plants.

### 6. Biodiversity–Biomass Relationship
- `# Biodiversity–biomass relationship for Fig. 2 and Figs. S9–S12`: Generates biodiversity–biomass relationship figures for Figure 2 and Supplementary Figures S9–12.
- `## Overall biodiversity–biomass relationship`: Overall biodiversity–biomass relationship.
  - `### Plant biodiversity–biomass relationship`: Plant biodiversity–biomass relationship.
  - `### Plant biodiversity–biomass relationship by intensity and duration`: Plant biodiversity–biomass relationship stratified by treatment intensity and duration.
- `## Biodiversity–biomass relationship by factor`: Biodiversity–biomass relationship stratified by factor.
  - `### Plant biodiversity–biomass relationship by factor`: Plant biodiversity–biomass relationship stratified by factor.

### 7. Aboveground–Belowground Relationships
- `# Aboveground–belowground relationships`: Overview of aboveground–belowground relationships.
- `## Aboveground–belowground coupling`: Aboveground–belowground coupling relationships.
  - `### Plant biomass–microbial biomass`: Relationship between plant biomass and microbial biomass.
- `## Aboveground–belowground relationships under NPK treatment`: Aboveground–belowground relationships under NPK treatment.
  - `### Plant biomass and microbial biomass under NPK treatment`: Plant biomass and microbial biomass under NPK treatment.
- `## Aboveground–belowground relationships by individual and combined factors`: Aboveground–belowground relationships analyzed by individual and combined factors.
  - `### Plant biomass and microbial biomass`: Corresponding plant and microbial biomass data.

### 8. Publication Bias
- `# Publication bias`: Publication bias tests.
- `## Stratified by biomes`: Publication bias analysis stratified by biomes.
  - `### Plant`: Publication bias for plant-related studies.
- `## By taxon`: Publication bias analysis stratified by taxonomic group.
  - `### Microbes`: Publication bias for microbe-related studies.

## Environment and Dependencies
- **Software**: R (≥ 4.4.1)
- **R Packages**:
  - `meta` / `metafor`: For meta-analysis
  - `ggplot2`: For plotting
  - `dplyr` / `tidyr`: For data manipulation
  - `cowplot` / `patchwork`: For combining plots
  - `rnaturalearth` / `sf`: For global map generation
  - `knitr` / `rmarkdown`: For running the Rmd file

---
