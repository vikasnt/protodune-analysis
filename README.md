# ProtoDUNE Analysis

ProtoDUNE-SP is an 800-tonne liquid argon detector at CERN, built as a full-scale prototype for the DUNE experiment. It images particle interactions in 3D by recording the trails of charge and light left behind as particles traverse the liquid argon. Example 2D projection of a particle interactino in ProtoDUNE-SP:

<img src="https://raw.githubusercontent.com/vikasnt/vikasnt/main/protodune_event.png" width="600px">

Raw detector signals are processed by Pandora, a multi-algorithm 3D reconstruction framework that identifies individual particle trajectories from wire readout data. Each reconstructed object is then scored by a convolutional neural network (CNN) trained to distinguish shower-like signatures from track-like ones, giving a probability score used in downstream analysis to select signal candidates.

This repository contains analysis code built on top of these reconstructed objects, for two studies using 1 GeV pion beam data:

**1. Neutral pion reconstruction**
Reconstructing photon pair signatures from neutral pion decays in 3D detector images, used to calibrate shower reconstruction and validate detector energy response.

**2. Pion production cross-section**
First measurement of the pion production channel in liquid argon, a key systematic input for neutrino energy reconstruction in DUNE.

## Tools
Python · C++ · ROOT · scikit-learn · NumPy · Matplotlib
