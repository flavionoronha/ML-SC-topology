# ML-SC-topology
In this project we use machine learning (ML) methods to predict the topological invariant Bott index of disordered superconductors. If the Bott index is nonzero, the superconductor is topologically nontrivial and hosts Majorana quasiparticles. These Majorana states are known for their potential to be a building bloch for quantum computing. The precise calculation of the Bott index demands high computational resources. If we are able to predict this index using a ML method, we can save time and computational resources.

The input data is extracted from Green's functions of the superconductors which I computed using a Fortran code. We have data for chimical potential (denoted 'mu') ranging from -7 to 0 and magnetic dilution (denoted 'p') ranging from 0 to 1. For each value of mu and p, we have data of several realizations of superconductors. Our goal is to build the topological phase diagram of the Bott index ('B') as a function of mu and p. 

We present two Jupyter Notebooks. In one of them, we train the models using all values of p and mu. In the other Jupyter Notebook we train the models using only the data with p=0, for which we have analytical results. With both Notebooks we predict B for all values of mu and p and recover the full phase diagram, which is known from reference [1].

The precise calculation of the Bott index demands high computational resources and we are able to make quick accurate predictions of this topological index using ML methods, which require less computational resources.

## INSTRUCTIONS:
1. The input data and the Fortran code are not shared at this moment once our research is not published yet.
2. The analysis of the data is available in the Jupyter Notebooks.
3. In the Jupyter notebook 'LDOS_full.ipynb' we train the models using all values of p and mu.
4. In the Jupyter notebook 'LDOS_p0.ipynb' we train the models using p=0 and all values of mu.

## Acknowledgements
We acknowledge funding from CNPq.

## Giving Credit

This repository can be cited using:
```
@software{ML-SC-topology,
  author = {Flavio Noronha},
  title = {ML-SC-topology},
  url = {https://github.com/flavionoronha/ML-SC-topology},
  year = {2023},
}
```

## Bibliography
[1] Eric Mascot et al., Phys. Rev. B 100, 235102 (2019).
