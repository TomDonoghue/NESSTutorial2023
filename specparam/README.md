# Title

Words, words, words.

## Overview

In **Part 1** we will cover an overview of the key tools, following along with the module documentation.

Part 1 will use the following materials:
- the [neurodsp module documentation](https://neurodsp-tools.github.io/neurodsp/auto_tutorials/index.html)
- the [specparam module documentation](https://fooof-tools.github.io/fooof/auto_tutorials/index.html)

In **Part 2** we will cover a tutorial including hands-on problems that explore key topics.

Part 2 will use the following materials:
- the [specparam problem set](https://github.com/fooof-tools/Tutorial)

## Learning Goals

Learning goals for this workshop include to:
- Explore and understand the assumptions of common analysis methods, and how these relate to empirical data
- Use hands-on, practical examples to demonstrate how common analysis methods may conflate periodic and aperiodic activity
- Learn how to use the spectral parameterization method to measure periodic and aperiodic features from neural power spectra, including choosing appropriate parameters, doing quality control on model fits, and interpreting results
- Apply spectral parameterization to empirical datasets, from different modalities and experimental designs

## Key Tools

This section of the tutorial will focus on the following modules:

**NeuroDSP: Neuro Digital Signal Processing**

The `neurodsp` module is a general purpose open-source Python module that includes tools to analyze neural data, with a focus on digital signal processing. It also includes a sub-module for simulating neural time series, which we will use in this workshop.

Documentation:      https://neurodsp-tools.github.io/
Source Code:        https://github.com/neurodsp-tools/neurodsp

**specparam: Spectral Parameterization**

The `specparam` module (formerly `fooof`) is an open-source Python module for parameterizing neural power spectra into periodic and aperiodic components. This module will be used for fitting spectral models, and analyzing and visualizing the results.

Documentation:      https://specparam-tools.github.io
Source Code:        https://github.com/fooof-tools/fooof
