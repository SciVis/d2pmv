# Supplemental Material for "A Visual Environment for Data Driven Protein Modeling and Validation"

## bS6m - Ribosomal Protein
This protein is part of the mitochondrial ribosome of yeast _Saccharomyces cerevisiae_ [^1] and consists of 2206 atoms of which 1126 are hydrogen atoms that were added after modeling. The corresponding density map (`b6m_density_map.mrc`) and the derived local resolution (`b6m_local_resolution.mrc`) have dimensions of 60 x 60 x 60 voxels.

### Atomic models
+ `bS6m.pdb` - the initial model
+ `bS6m_bad.pdb` - refined model obtained through automated fitting to the density map
+ `bS6m_refined.pdb` - deteriorated model with approx. 1/3 of the atoms' positions modified

### Validation metrics
+ `*.resmetrics.csv` - per-residue validation metrics
+ `*.clashes.csv` - aggregated atom clash scores (max score per atom)
+ `*.clashes-full.txt` - all pair-wise clashes between atoms


## Chloroplast Ribosome (PDB-ID: 6ERI, EM Map: EMD-3941)
This spinach chloroplast ribosome (PDB-ID: [6ERI](https://www.rcsb.org/structure/6ERI), EM Map: [EMD-3941](https://www.ebi.ac.uk/emdb/EMD-3941)}) is involved in oxygenic photosynthesis [^2]. The structure was obtained at 3Å resolution and comprises 145000 atoms distributed over 11094 residues. For some of the chains, including about 5000 residues, we were not able to produce any validation metrics as those are marked as ``unknown''.

### Atomic model & maps
+ `6eri.cif` - atomic structure of [6ERI](https://www.rcsb.org/structure/6ERI)
+ `emd_3941.map` - density map (not included), accessible via the Electron Microscopy Data Bank [EMD-3941](https://www.ebi.ac.uk/emdb/EMD-3941)
+ `emd_3941_resmap.map` - local resolution derived from the density map and its halfmaps

### Validation metrics
+ `6eri.resmetrics.csv` - per-residue validation metrics
+ `6eri.clashes.csv` - aggregated atom clash scores (max score per atom)
+ `6eri.clashes-full.txt` - all pair-wise clashes between atoms


[^1]: N. Desai, A. Brown, A. Amunts, and V. Ramakrishnan, "The structure of the yeast mitochondrial ribosome," Science, vol. 355, no. 6324, pp. 528–531, 2017.

[^2]: A. P. Boerema, S. Aibara, B. Paul, V. Tobiasson, D. Kimanius, B. O.
Forsberg, K. Wallden, E. Lindahl, and A. Amunts, "Structure of the chloroplast ribosome with chl-RRF and hibernation-promoting factor," Nature plants, vol. 4, no. 4, pp. 12–217, 2018.
