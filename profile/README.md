This page is about the research on phase-field methods at the [Camille Jordan Institute (ICJ) of the University of Claude-Bernard Lyon 1, France](http://math.univ-lyon1.fr/?lang=en).

# Last article

[Learning phase field mean curvature flows with neural networks, Bretin & Denis & Masnou & Terii, 2022](https://www.sciencedirect.com/science/article/pii/S0021999122006416) and on [arXiv](https://arxiv.org/abs/2112.07343).

**Abstract:**
We introduce in this paper new and very effective numerical methods based on neural networks for the approximation of the mean curvature flow of either oriented or non-orientable surfaces. To learn the correct interface evolution law, our neural networks are trained on phase field representations of exact evolving interfaces. The structures of the networks draw inspiration from splitting schemes used for the discretization of the Allen-Cahn equation. But when the latter approximate the mean curvature motion of oriented interfaces only, the approach we propose extends very naturally to the non-orientable case. Through a variety of examples, we show that our networks, trained only on flows of smooth and simplistic interfaces, generalize very well to more complex interfaces, either oriented or non-orientable, and possibly with singularities. Furthermore, they can be coupled easily with additional constraints which opens the way to various applications illustrating the flexibility and effectiveness of our approach: mean curvature flows with volume constraint, multiphase mean curvature flows, numerical approximation of Steiner trees or minimal surfaces. 


# Python package for the learning process of mean curvature flow

About making a neural network learn a mean curvature flow (oriented or not, isotropic or anisotropic), we have developped a dedicated module [nnpf](https://pypi.org/project/nnpf/) (see also the [GitHub repository](https://github.com/PhaseFieldICJ/nnpf)) that features problems (type of mean curvature flows to learn) and associated datasets, signed distance for many shapes, fast convolution using FFT, visualization...

It relies on [PyTorch](https://pytorch.org/) and [Lightning](https://www.pytorchlightning.ai/).


# Interactive painter in 2D

![nnpf](https://user-images.githubusercontent.com/10435058/207285788-97c68200-e19d-4657-9d94-abda977152dc.png)

In [nnpf_paint2d](https://github.com/PhaseFieldICJ/nnpf_paint2d) you can find a Python script to play with mean curvature flows in 2D, to add inclusion or exclusion constraints, visually compare oriented and non-oriented flows, isotropic and anisotropic energy...

Three already learned neural networks are included for the oriented isotropic, non-oriented isotropic and non-oriented anisotropic cases.
