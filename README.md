### Flow Matching for Reaction Coordinates

Authors: Mingyuan Zhang, Zhicheng Zhang, Yong Wang and Hao Wu

The implementation and analysis scripts for the paper "Flow Matching for Optimal Reaction Coordinates of Biomolecular System". Currently under review, arxiv preprint: https://arxiv.org/abs/2408.17139. 

There are three folders under the main directory, each corresponding to the files and scripts for each model system to reproduce the results in the paper. The files in each folder are similar:

- `FMRC_training.ipynb` contains the implementation of the FMRC algorithm and the code for training FMRC models.
- `RC_comparison.ipynb` contains all the analysis scripts necessary to reproduce the figures presented in the main text and SI of the paper. 
- Under the `traj_and_dat/` folder, `features.dat` (for all neural network-based algorithms) and `features_tica.dat` (for TICA only) are `PLUMED` scripts we used to create the featurized trajectory dataset for RC learning. `input.pdb` is the topology file we used for the `PLUMED` driver utility. The generated `COLVAR` files are usually placed under a separate `COLVAR/` directory. We do not provide the `COLVAR` file here due to the copyright reason and the large file size.
- In addition, we provide all trained models in the form of `*.pt` files under the folder `models/` in the zip file we uploaded to Zenodo at https://zenodo.org/records/13474614.

We thank D. E. Shaw Research for providing their ultralong trajectories used in this study. Feel free to ask any question related to the paper at this Github page or by email mingyuanzhang@zju.edu.cn.
