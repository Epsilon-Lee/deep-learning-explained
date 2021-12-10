
# Deep learning explained

A collection of papers that try to explain the mysteries of deep learning with theories and empirical evidences.


## Theory-oriented explanations

### Neural Tangent Kernel, and PAC-Bayes

- [How Tight Can PAC-Bayes be in the Small Data Regime?](https://arxiv.org/pdf/2106.03542.pdf), Oct. 27 2021.

### Information-theoretic

- [Towards a Unified Information-Theoretic Framework for Generalization](https://arxiv.org/pdf/2111.05275.pdf), Nov. 9 2021. `nips2021` Daniel Roy's group. `non-vacuous generalization bound`

### Training: SGD, learning dynamics, curriculum

- [Stochastic Training is Not Necessary for Generalization](https://arxiv.org/pdf/2109.14119.pdf), Tom Goldstein's group, `nips2021`.
- [Large Learning Rate Tames Homogeneity: Convergence and Balancing Effect](https://arxiv.org/pdf/2110.03677.pdf), Tuo Zhao's group.
- [Momentum Doesn't Change The Implicit Bias](https://arxiv.org/pdf/2110.03891.pdf).
- [On the Implicit Biases of Architecture & Gradient Descent](https://arxiv.org/pdf/2110.04274.pdf), 2021, Yisong Yue's group, `implicit bias` of `gd`
- [Parameter Prediction for Unseen Deep Architectures](https://arxiv.org/pdf/2110.13100.pdf), Oct. 25 2021.
- [Gradient Starvation: A Learning Proclivity in Neural Networks](https://arxiv.org/pdf/2011.09468.pdf), Oct. 26 2021. `nips2021`
- [What training reveals about neural network complexity](https://arxiv.org/pdf/2106.04186.pdf), Oct. 29 2021.
- [A Loss Curvature Perspective on Training Instabilities of Deep Learning Models](https://openreview.net/forum?id=OcKMT-36vUs), `iclr2022 submit`
- [Permutation-Based SGD: Is Random Optimal?](https://openreview.net/forum?id=YiBa9HKTyXE), `iclr2022 submit`
- [A General Analysis of Example-Selection for Stochastic Gradient Descent](https://openreview.net/forum?id=7gWSJrP3opB), `iclr2022 submit`
- [How many degrees of freedom do we need to train deep networks: a loss landscape perspective](https://arxiv.org/pdf/2107.05802.pdf), Jul. 13 2021.
- [The Benefits of Implicit Regularization from SGD in Least Squares Problems](https://arxiv.org/abs/2108.04552), Aug. 10 2021 `nips2021`

#### Training tricks

- [Does Knowledge Distillation Really Work?](https://arxiv.org/pdf/2106.05945.pdf), Jun. 10 2021. `nips2021`


### Understanding inductive bias: architectural bias, algorithmic bias etc.

- [On Margin Maximization in Linear and ReLU Networks](https://arxiv.org/pdf/2110.02732.pdf), Nathan Srebro's group, 2021.
- [The Role of Permutation Invariance in Linear Mode Connectivity of Neural Networks](https://arxiv.org/pdf/2110.06296.pdf), 2021, Google Research.
- [On the Implicit Biases of Architecture & Gradient Descent](https://arxiv.org/pdf/2110.04274.pdf), 2021, Yisong Yue's group.
  - *"This paper finds that while typical networks that fit the training data already generalise fairly well, gradient
descent can further improve generalisation by selecting networks with a large margin."*
- [The Deep Bootstrap Framework: Good Online Learners Are Good Offline Generalizers](https://arxiv.org/pdf/2010.08127.pdf), Feb. 2021. `iclr2021`
- [No One Representation to Rule Them All: Overlapping Features of Training Methods](https://arxiv.org/pdf/2110.12899.pdf), Oct. 26 2021.
- [Gradient Descent on Two-layer Nets: Margin Maximization and Simplicity Bias](https://arxiv.org/abs/2110.13905), Oct. 26. 2021.
- [Diversity and Generalization in Neural Network Ensembles](https://arxiv.org/pdf/2110.13786.pdf), Oct. 6 2021.
- [The Limitations of Large Width in Neural Networks: A Deep Gaussian Process Perspective](https://arxiv.org/pdf/2106.06529.pdf), Jun. 11 2021.


### Interpolation and Extrapolation

- [Learning in High Dimension Always Amounts to Extrapolation](https://arxiv.org/abs/2110.09485), Oct. 18 2021, Yann LeCun et al.


## Empirical explanations

### Understanding representation learning

### Self-supervised learning

- [Exploring the Limits of Large Scale Pre-training](https://arxiv.org/pdf/2110.02095.pdf), Google Research.

#### Contrastive learning

- [The Power of Contrast for Feature Learning: A Theoretical Analysis](https://arxiv.org/pdf/2110.02473.pdf), Oct. 2021. James Zou's group.
- [Sharp Learning Bounds for Contrastive Unsupervised Representation Learning](https://arxiv.org/pdf/2110.02501.pdf), Oct. 2021. RIKEN AIP.
- [Can contrastive learning avoid shortcut solutions?](https://arxiv.org/pdf/2106.11230.pdf), Jun. 21 2021. MIT and Pittsburg univ.
- [Intriguing Properties of Contrastive Losses](https://arxiv.org/pdf/2011.02803.pdf), Oct. 23 2021. Google Research.
- [Stochastic Contrastive Learning](https://arxiv.org/pdf/2110.00552.pdf), Oct. 2021. `interpretability`

### Explaining representational power

- [Grounding Representation Similarity with Statistical Testing](https://arxiv.org/pdf/2108.01661.pdf), Nov. 3 2021. `representation comparison`
- [Revisiting Model Stitching to Compare Neural Representations](https://arxiv.org/pdf/2106.07682.pdf), Jun. 14 2021. `representation comparison`
- [Comparing Text Representations: A Theory-Driven Approach](https://arxiv.org/pdf/2109.07458.pdf), Sep. 2021. `sentence embedding`
- [Discovering and Explaining The Representation Bottleneck of DNNs](https://openreview.net/forum?id=iRCUlgmdfHJ), `iclr2022 submit`

### Data-centric understanding

- [Deep Learning Through the Lens of Example Difficulty](https://arxiv.org/pdf/2106.09647.pdf), Google Research 2021.
- [Deep Learning on a Data Diet: Finding Important Examples Early in Training](https://arxiv.org/pdf/2107.07075.pdf), Jul. 15 2021. `nips2021`


### Generalization metrics

- [Neural Tangent Kernel Eigenvalues Accurately Predict Generalization](https://arxiv.org/pdf/2110.03922.pdf), UCB，`nips2021` spotlight. 
- [Predicting Unreliable Predictions by Shattering a Neural Network](https://arxiv.org/abs/2106.08365), 2021, Yoshua Bengio's group.
- [On Predicting Generalization using GANs](https://arxiv.org/pdf/2111.14212.pdf), Nov. 28 2021.
- [Intrinsic Dimension, Persistent Homology and Generalization in Neural Networks](https://arxiv.org/pdf/2111.13171.pdf), Nov. 25 2021.

### Other learning paradigms related to deep learning

- [Towards a theory of out-of-distribution learning](https://arxiv.org/pdf/2109.14501.pdf), JHU 2021.
