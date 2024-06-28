

The title of my booklet is "The Art of Crafting Deep Learning".
I decide to write this booklet to really make myself grasp the philosophy and craftmanship of deep learning, the machine learning field that continues to make technical breakthroughs (e.g. Large Language Models) and leverage world-changing products (e.g. ChatGPT).
However, as said by [xxx], the field is advancing by continuous optimization improvements, inductive bias innovations and scaling up that are separately conducted by different individuals and groups within the whole community.
And no one can grasp the motivation and reasoning behind these historically distributed byt systemantic exploration as a whole.
This booklet is aiming to provide a biased perspective on my effort for achieving the above goal.

I would like to first survey several introductory books about deep learning, a non-exhaustive list is the following (see [here](https://github.com/Carl-McBride-Ellis/Compendium-of-free-ML-reading-resources?tab=readme-ov-file#deep-learning--neural-networks) for a more complete list of books):
- "Deep Learning", Ian Goodfellow et al. 2016.
- "Dive into Deep Learning", Aston Zhang, 2021.
- "The Little Book of Deep Learning", Francois Fleuret, 2023.
- "Understanding Deep Learning", Simon J. D. Prince, 2023.
- "Deep Learning: Foundations and Concepts", Chris Bishop et al. 2024.

After extracting the key technical advancements along these years from the books (most of them are textbooks), I would like to further discuss and experiment more on the following topics under the light of optimization theory, generalization theory and learning dynamics:
- **optimization methods**: for example, how learning rate warmup stabilizes gradient descent from finetuned models (how about random initialized model);
- **input representations**: for example, the acceleration of learning with feature binning and embedding than original numerical ones in tabular deep learning;
- **initialization methods**: for example, the acceleration of optimization via weight transpose and tying in autoencoders;
- **architectural inductive biases**: for example, how highway net and resnet alleviate gradient diminishing, how normalization techniques accelerate optimization;
- **scaling up and double descent**: for example, do scaling up really accelerate learning and improve generalization in all kinds of neural architectures;




