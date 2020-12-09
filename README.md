# Multilayer Least Square Based Neural Network with Recomputation for Multi-View Big Data Analysi
## Abstract:

Most multilayer least square (LS)-based neural networks are structured with two separate stages: unsupervised feature encoding and supervised pattern classification. Once the unsupervised learning is finished, the latent encoding will be fixed without supervised fine-tuning. However, in complex tasks (such as handling the ImageNet dataset), there are often many more clues than can be directly encoded, and the unsupervised learning, by definition cannot know exactly what is useful for a certain task. This serves as the motivation to retrain the latent space representations to learn some clues that unsupervised learning has not yet learned. We pull back the error from the output layer to each hidden layer and recalculate the parameters of the hidden layer with Moore-Penrose (MP) inverse for more generalized representations. In this paper, a recomputation-based multilayer network using MP inverse (RML-MP) is developed. Then, a sparse RML-MP (SRML-MP) model to boost the performance of RML-MP is then proposed. More precisely, the latent space weights of RML-MP and SRML-MP are updated with $\ell_{2}$ and $\ell_{1/2}$ penalty, respectively. The experimental results on different domains with a varying number of training samples (from $3\, K$ to $1.8\, M$) show that the proposed models provide better generalization performance than most representation learning algorithms.
## Contributions:
* I. Architecture side -  Two novel OCC algorithms called OC-SNN and MCOC-SNN are proposed. Specifically, i) to enhance the discriminitively of the latent space features, the MCC is used; ii) the subnetwork structure is used to develop the architectures; ii) the global-level representations of input pattern are generated through the proposed one-step learning strategy.

* II. Application side - The key contribution of this paper in terms of its application is the usage of OC-SNN and MCOC-SNN, which harnesses high-level abstract features to handle large-scale datasets with more than 500 K samples. Furthermore, the cross-domain validations verify the effectiveness of the proposed methods. 

## Learning Structure:

<img src="https://github.com/W1AE/OCC/blob/main/F.jpg" width="1050" height="430" />

## Related Work:

[1] Zhang, W. (2020). One-Class Classification Using Hierarchical Subnetwork-based Structure. IEEE Transactions on Systems, Man, and Cybernetics: Systems.

## Downloads:
### MNIST-2 (Visual Image Classification Domain)
* MNIST dataset: [MNIST DATASET](http://yann.lecun.com/exdb/mnist/)
* MNIST-2 features: [MNIST-2 (GoogLe Drive)](https://drive.google.com/file/d/1kWEMoIbtR8TKJq0X8btXrFqSetzOyHWH/view?usp=sharing) or [MNIST-2 (GitHub)](https://github.com/W1AE/OCC/blob/main/M_2.mat)
* Source code for MNIST-2: [SC-MNIST-2](https://github.com/W1AE/OCC/blob/main/Demo_MNIST.zip)
### NORB-2 (Visual Image Classification Domain)
* NORB dataset: [NORB DATASET](https://cs.nyu.edu/~ylclab/data/norb-v1.0-small/)
* NORB-2 features: [NORB-2 (GoogLe Drive)](https://drive.google.com/file/d/11CNibSMWIP77VYPBiN9-GEmDQT-jTWnl/view?usp=sharing)
* Source code for NORB-2: [SC-NORB-2](https://github.com/W1AE/OCC/blob/main/Demo_NORB.zip)
### Place-D (Visual Image Classification Domain)
* Place-365 dataset: [PLACE DATASET](http://places2.csail.mit.edu/)
* Place-D features: [PLACE-D (GoogLe Drive)](https://drive.google.com/file/d/18eULO1viweE_x5hOetlavGshYggIigVd/view?usp=sharing)
* Source code for Place-D: [SC-PLACE-D](https://github.com/W1AE/OCC/blob/main/Demo_Place.zip)
### Food identification (Extended Domain)
* Food-251 dataset: [FOOD DATASET](https://github.com/karansikka1/iFood_2019)
* Food+ features: [FOOD+ (GoogLe Drive)](https://drive.google.com/file/d/1UfG5LUW8CtTB7fc4sPZhMW6eHiV32opc/view?usp=sharing)
* Source code for Food+: [SC-FOOD+](https://github.com/W1AE/OCC/blob/main/Demo_Food.zip)
### Rumor detection (Extended Domain)
* Rumor dataset (Data collected from three major news agencies): [RUMOR DATASET](https://github.com/W1AE/OCC/blob/main/BL.csv)

#The rumor dataset is our newly collected dataset, here we only show part of the dataset. After acceptance of the manuscript (if decided so), the whole dataset will be released.

## Dependancies
* Matlab version 2020a,
* A workstation with a 256GB memory and an E5-2650 processor.

## Reproduce the Experimental Results

Run script "Coding_OCSNN.m" for original OC-SNN algorithm, run script "Coding_MCOCSNN.m" for the improved MCOC-SNN algorithm.

#The code is released in content-obscured version (p files). After acceptance of the manuscript (if decided so), the source code will be made public.

