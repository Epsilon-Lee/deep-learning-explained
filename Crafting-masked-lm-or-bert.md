
The [The art of crafting dl](https://github.com/Epsilon-Lee/deep-learning-explained/blob/main/The-art-of-crafting-dl.md) series is very ambitious, as I put in that file (below), and from the beginning, I would like to get started with bert-based model for nlp and transformers for cv.
> _"So I would like to do the Jigsaw Puzzle, where I first write several pieces, and organize my writings locally, and then start to put them together under a coherent logic."_

So the first question I would like to answer is: what is the outline of [bertology](A Primer in BERTology: What we know about how BERT works) that I would like to cover?

An top-down approach is to follow the construction of "The art of crafting dl" file, i.e. discuss and experiments with the elements of bert and making bert work, including the following topics:
- **Architectural Design**: the post-norm vs pre-norm, the role of multi-head design, reidual and feed-forward layer.
- **Optimization Design**: learning rate schedule and warming-up.
- **Learning Objective Design**: the ratio of masking, the various objectives for dependency learning, e.g. xlnet, electra, autoregressive, filling-the-blank etc.

Another bottom-up approach is to list several influential papers as follows, and summrize the core problems they have studied:
- [On the variance of the adaptive learning rate and beyond](https://arxiv.org/pdf/1908.03265), Oct. 26 2021. `about optimization of bert`.
