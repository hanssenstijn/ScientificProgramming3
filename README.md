# Parallel computing
`main.Rmd` is the R markdown notebook. The notebook imports molecules in `.sdf` format. The `.sdf` file can be downloaded from [PubChem](https://pubchem.ncbi.nlm.nih.gov/bioassay/624202). Go to `download`, then open `Tested Substances` and click on the `Structures SDF`. A subset of molecules is iteratively imported and their molecular descriptors will be computed in parallel. The parallel computing was done once with 3 cores and the second time with 2 cores. The molecules had to be converted into smiles for the parallel computing. Each core will eventually parse back the smiles into the molecules.

The hosted compiled notebook can be found [here](https://hanssenstijn.github.io/ScientificProgramming3/main.nb.html). 
In order to repdroduce the compiled notebook files can be downloaded from [github](https://github.com/hanssenstijn/ScientificProgramming3) and [PubChem](https://pubchem.ncbi.nlm.nih.gov/bioassay/624202). The working directory has to be changed in the notebook. The working memory, subset number of molecules and the number of cores that are used can be adjusted to personal preferences in the notebook.

The licenses for the used R packages can be founde here: [parallel & doParallel](https://cran.r-project.org/web/licenses/GPL-2), [rcdk](https://cran.r-project.org/web/licenses/LGPL-3) and
[itertools](https://cran.r-project.org/web/licenses/GPL-2)