[![INFORMS Journal on Computing Logo](https://INFORMSJoC.github.io/logos/INFORMS_Journal_on_Computing_Header.jpg)](https://pubsonline.informs.org/doi/10.1287/ijoc.2023.1281)

# Data for the Empirical Analysis of the Paper [Learning Equilibria in Asymmetric Auction Games]

This archive is distributed in association with the [INFORMS Journal on
Computing](https://pubsonline.informs.org/journal/ijoc) under the [General Public License v3.0](LICENSE).

The software in this repository is a snapshot of the software that was used in the research reported on in the paper [Learning Equilibria in Asymmetric Auction Games](tbd) by Martin Bichler, Stefan Heidekrüger ([@heidekrueger](https://github.com/heidekrueger)), Nils Kohring ([@kohring](https://github.com/kohring)). The snapshot is based on the `bnelearn` software library, and corresponds to [this release](https://github.com/heidekrueger/bnelearn/releases/tag/v1.1.0) in the development repository. 

**Important:** The underlying `bnelearn` software is being developed on an on-going basis at 
https://github.com/heidekrueger/bnelearn/. Please go there if you would like to get a more recent version or would like support. The documentation of the `bnelearn` software can be found at https://bnelearn.readthedocs.io/.

## Cite

To cite this software, please cite the [paper](https://pubsonline.informs.org/doi/10.1287/ijoc.2023.1281) using its DOI and the software itself, using the suggested citation in the `bnelearn` software repository linked above.

[![DOI](https://zenodo.org/badge/571825331.svg)](https://zenodo.org/badge/latestdoi/571825331)

If you need to cite _this specific version_ of the code, you may use the citation below:

```
@article{bnelearn-asymmetric,
  author    = {Bichler, Martin and Heidekr\"uger, Stefan and Kohring, Nils},
  publisher = {INFORMS Journal on Computing},
  title     = {{bnelearn-asymmetric} {V}ersion v2021.0151},
  year      = {2023},
  doi       = {https://zenodo.org/badge/latestdoi/571825331},
  note      = {available for download at https://github.com/INFORMSJoC/2021.0151}
}
```

## Description

The goal of this software is to demonstrate the demonstration of the empirical convergence behavior of the NPGA algorithm in asymmetric auction games. Please see the paper for details.

## Requirements and setup

To install the software and it's requirements, please follow the instructions at https://bnelearn.readthedocs.io/en/latest/usage/installation.html. The specific requirements for this snapshot of the code can also be found [here](bnelearn/docs/usage/installation.rst). 

## Results

The following table presents all asymmetric sealed-bid auctions were we successfully deployed the equilibrium learning algorithm with references to the corresponding sections in the IJOC article and in the code.

| Auction Setting                          | Reference in Paper | Reference in Code                                            |
| :---                                     | :---               | :---                                                         |
| single-item uniform overlapping FPSB     | Subsection 6.1.1   | [Script L31](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L31) |
| single-item uniform non-overlapping FPSB | Subsection 6.1.1   | [Script L32](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L32) |
| single-item beta asymmetric FPSB         | Subsection 6.1.2   | [Script L33](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L33) |
| multi-unit with 4 units                  | Section 6.2        | [Script L139](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L139) |
| multi-unit with 8 units                  | Section 6.2        | [Script L139](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L139) |
| multi-unit with 12 units                 | Section 6.2        | [Script L139](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L139) |
| LLG, adapted VCG                         | Section 6.3        | [Script L69](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L69) |
| split-award FPSB                         | Section 6.4        | [Script L106](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L106) |
| LLLLGG FPSB                              | Section 6.5        | [Script L190](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L190) |
| LLLLRRG FPSB                             | Section 6.5        | [Script L278](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py#L278) |

## Replicating

To replicate the experiments in the paper and the figures above, please follow the installation instructions above, then run this [script](https://github.com/heidekrueger/bnelearn/blob/a9a7d895295adf79f863c384535f2d4740dc88f0/scripts/run_experiments_asymmetric.py).

## Ongoing Development

This code is being developed on an on-going basis at the author's [GitHub site](https://github.com/heidekrueger/bnelearn/).

## Support

For support in using this software, submit an [issue](https://github.com/heidekrueger/bnelearn/issues/new).
