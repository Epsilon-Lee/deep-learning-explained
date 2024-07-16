
```text
***[UPDATE]***
- Jul. 16 2024: add regularization item in the outline.
```

The title of my booklet is "The Art of Crafting Deep Learning".
I decide to write this booklet to really make myself grasp the philosophy and craftmanship of deep learning, the machine learning field that continues to make technical breakthroughs (e.g. Large Language Models) and leverage world-changing products (e.g. ChatGPT).
However, as said by [xxx], the field is advancing by continuous optimization improvements, inductive bias innovations and scaling up that are separately conducted by different individuals and groups within the whole community.
And no one can grasp the motivation and reasoning behind these historically distributed byt systemantic exploration as a whole.
This booklet is aiming to provide a biased perspective on my effort for achieving the above goal.

I would like to first survey several introductory books about deep learning, a non-exhaustive list is the following (see [here](https://github.com/Carl-McBride-Ellis/Compendium-of-free-ML-reading-resources?tab=readme-ov-file#deep-learning--neural-networks) for a more complete list of books):
- *"Deep Learning", Ian Goodfellow et al. 2016.*
- *"Dive into Deep Learning", Aston Zhang, 2021.*
- *"The Little Book of Deep Learning", Francois Fleuret, 2023.*
- *"Understanding Deep Learning", Simon J. D. Prince, 2023.*
- *"Deep Learning: Foundations and Concepts", Chris Bishop et al. 2024.*

After extracting the key technical advancements along these years from the books (most of them are textbooks), I would like to further discuss and experiment more on the following topics under the light of optimization theory, generalization theory and learning dynamics:
- **Optimization Methods**: for example, how learning rate warmup stabilizes gradient descent from finetuned models (how about random initialized model);
- **Input Representations**: for example, the acceleration of learning with feature binning and embedding than original numerical ones in tabular deep learning;
- **Initialization Methods**: for example, the acceleration of optimization via weight transpose and tying in autoencoders;
- **Architectural Inductive Biases**: for example, how highway net and resnet alleviate gradient vanishing, how normalization techniques accelerate optimization;
  - [Training Very Deep Networks](https://arxiv.org/abs/1507.06228), Jul. 22 2015.
  - [Deep Residual Learning for Image Recognition](https://arxiv.org/abs/1512.03385), Dec. 10 2015.
  - [Learning sparse neural networks through L0 regularization](https://openreview.net/pdf?id=H1Y8hhg0b), ICLR 2018.
- **Regularization**: for example, how to impose sparsity on neural networks, and how to avoid overfitting (dropout, label-smoothing).
- **Scaling-up and Double Descent**: for example, do scaling up really accelerate learning and improve generalization in all kinds of neural architectures;

***2024/7/1***.
I realize that starting to write this booklet from top-down is very difficult based on my current knowledge.
So I would like to do the Jigsaw Puzzle, where I first write several pieces, and organize my writings locally, and then start to put them together under a coherent logic.

- **Normalization techniques**. The first topic I want to start with is normalization, an architectural component that accelerates optimization and improve generalization. See [this](https://github.com/Epsilon-Lee/deep-learning-explained/blob/main/topics/normalization.md) markdown file for the details.


