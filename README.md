### Flow Matching for Reaction Coordinates

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.14257538.svg)](https://doi.org/10.5281/zenodo.14257538)

Authors: Mingyuan Zhang, Zhicheng Zhang, Yong Wang and Hao Wu

The implementation and analysis scripts for the paper "Flow Matching for Optimal Reaction Coordinates of Biomolecular System". For a detailed description of the algorithm, please refer to: https://pubs.acs.org/doi/full/10.1021/acs.jctc.4c01139

There are three folders under the main directory, each corresponding to the files and scripts for each model system to reproduce the results in the paper. The files in each folder are similar:

- `FMRC_training.ipynb` contains the implementation of the FMRC algorithm and the code for training FMRC models.
- `RC_comparison.ipynb` contains all the analysis scripts necessary to reproduce the figures presented in the main text and SI of the paper. 
- Under the `traj_and_dat/` folder, `features.dat` (for all neural network-based algorithms) and `features_tica.dat` (for TICA only) are `PLUMED` scripts we used to create the featurized trajectory dataset for RC learning. `input.pdb` is the topology file we used for the `PLUMED` driver utility. The generated `COLVAR` files are usually placed under a separate `COLVAR/` directory. We do not provide the `COLVAR` file here due to the copyright reason and the large file size.

We thank D. E. Shaw Research for providing their ultralong trajectories used in this study. Feel free to ask any question related to the paper at this Github page or by email mingyuanzhang@zju.edu.cn.

Please cite the following articles if you find this repositary useful:
1. Zhang, M., Zhang, Z., Wu, H., & Wang, Y. (2024). Flow Matching for Optimal Reaction Coordinates of Biomolecular Systems. Journal of Chemical Theory and Computation.
2. Zhang, Z., Guo, L., & Wu, H. (2024). Optimal Low-dimensional Approximation of Transfer Operators via Flow Matching: Computation and Error Analysis. arXiv preprint arXiv:2408.15981.
