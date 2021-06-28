# PyStableMotifs_benchmarks
This is a collection of tools to run benchmarks of the PyStableMotifs package https://github.com/jcrozum/PyStableMotifs
<br>
Tools compared in the benchmarks (recommended to install them in the same conda environment):
* StableMotifs: https://github.com/jcrozum/PyStableMotifs
* GinSim-python: https://github.com/GINsim/GINsim-python
* boolSim-python: https://github.com/colomoto/boolSim-python
* CABEAN-python: https://github.com/algorecell/cabean-python
* pypint: https://github.com/pauleve/pypint
* PyBoolNet: https://github.com/hklarner/PyBoolNet
* stablemotifs (Java version - only compatible with  JRE/JDK 8): https://github.com/jgtz/StableMotifs

An up-to-date list of all the tools can be found at: https://colomoto.github.io/colomoto-docker/

## benchmark_timings - Jupyter notebook

Comparison of finding attractors on empirical models. The models should be in BooleanNet format (and \*.booleannet extension) in the _models_for_benchmark/_ folder. The code will automatically run all models in the folder and exporth the results into the _timing_results.xlsx_ excel. <br>
For further parameters, such as which methods to compare and the timeout limit see the notebook.

## benchmark_timings-RBN - Jupyter notebook


Comparison of finding attractors on ensembles of random Boolean networks (RBN). The RBNs should be in BooleanNet format (and \*.booleannet extension) in the _rbn_models_for_benchmark/_ folder. The notebook can also generate RBNs with a variety of parameters (see the the code for details). The code will automatically run all models in the folder and exporth the results into the _timing_results_RBN.xlsx_ excel.<br>
For further parameters, such as which methods to compare and the timeout limit see the notebook.

## Benchmark_RBN_statistics_plotter - Jupyter notebook

The code processes the contents of _timing_results_RBN.xlsx_ and generates a boxplot figure summarizing the comparison between the methods. The for the detailed parameters of the plots such as which methods to include in the comparison, color schemes, etc. see the notebook.

### Note on compatibility
Getting all the methods to work together in the same environment proved to be a difficult task, and difficult to reproduce on new installs, due to some unclear  incompatibilities. We are working on a foolproof way to get everything working smoothly and will update the repository as things progress.

*For questions and comments regarding the code and the bechmarks feel free to open an issue or contact me at deriteidavid@gmail.com.*
