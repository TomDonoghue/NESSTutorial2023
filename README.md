# NESS Tutorial 2023

This repository hosts materials for the "Advanced topics in the analysis of neural electrophysiology data: decomposing rhythmic and broadband components" short course, for [NESS 2023](https://symposium.nestat.org/index.html).

## Overview

Neural electrophysiological signals reflect complex combinations of multiple underlying sources, such that traditional approaches from time-series and digital signal processing can often conflate multiple overlapping features, complicating accurate interpretations of the underlying physiology. In particular, recent methodological work has shown how the complexity of neural data – which can include multiple rhythmic features, transient events and aperiodic activity as well as interactions between these features and traversals between discrete states – requires dedicated methods to accurately measure features of interest.

This short course will introduce statistical tools to model and decompose neural electrophysiological signals into physiologically informed features of interest, including rhythmic and broadband components. The presenters will present brief lectures on:
- (1) using frequency-domain spectral decomposition to estimate and separate rhythmic peaks from broadband power spectral signatures, and
- (2) using state space models to capture time-domain rhythms and their interactions. Following each lecture, attendees will use interactive notebooks to explore the methods in hands-on tutorials.

## Software Environment

The materials in this tutorial require the Python programming language, as well as Jupyter notebooks. Participants will need a working install of Python (>=3.6), with standard scientific packages (numpy, scipy, matplotlib), as well as some neuroscience specific modules.

To assist with getting an environment setup, we have provided an environment file which can be initialized as:


    > git clone ***
    > cd NESSTutorial2023
    > conda env create -f environment.yml
    > conda activate NESSTutorial2023
    > jupyter lab

The above assumes you have the [conda](https://docs.conda.io/en/latest/) package manager, which can be downloaded as part of the [Anaconda distribution](https://www.anaconda.com/download).

## Acknowledgements

Special thanks to:
- David W. Zhou, PhD, Carney Institute for Brain Science, Brown University, Providence, RI, USA
- Matteo Fecchio, PhD, Center for Neurotechnology and Neurorecovery, Massachusetts General Hospital, Boston, MA, USA
