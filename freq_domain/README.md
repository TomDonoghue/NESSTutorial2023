# Hands-On Materials: Spectral Parameterization

These materials are hands-on tutorials and problem sets for working with spectral parameterization.

## Overview

These materials include:
- 00-Setup: a notebook for getting setup & started with the key tools
- 01-SpecParamModel: a notebook for practicing fitting spectral models to example data
- 02-Simulations: a notebook exploring using simulations to test and explore data properties and methods
- 03-RealData: a notebook to explore using spectral parameterization on a real dataset

## Learning Goals

Learning goals for this workshop include to:
- Explore and understand the assumptions of common analysis methods, and how these relate to empirical data
- Use hands-on, practical examples to demonstrate how common analysis methods may conflate periodic and aperiodic activity
- Learn how to use the spectral parameterization method to measure periodic and aperiodic features from neural power spectra
- Apply spectral parameterization to empirical data

## Key Tools & Resources

This section of the tutorial will focus on the following modules:

**specparam: Spectral Parameterization**

The `specparam` module (formerly `fooof`) is an open-source Python module for parameterizing neural power spectra into periodic and aperiodic components. This module will be used for fitting spectral models, and analyzing and visualizing the results.

Documentation:      https://specparam-tools.github.io
Source Code:        https://github.com/fooof-tools/fooof

**NeuroDSP: Neuro Digital Signal Processing**

The `neurodsp` module is a general purpose open-source Python module that includes tools to analyze neural data, with a focus on digital signal processing. It also includes a sub-module for simulating neural time series, which we will use in this workshop.

Documentation:      https://neurodsp-tools.github.io/
Source Code:        https://github.com/neurodsp-tools/neurodsp

**Oscillations Methods Project**

The `OscillationsMethods` project is a project that explores properties of neural oscillations and how these relate to common measures, and includes visualizers and open-code for topics related to these materials.

Website:            https://oscillationmethods.github.io/docs/index.html
