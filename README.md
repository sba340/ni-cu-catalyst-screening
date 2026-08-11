# Ni-Cu Catalyst Adsorption Screening

Machine-learning-accelerated screening of ethylidyne (coking-precursor surrogate) adsorption energies on Ni-Cu bimetallic catalyst surfaces of varying composition, using Meta FAIR's FAIRChem (formerly Open Catalyst Project) universal machine-learned interatomic potentials as a fast surrogate for DFT.

## Overview

This workflow supports ongoing research into coke resistance in Ni-Cu bimetallic catalysts for renewable diesel production (biomass-to-fuel conversion). It uses pretrained UMA models to rapidly screen thousands of adsorption configurations before validating top candidates with DFT.

## Contents

- Adsorption energy calculation and trajectory relaxation (GPU/CPU)
- Batch processing across catalyst compositions
- AdsorbML-based site sampling, including a pure-Ni and pure-Cu baseline
- Large-scale (10,000+ structure) adsorption energy distribution analysis

## Requirements
A Hugging Face account/token is required to download pretrained FAIRChem model checkpoints.

## Attribution

This workflow builds on models and tools from the Open Catalyst Project / FAIR Chemistry team at Meta AI.

```bibtex
@article{ocp_dataset,
  author  = {Chanussot et al.},
  title   = {Open Catalyst 2020 (OC20) Dataset and Community Challenges},
  journal = {ACS Catalysis},
  year    = {2021},
  doi     = {10.1021/acscatal.0c04525}
}
```

- FAIRChem code: [github.com/facebookresearch/fairchem](https://github.com/facebookresearch/fairchem)
- Documentation: [fair-chem.github.io](https://fair-chem.github.io/)

## Author

Sahar Bayat, PhD Candidate, Risko Lab, University of Kentucky
