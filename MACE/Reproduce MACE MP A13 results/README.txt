his notebook reproduces results from Section A.13 of MACE MP paper for tungsten (W), molybdenum ()Mo and niobium (Nb) benchmarks using the MACE foundation model (MACE-MP-0 and MACE-MP-FT). It provides a reference for evaluating model accuracy and extracting benchmark properties comparable to DFT data.

Overview

The notebook runs inference with pre-trained MACE models to obtain benchmark properties as described in Section A.13 of the MACE MP paper:

Lattice constant

ΔE–V curve

Elastic constants (C11, C12, C44)

Vacancy formation energy


Requirements

Python ≥ 3.9

ase, torch, mace, numpy, matplotlib

Access to the pre-trained MACE-MP-0 and MACE-MP-FT models


Usage

Open the notebook in Jupyter or Colab.

Run the cells sequentially to generate the benchmark plots and summary tables.


MACE MP paper citation:
I. Batatia, P. Benner, Y. Chiang, A. M. Elena, D. P. Kovács, J. Riebesell, X. R. Advincula, M. Asta, M. Avaylon, W. J. Baldwin, F. Berger, N. Bernstein, A. Bhowmik, S. M. Blau, V. Cărare, J. P. Darby, de Sandip, F. Della Pia, V. L. Deringer, R. Elijošius, Z. El-Machachi, F. Falcioni, E. Fako, A. C. Ferrari, A. Genreith-Schriever, J. George, R. E. A. Goodall, C. P. Grey, P. Grigorev, S. Han, W. Handley, H. H. Heenen, K. Hermansson, C. Holm, J. Jaafar, S. Hofmann, K. S. Jakob, H. Jung, V. Kapil, A. D. Kaplan, N. Karimitari, J. R. Kermode, N. Kroupa, J. Kullgren, M. C. Kuner, D. Kuryla, G. Liepuoniute, J. T. Margraf, I.-B. Magdău, A. Michaelides, J. H. Moore, A. A. Naik, S. P. Niblett, S. W. Norwood, N. O'Neill, C. Ortner, K. A. Persson, K. Reuter, A. S. Rosen, L. L. Schaaf, C. Schran, B. X. Shi, E. Sivonxay, T. K. Stenczel, V. Svahn, C. Sutton, T. D. Swinburne, J. Tilly, C. van der Oord, E. Varga-Umbrich, 
 T. Vegge, M. Vondrák, Y. Wang, W. C. Witt, F. Zills, G. Csányi, A foundation model for atomistic materials chemistry; 30/12/2023.