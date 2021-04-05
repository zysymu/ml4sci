A repository containing my submissions for the evaluation test for prospective GSoC applicants for the DeepLense project. I applied for the **Domain Adaptation for Decoding Dark Matter with Strong Gravitational Lensing** project, and had to do the following tests:

- Common test (I): Simulating Superfluid Dark Matter (DM) with PyAutoLens: solution can be found [here](https://github.com/zysymu/ml4sci/blob/main/superfluid_dark_matter/simulation.ipynb)!
- Specific test (II): Learning the DM representation: solution can be found [here](https://nbviewer.jupyter.org/github/zysymu/ml4sci/blob/main/domain_adaptation/domain_adaptation.ipynb)! **NOTE:** I had to submit the evaluation test until March 24 and these last links are my original submissions. Since then I continued experimenting with AAEs and managed to get much better results and fix a lot of mistakes that I had made during my rush to finish the evaluation test on time. The new version can be seen in [this](https://github.com/zysymu/unsupervised-adversarial-autoencoder) repository (I choose to use a differente repo so that it doesn't interfere with the dates, but also added the `aae.ipynb` file here just for good measure)!

---

Below are the descriptions of each test:

### Common test (I): Simulating Superfluid Dark Matter (DM) with PyAutoLens 

Familiarize yourself with PyAutoLens: Refer to the following documentation for examples of how to simulate strong gravitational lensing.

What is PyAutoLens? — PyAutoLens

Task: Modify and/or use the already existing functionality of PyAutoLens to simulate strong lensing from superfluid dark matter. Specifically, you will need to simulate the effects of lensing from a linear mass density - imagine this being a string of mass on galactic scales.

### Specific test (II): Learning the DM representation

Unsupervised Anomaly Detection and Transfer Learning

The following link contains the network architecture and weights of an Adversarial Autoencoder trained on a large dataset of strong gravitational lensing images without substructure.

Link:
https://github.com/ML4SCI/ML4SCI_GSoC/tree/main/DeepLense/Domain%20Adaptation

Task: Use the provided model weights for weight initialization or feature extraction, and train an unsupervised deep learning algorithm of your choice to learn the distribution of the provided strong lensing images with no substructure to solve the task of unsupervised anomaly detection using PyTorch. Pick the most appropriate approach and discuss your strategy.                        
Dataset: https://github.com/ML4SCI/ML4SCI_GSoC/blob/main/DeepLense/Domain%20Adaptation/lenses.tgz
Dataset Description: A set of simulated strong gravitational lensing images with and without substructure. 
Evaluation Metrics: ROC curve (Receiver Operating Characteristic curve) and AUC score (Area Under the ROC Curve)
