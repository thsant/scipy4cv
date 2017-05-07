
# Introduction

## About these notebooks

These notebooks are part of the tutorial *[SciPy and OpenCV as an interactive
computing environment for computer
vision](http://emap.fgv.br/sibgrapi-2014/tutorials.html)*, first presented at
[SIBGRAPI 2014](http://emap.fgv.br/sibgrapi-2014/). The tutorial is also
available as a full paper in
[RITA](http://www.seer.ufrgs.br/rita/article/view/RITA-VOL22-NR1-154).

## What are we looking for in a computer environment?

- **Data exploration and visualization**
    - Images, video sequences, point clouds and feature vectors
- **Extensive list of tools**
    - Image processing
    - Machine learning
    - Optimization
    - Statistics
    - Linear algebra
- **High-performance computing** (HPC)
- Promote **reproducible research**

Computer vision practitioners need a computing environment that lets them
explore data like images, video sequences, point clouds and feature vectors.
Such an environment should help on the development and testing of new models and
algorithms, and on the deployment of the results, either as a final software
module or a scientific/technical publication. It should also provides a
*extensive* list of tools, routines for image processing, machine learning,
statistical inference, linear algebra, convex optimization and graph algorithms,
just to name a few. Problems involving large sets of images can require high-
performance computing (HPC) such that the environment should provide practical
ways to parallelize and distribute computation. An ideal environment should also
combine documentation and computation in a single bundle, promoting results
reproducibility, but preventing the research pipeline to become more cumbersome.

## A Python-based environment
![xkcd on Python](./figs/python.png)

[http://xkcd.com/353/](http://xkcd.com/353/) by Randall Munroe

- *SciPy*, a **scientific computing** environment based on Python
  - Developed in the last **12 years**
- Based on the **NumPy** module for $n$-dimensional arrays
- Not just software, but a **community**
  - This community meets at [SciPy Conferences](http://conference.scipy.org)

In the last twelve years, a powerful scientific computing environment emerged
from the Python programming community. This language is an attractive option for
researchers: it is interpreted (a wanted property for interactive computing
environments), dynamically typed,
and presents a very concise and elegant syntax, resembling the pseudo-code found
in computer science textbooks. But the tipping point for Python to become a
major player in scientific computing was the advent of an efficient module for
$n$-dimensional array
representation and manipulation. The Numarray module was created by [Greenfield
*et al.*](http://adsabs.harvard.edu/abs/2002adass..11..140G) to address
astronomical data analysis. In 2005, Numarray successor,
[NumPy](http://www.numpy.org/), appeared and became the workhorse of the Python
scientific computing. An active community composed of scientists and engineers
flourished around Python and NumPy, represented today by the SciPy Stack and the
[SciPy Conferences](http://conference.scipy.org).

## Why is an interactive environment important to computer vision?

In computer vision, the practitioner is interested in inferring the **world
state** from images, that act as **observations**. The statistical relation
between the world state and the observed images is defined by **models**. A
particular model is defined by **parameters**, chosen  by **learning
algorithms**. Finally, the world state is estimated by **inference algorithms**.

 This *vision on computer vision* is properly presented by Prince in [his
book](http://www.computervisionmodels.com/) and translates the state-of-the-art
of contemporary research in the field, which is deeply associated to machine
learning nowadays.

- Environment should enable tinkering with machine learning techniques
- Visualization and exploration tools to address problems involving:
    - generalization,
    - overfitting,
    - dimensionality reducion,
    - optimization
- The SciPy environment provides these capabilities

The development of these models and subsequent problems in learning and
inference require a computing environment that allows proper tinkering with
machine learning techniques. Visualization and exploration tools are necessary
to address problems involving generalization, overfitting, dimensionality
reduction and optimization. An interactive computing environment as
[IPython](ython.org/), enriched with tools from the SciPy Stack and the OpenCV
library, can address these needs.

## This tutorial presents:

- interactive computing *and* HPC with the **IPython** shell;
- **OpenCV** use under Python;
- **Matplotlib** for visualization and 2D plotting;
- the SciPy **scientific library** and
- machine learning with the **scikit-learn** module

* This tutorial provides a *glimpse*, not a broad and deep coverage
* Examples should provide a starting point for the insterested user

The present tutorial provides a short overview on this Python-based computing
environment. Considering the large set of tools available and the space
constraints, this tutorial does not pretend to be a complete reference or a
broad review. It provides just a glimpse of the environment's capabilities to
the computer vision community, briefly presenting and discussing some problems
and code examples. These examples can guide the user's first steps and the
provided references help on the next ones.

**IPython notebooks** presenting the complete code for the examples are
available on

[http://nbviewer.ipython.org/github/thsant/scipy4cv](http://nbviewer.ipython.org/github/thsant/scipy4cv)

and on GitHub:

[https://github.com/thsant/scipy4cv/tree/master/](https://github.com/thsant/scipy4cv/tree/master/)
