
# Deep learning explained

A collection of papers that try to explain the mysteries of deep learning with theories and empirical evidences. And [here](https://hanin.princeton.edu/paper_list.pdf) is a curated resource of deep learning theory papers by Prof. Boris Hanin at Princeton.

- [Theory-oriented explanations](#theory-oriented-explanations)
  - [Differential equation view](#differential-equation-view)
  - [Interpolation-Extrapolation tradeoffs](#interpolation-extrapolation-tradeoffs)
  - [Deep PAC and PAC-Bayes](#deep-pac-and-pac-bayes)
  - [Information-theoretic](#information-theoretic)
  - [Theory of training](#theory-of-training)
    - [Neural Tangent Kernel](#neural-tangent-kernel)
    - [Understanding training tricks](#understanding-training-tricks)
  - [Implicit regularization](#implicit-regularization)
  - [Theory of representation learning](#theory-of-representation-learning)

- [Empirical observations and explanations](#empirical-observations-and-explanations)
  - [Self-supervised learning](#self-supervised-learning)
  - [Contrastive learning](#contrastive-learning)
  - [Generalization metrics](#generalization-metrics)
  - [Decision boundary](#decision-boundary)
  - [Data-centric understanding](#data-centric-understanding)
  - [Spurious correlation](#spurious-correlation)
  - [Lottery ticket hypothesis](#lottery-ticket-hypothesis)
  - [Memorization](#memorization)

## Theory-oriented explanations

### Differential equation view

- [The Principles of Deep Learning Theory](https://arxiv.org/abs/2106.10165), Jun. 18 2021.

### Interpolation-Extrapolation tradeoffs

- [Learning in High Dimension Always Amounts to Extrapolation](https://arxiv.org/abs/2110.09485), Oct. 18 2021, Yann LeCun et al.
- [Benign, Tempered, or Catastrophic: A Taxonomy of Overftting](https://arxiv.org/pdf/2207.06569.pdf), Jul. 14 2022.

### Inductive Bias

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

### Deep PAC and PAC-Bayes

- [How Tight Can PAC-Bayes be in the Small Data Regime?](https://arxiv.org/pdf/2106.03542.pdf), Oct. 27 2021.

### Information-theoretic 

- [Towards a Unified Information-Theoretic Framework for Generalization](https://arxiv.org/pdf/2111.05275.pdf), Nov. 9 2021. `nips2021` Daniel Roy's group. `non-vacuous generalization bound`

### Theory of training

> SGD, loss landscape, learning dynamics, stochacity, sgd for feature learning, learning curriculum etc.

- [Don't Decay the Learning Rate, Increase the Batch Size](https://arxiv.org/abs/1711.00489#), Nov. 2017. `iclr2018`.
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
- [The Limiting Dynamics of SGD: Modified Loss, Phase Space Oscillations, and Anomalous Diffusion](https://arxiv.org/pdf/2107.09133.pdf), Dec. 2 2022.
- [Understanding Gradient Descent on Edge of Stability in Deep Learning](https://arxiv.org/pdf/2205.09745.pdf), May 22 2022.
- [Understanding Edge-of-Stability Training Dynamics with a Minimalist Example](https://arxiv.org/pdf/2210.03294.pdf), Oct. 7 2022.
- [Neural Networks can Learn Representations with Gradient Descent](https://arxiv.org/abs/2206.15144), Jun. 30 2022. `colt2022`
- [Git Re-Basin: Merging Models modulo Permutation Symmetries](https://arxiv.org/abs/2209.04836), Sep. 11 2022. [tweet1](https://twitter.com/SamuelAinsworth/status/1569719494645526529?cxt=HBwWgsDRtYnk4cgrAAAA&cn=ZmxleGlibGVfcmVjcw%3D%3D&refsrc=email), [tweet2](https://twitter.com/iamtrask/status/1569809615398883328?cxt=HBwWgMC-reXhiskrAAAA&cn=ZmxleGlibGVfcmVjcw%3D%3D&refsrc=email), [tweet3](https://twitter.com/boazbaraktcs/status/1569744030090817539?cxt=HBwWhsDT3Zz47MgrAAAA&cn=ZmxleGlibGVfcmVjcw%3D%3D&refsrc=email).
- [The Dynamics of Sharpness-Aware Minimization: Bouncing Across Ravines and Drifting Towards Wide Minima](https://arxiv.org/pdf/2210.01513.pdf), Oct. 4 2022.
- [From Gradient Flow on Population Loss to Learning with Stochastic Gradient Descent](https://arxiv.org/pdf/2210.06705.pdf), Oct. 13 2022.
- [Grokking phase transitions in learning local rules with gradient descent](https://arxiv.org/pdf/2210.15435.pdf), Oct. 26 2022.
- [High-dimensional Asympototics of Feature Learning: How One Gradient Step Improves the Representation](https://arxiv.org/pdf/2205.01445.pdf), Jimmy Ba et al. arXiv May 3 2022.
- [Exact learning dynamics of deep linear networks with prior knowledge](https://openreview.net/pdf?id=lJx2vng-KiC), `nips2022`. `learning dynamics`.
- [Handbook of Convergence Theorems for (Stochastic) Gradient Methods](https://arxiv.org/abs/2301.11235), Jan. 26 2023.

#### Neural Tangent Kernel

- [Learning sparse features can lead to overfitting in neural networks](https://arxiv.org/pdf/2206.12314.pdf), Jun. 24 2022.
- [Limitations of the NTK for Understanding Generalization in Deep Learning](https://arxiv.org/abs/2206.10012), Jun. 20 2022.
- [The Influence of Learning Rule on Representation Dynamics in Wide Neural Networks](https://arxiv.org/pdf/2210.02157.pdf), Oct. 5 2022.

#### Understanding training tricks

- [Does Knowledge Distillation Really Work?](https://arxiv.org/pdf/2106.05945.pdf), Jun. 10 2021. `nips2021`
- [Understanding Why Generalized Reweighting Does Not Improve Over ERM](https://arxiv.org/pdf/2201.12293.pdf), Jan. 28 2022.

### Implicit regularization

- [Limitation of characterizing implicit regularization by data-independent functions](https://arxiv.org/pdf/2201.12198.pdf), Jan. 28 2022.
- [Implicit Bias in Leaky ReLU Networks Trained on High-Dimensional Data](https://arxiv.org/pdf/2210.07082.pdf), Oct. 2022.

### Theory of representation learning

- [Neural Networks Efficiently Learn Low-Dimensional Representations with SGD](https://arxiv.org/pdf/2209.14863.pdf), Sep. 29 2022. `sgd`
- [Deep Learning meets Nonparametric Regression: Are Weight-Decayed DNNs Locally Adaptive?](https://arxiv.org/pdf/2204.09664.pdf), Jun. 13 2022.
- [Feature learning in neural networks and kernel machines that recursively learn features](https://arxiv.org/pdf/2212.13881.pdf), Dec. 28 2022.
  - From Mikhail Belkin's group.

#### Self-supervised learning

- [Exploring the Limits of Large Scale Pre-training](https://arxiv.org/pdf/2110.02095.pdf), Google Research.

##### Contrastive learning

- [The Power of Contrast for Feature Learning: A Theoretical Analysis](https://arxiv.org/pdf/2110.02473.pdf), Oct. 2021. James Zou's group.
- [Sharp Learning Bounds for Contrastive Unsupervised Representation Learning](https://arxiv.org/pdf/2110.02501.pdf), Oct. 2021. RIKEN AIP.
- [Can contrastive learning avoid shortcut solutions?](https://arxiv.org/pdf/2106.11230.pdf), Jun. 21 2021. MIT and Pittsburg univ.
- [Intriguing Properties of Contrastive Losses](https://arxiv.org/pdf/2011.02803.pdf), Oct. 23 2021. Google Research.
- [Stochastic Contrastive Learning](https://arxiv.org/pdf/2110.00552.pdf), Oct. 2021. `interpretability`
- [How Does Contrastive Pre-training Connect Disparate Domains?](https://openreview.net/pdf?id=ZKCw3atVfsy), `nipst2021`
- [Contrastive Learning Can Find An Optimal Basis for Approximately View-Invariant Functions](https://arxiv.org/pdf/2210.01883.pdf), arXiv Oct. 4 2022.
- [Do More Negative Samples Necessarily Hurt In Contrastive Learning?](https://arxiv.org/pdf/2205.01789.pdf), Jun. 22 2022. `icml2022`.
- [Understanding Deep Contrastive Learning via Coordinate-wise Optimization](https://arxiv.org/pdf/2201.12680.pdf), `nips2022`.
- [Understanding Contrastive Learning Requires Incorporating Inductive Biases](https://arxiv.org/pdf/2202.14037.pdf), Feb. 28 2022.
- [Feature Dropout: Revisiting the Role of Augmentations in Contrastive Learning](https://sslneurips22.github.io/paper_pdfs/paper_60.pdf), Dec. 15 2022.

#### Explaining representational power

- [Emergence of Invariance and Disentanglement in Deep Representations](https://jmlr.org/papers/volume19/17-646/17-646.pdf), `jmlr2018`
- [Grounding Representation Similarity with Statistical Testing](https://arxiv.org/pdf/2108.01661.pdf), Nov. 3 2021. `representation comparison`
- [Revisiting Model Stitching to Compare Neural Representations](https://arxiv.org/pdf/2106.07682.pdf), Jun. 14 2021. `representation comparison`
- [Comparing Text Representations: A Theory-Driven Approach](https://arxiv.org/pdf/2109.07458.pdf), Sep. 2021. `sentence embedding`
- [Discovering and Explaining The Representation Bottleneck of DNNs](https://openreview.net/forum?id=iRCUlgmdfHJ), `iclr2022 submit`

---

## Empirical observations and explanations

### Double descent

- [Double Descent Demystified: Identifying, Interpreting & Ablating the Sources of a Deep Learning Puzzle](https://arxiv.org/pdf/2303.14151.pdf), Mar. 24 2023.

### Mechanistic interpretability of DL

- [An Extremely Opinionated Annotated List of My Favourite Mechanistic Interpretability Papers](https://www.neelnanda.io/mechanistic-interpretability/favourite-papers), Oct. 18 2022.

### Generalization metrics

- [Neural Tangent Kernel Eigenvalues Accurately Predict Generalization](https://arxiv.org/pdf/2110.03922.pdf), UCB，`nips2021` spotlight. 
- [Predicting Unreliable Predictions by Shattering a Neural Network](https://arxiv.org/abs/2106.08365), 2021, Yoshua Bengio's group.
- [On Predicting Generalization using GANs](https://arxiv.org/pdf/2111.14212.pdf), Nov. 28 2021.
- [Intrinsic Dimension, Persistent Homology and Generalization in Neural Networks](https://arxiv.org/pdf/2111.13171.pdf), Nov. 25 2021.

#### Flatness

- [On the Maximum Hessian Eigenvalue and Generalization](https://arxiv.org/pdf/2206.10654.pdf), Jun. 22 2022.

### Decision boundary

- [Can You Learn the Same Model Twice? Investigating Reproducibility and Double Descent from the Decision Boundary Perspective](https://somepago.github.io/files/db_preprint.pdf), Dec. 16 2021.

### Data-centric understanding

- [Deep Learning Through the Lens of Example Difficulty](https://arxiv.org/pdf/2106.09647.pdf), Google Research 2021.
- [Deep Learning on a Data Diet: Finding Important Examples Early in Training](https://arxiv.org/pdf/2107.07075.pdf), Jul. 15 2021. `nips2021`

### Spurious correlation

See [here](https://github.com/Epsilon-Lee/paper-jam/blob/main/topics/ood-related-topics-and-generalization-mystery.md#spurious-correlation) for the detailed discussion on spurious correlation.

### Lottery ticket hypothesis

- [Can You Win Everything with A Lottery Ticket?](https://openreview.net/forum?id=JL6MU9XFzW), TMLR 2022.

### Memorization

- [Network size and weights size for memorization with two-layers neural networks](https://arxiv.org/pdf/2006.02855.pdf), Nov. 3 2020.
- [What Do Neural Networks Learn When Trained With Random Labels?](https://papers.nips.cc/paper/2020/file/e4191d610537305de1d294adb121b513-Paper.pdf), `nips2020`.
- [Neural Networks Learning and Memorization with (almost) no Over-Parameterization](https://proceedings.neurips.cc/paper/2020/file/662a2e96162905620397b19c9d249781-Paper.pdf), `nips2020`.
- [On the geometry of generalization and memorization in deep neural networks](https://openreview.net/forum?id=V8jrrnwGbuc), `iclr2021`.
- [The Curious Case of Benign Memorization](https://arxiv.org/abs/2210.14019), Oct. 25 2022.
  - _"only the very last layers are used for memorization, while preceding layers encode performant features which remain largely unaffected by the label noise"_
- [Distinguishing rule and exemplar-based generalization in learning systems](https://proceedings.mlr.press/v162/dasgupta22b.html), `icml2022`.
  - The experiment setting has been applied to study in-context ability of Transformers [tweet](https://twitter.com/scychan_brains/status/1580563395891597312).
- [Unintended memorisation of unique features in neural networks](https://arxiv.org/pdf/2205.10079.pdf), May 20 2022.
