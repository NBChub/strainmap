# strainmap
Map of the G1034 NPGM actinomycete strains published in [NAR](https://doi.org/10.1093/nar/gkae523).

Open [notebook here](https://github.com/NBChub/strainmap/blob/main/notebook/strainmap_G1034.ipynb).

## Overview
This repository contains data, analysis notebooks, and results for mapping NPGM isolates/strains. It includes processed data, figures generated from the analysis, and the Jupyter notebook used for the analysis.

*Important Note*: Two genomes are dropped because of inconsistent exon ordering for features: `NBC_01310` (`NBC_0131000000000_213589.current.gb`) and `NBC_01080` (`NBC_0108000000000_76298.current.gb`)

## Repository Structure
- `data/`: Contains processed data used in the analysis.
  - `processed/G1032_20240208/`: [BGCFlow](https://github.com/NBChub/bgcflow) run result of the dataset.
    - `metadata/`: Contains JSON files with project metadata and dependency versions.
    - `tables/`: CSV files with summaries from antiSMASH and GTDB metadata.
- `figures/`: Contains figures generated from the analysis.
  - `strainmap_G1032_20240208.html`: Interactive map of strains.
- `notebook/`: Jupyter notebooks for analysis.
  - `strainmap_G1034.ipynb`: Notebook with the analysis code.
- `README.md`: This file, providing an overview of the repository.
- `strainmap_env.yaml`: Conda environment file to reproduce the analysis environment.
- `tables/`: Cleaned table with latitude and longitude data.
  - `df_antismash_7.1.0_summary_with_gps.csv`: Summary table with GPS coordinates.

## Getting Started
To replicate the analysis environment, use the provided `strainmap_env.yaml` file with Conda:

```bash
conda env create -f strainmap_env.yaml
```

Activate the environment:
```bash
conda activate strainmap_env
```

You can then open the Jupyter notebook in the `notebook/` directory to explore the analysis.

## Data Description
The `data/` directory contains processed datasets from [BGCFlow](https://github.com/NBChub/bgcflow) run used in the analysis. Metadata files describe the project context and software dependencies. The tables provide summaries of genomic features and metadata relevant to the NPGM isolates/strains.

## Figures
The `figures/` directory includes interactive maps generated from the analysis, allowing for a visual exploration of the strain distributions.

## Notebooks
The `notebook/` directory contains Jupyter notebooks that detail the analysis process, from data processing to visualization.

## Conda Environment
The `strainmap_env.yaml` file specifies the Conda environment necessary to run the analysis, ensuring reproducibility.

## Tables
Processed tables, including summaries with GPS coordinates, are provided in the `tables/` directory for further analysis and reference.
