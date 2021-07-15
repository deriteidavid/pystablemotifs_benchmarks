# PyStableMotifs_benchmarks
This repository contains benchmarking code to compare the PyStableMotifs package (https://github.com/jcrozum/PyStableMotifs) to several other software tools for the identification of Boolean network attractors.
<br>
Tools compared in the benchmarks:
* StableMotifs: https://github.com/jcrozum/PyStableMotifs
* GinSim-python: https://github.com/GINsim/GINsim-python
* boolSim-python: https://github.com/colomoto/boolSim-python
* CABEAN-python: https://github.com/algorecell/cabean-python
* pypint: https://github.com/pauleve/pypint
* PyBoolNet: https://github.com/hklarner/PyBoolNet
* stablemotifs (Java version - only compatible with  JRE/JDK 8): https://github.com/jgtz/StableMotifs

It is recommended that these be installed in the same environment in order to run the benchmarks in the most seamless manner. 

An up-to-date list of Boolean network analysis tools can be found at: https://colomoto.github.io/colomoto-docker/

Please contact the respective tool creators with queries regarding installation of these dependencies.

## benchmark_timings - Jupyter notebook

Comparison of attractor identification speeed on empirical models. The models should be in BooleanNet format (and \*.booleannet extension) in the _models_for_benchmark/_ folder. The code will automatically run all models in the folder and exporth the results into the _timing_results.xlsx_ excel file. <br>

For additional information, such as which methods are compared and the value of the timeout limit, see the notebook.

## benchmark_timings-RBN - Jupyter notebook

Comparison of attractor identification speed on ensembles of random Boolean networks (RBN). The RBNs should be in BooleanNet format (and \*.booleannet extension) in the _rbn_models_for_benchmark/_ folder. The notebook can also generate RBNs with a variety of parameters (see the the code for details). The code will automatically run all models in the folder and exporth the results into the _timing_results_RBN.xlsx_ excel.<br>

For additional information, such as which methods are compared and the value of the timeout limit, see the notebook.

## Benchmark_RBN_statistics_plotter - Jupyter notebook

The code processes the contents of _timing_results_RBN.xlsx_ and generates a boxplot figure summarizing the comparison between the methods. The for the detailed parameters of the plots such as which methods to include in the comparison, color schemes, etc. see the notebook.

*For questions and comments regarding the code and the bechmarks feel free to open an issue or contact me at deriteidavid@gmail.com.*
