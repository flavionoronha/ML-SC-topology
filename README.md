# ML-SC-topology
In this Jupyter Notebook we use machine learning (ML) methods to predict the topological invariant Bott index of disordered superconductors. If the Bott index is nonzero, the superconductor is topologically nontrivial and hosts Majorana quasiparticles. These Majorana states are known for their potential to be a building bloch for quantum computing. The precise calculation of the Bott index demands high computational resources. If we are able to predict this index using a ML method, we can save time and computational resources.

The input data is extracted from Green's functions of the superconductors which I computed using a Fortran code. For each value of the chimical potential (denoted 'mu') and magnetic dilution (denoted 'p'), we have data of several realizations of superconductors. Our goal is to build the topological phase diagram of the Bott index ('B') as a function of mu and p. 

We load the data for p=0, which we use to train different ML models. We also load the data whose labels we will predict. We have data for mu ranging from -7 to 0 and p ranging from 0 to 1. Then, we recover the full phase diagram, which is known from the reference [1].

The best method was based on neural networks with no hidden layer, indicating that the correlations between labels and features are linear. The precise calculation of the Bott index demands high computational resources and we are able to make quick accurate predictions of this topological index using ML methods, which require less computational resources.

## INSTRUCTIONS:
1. The input data and the Fortran code are not shared at this moment once our research is not published yet.
2. The analysis of the data is available in the Jupyter Notebook.

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
