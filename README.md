## iVS1191: Genome-scale metabolic model of _Aurantiochytrium_ sp. T66

[![GitHub version](https://badge.fury.io/gh/AlmaasLab%2FiVS1191.svg)](https://badge.fury.io/gh/AlmaasLab%2FiVS1191) 
[![Zenodo](https://zenodo.org/badge/{{Zenodo ID}}.svg)](https://zenodo.org/badge/latestdoi/{{Zenodo ID}})

### Description

This repository contains the genome-scale metabolic model (GEM) of the thraustochytrid _Aurantiochytrium_ sp. T66. Considerably improving on the model quality and scope to that of previously published thraustochytrid GEMs, this model provides a great starting point for conducting research on thraustochytrids as microbial cell factories.

### Citation

If you use iVS1191 please cite the following paper:
> Simensen, V., Voigt, A., Almaas, E. High-quality genome-scale metabolic model of Aurantiochytrium sp. T66. Biotechnology and Bioengineering, 118:2105–2117 (2021) [doi:10.1002/bit.27726](https://doi.org/10.1002/bit.27726)

### Keywords

**Utilisation:** model template; _in silico_ strain design; multi-omics integrative analysis  
**Field:** metabolic-network reconstruction  
**Type of model:** reconstruction; curated  
**Model source:** [iVS1191](https://doi.org/10.1002/bit.27726)  
**Omic source:** genomics; transcriptomics; metabolomics  
**Taxonomic name:** _Aurantiochytrium_ sp. T66  
**Taxonomy ID:** [taxonomy:1749249](https://identifiers.org/taxonomy:1749249)   
**Genome ID:** [insdc.gca:GCA_001462505.1](https://identifiers.org/insdc.gca:GCA_001462505.1)   
**Metabolic system:** general metabolism  
**Condition:** aerobic; glucose-limited; defined media

### Installation

If you want to use the model, any software that accepts SBML L3V1 FBCv3 formatted model files will work. We recommend the following as they are well-maintained and used by most researchers in the constraint-based metabolic modeling community:
* MATLAB
  * [COBRA Toolbox](https://github.com/opencobra/cobratoolbox)
  * [RAVEN Toolbox](https://github.com/SysBioChalmers/RAVEN)
* Python
  * [cobrapy](https://github.com/opencobra/cobrapy)

### Usage

The following code shows how the model can be read and written:
* In Matlab using either COBRA or RAVEN:
  ```matlab
  cd ./code
  % For RAVEN use toolbox="raven" instead
  model = loadT66Model(toolbox='cobra'); % loading
  saveT66Model(model, toolbox='cobra');    % saving
  ```

* In Python using cobrapy:
  ```python
  import code.io as io
  model = io.read_t66_model() # loading
  io.write_t66_model(model)   # saving
  ```


### Contributing

Contributions are always welcome! Please read the [contributing guideline](.github/CONTRIBUTING.md) to get started.


### Contributors

Code contributors are reported automatically by GitHub under [Contributors](https://github.com/{{organization or username}}/{{repository name}}/graphs/contributors), while other contributions come in as [Issues](https://github.com/{{organization or username}}/{{repository name}}/issues).