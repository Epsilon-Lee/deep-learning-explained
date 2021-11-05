
# Deep learning explained

A collection of papers that try to explain the mysteries of deep learning with theories and empirical evidences.


## Theory-oriented explanations


### Training: SGD, learning dynamics, curriculum

- [Stochastic Training is Not Necessary for Generalization](https://arxiv.org/pdf/2109.14119.pdf), Tom Goldstein's group, `nips2021`.
- [Large Learning Rate Tames Homogeneity: Convergence and Balancing Effect](https://arxiv.org/pdf/2110.03677.pdf), Tuo Zhao's group.
- [Momentum Doesn't Change The Implicit Bias](https://arxiv.org/pdf/2110.03891.pdf).
- [On the Implicit Biases of Architecture & Gradient Descent](https://arxiv.org/pdf/2110.04274.pdf), 2021, Yisong Yue's group, `implicit bias` of `gd`
- [Parameter Prediction for Unseen Deep Architectures](https://arxiv.org/pdf/2110.13100.pdf), Oct. 25 2021.

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


### Interpolation and Extrapolation

- [Learning in High Dimension Always Amounts to Extrapolation](https://arxiv.org/abs/2110.09485), Oct. 18 2021, Yann LeCun et al.


## Empirical explanations

### Data-centric understanding

- [Deep Learning Through the Lens of Example Difficulty](https://arxiv.org/pdf/2106.09647.pdf), Google Research 2021.
- [Deep Learning on a Data Diet: Finding Important Examples Early in Training](https://arxiv.org/pdf/2107.07075.pdf), Jul. 15 2021. `nips2021`


### Generalization metrics

- [Neural Tangent Kernel Eigenvalues Accurately Predict Generalization](https://arxiv.org/pdf/2110.03922.pdf), UCB，`nips2021` spotlight. 
- [Predicting Unreliable Predictions by Shattering a Neural Network](https://arxiv.org/abs/2106.08365), 2021, Yoshua Bengio's group.


### Other learning paradigms related to deep learning

- [Towards a theory of out-of-distribution learning](https://arxiv.org/pdf/2109.14501.pdf), JHU 2021.
