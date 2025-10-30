ACE Calculator & A13 Benchmarks

This notebook provides scripts and analysis routines for benchmarking Atomic Cluster Expansion (ACE) models against DFT and MACE-MP-0 reference data for tungsten (W), molybdenum (Mo) and niobium (Nb), following the methodology described in Section A.13 of the MACE MP paper.

Overview

The notebook automates the evaluation of ML interatomic potentials through:

Computing energy and force errors for ACE, MACE, and DFT reference datasets

Benchmarking key material properties:

ΔE–V curve

Lattice constant

Elastic constants (C11, C12, C44)

Vacancy formation energies

Comparing ACE-DFT, ACE-MACE-MP-0, and ACE-MACE-MP-FT, and models generated for different hyperparameters and dataset sizes

Structure

Setup & Imports – load dependencies, models, and datasets

ACE Calculator Initialization – configure linear ACE potential parameters

Benchmark Routines – evaluate the models on the tungsten dataset

Plotting & Analysis – generate comparison plots for A.13 benchmarks

Requirements

Python ≥ 3.9

ase, numpy, matplotlib, pandas, mace, acepotentials

Access to DFT or MACE reference datasets (.xyz or .csv format)

Usage

Place your model and dataset files in the working directory

Open the notebook

Run all cells sequentially to reproduce benchmark plots and tables

Output

The notebook generates:

Energy/force error statistics (MAE, RMSE)

A.13 benchmark plots (ΔE–V, elastic constants, vacancy formation energy)

Tables summarizing ACE and MACE model performance

MACE MP paper citation:
I. Batatia, P. Benner, Y. Chiang, A. M. Elena, D. P. Kovács, J. Riebesell, X. R. Advincula, M. Asta, M. Avaylon, W. J. Baldwin, F. Berger, N. Bernstein, A. Bhowmik, S. M. Blau, V. Cărare, J. P. Darby, de Sandip, F. Della Pia, V. L. Deringer, R. Elijošius, Z. El-Machachi, F. Falcioni, E. Fako, A. C. Ferrari, A. Genreith-Schriever, J. George, R. E. A. Goodall, C. P. Grey, P. Grigorev, S. Han, W. Handley, H. H. Heenen, K. Hermansson, C. Holm, J. Jaafar, S. Hofmann, K. S. Jakob, H. Jung, V. Kapil, A. D. Kaplan, N. Karimitari, J. R. Kermode, N. Kroupa, J. Kullgren, M. C. Kuner, D. Kuryla, G. Liepuoniute, J. T. Margraf, I.-B. Magdău, A. Michaelides, J. H. Moore, A. A. Naik, S. P. Niblett, S. W. Norwood, N. O'Neill, C. Ortner, K. A. Persson, K. Reuter, A. S. Rosen, L. L. Schaaf, C. Schran, B. X. Shi, E. Sivonxay, T. K. Stenczel, V. Svahn, C. Sutton, T. D. Swinburne, J. Tilly, C. van der Oord, E. Varga-Umbrich, 
 T. Vegge, M. Vondrák, Y. Wang, W. C. Witt, F. Zills, G. Csányi, A foundation model for atomistic materials chemistry; 30/12/2023.