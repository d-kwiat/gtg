# Welcome

Here you can explore the [concept of a genomic transmission graph](underlying-concepts.md) for modelling parasite transmission dynamics and population genetics.  This website accompanies a paper on this topic in BioRxiv (link TBD).

Before getting started, take a quick look at [how to use this book](how-to-use-this-book.md) as it contains worked examples with Python code that you can run in the cloud for yourself even if you are new to programming.

The sections aren't strictly ordered but this is a logical sequence to work through the scientific concepts:

1. [Underlying concepts](underlying-concepts.md)
1. [The basic model](basic-model.md)
   * [Time to coalescence](coalescence-time-basic.ipynb)
   * [Nucleotide diversity](nucleotide-diversity.ipynb)
   * [Haplotype homozygosity](haplotype-homozygosity.ipynb)
   * [Identity by descent](ibd.ipynb)
1. [Within-host diversity](within-host.ipynb)
   * [Estimating the quantum of transmission](within-host-pi.ipynb)
   * [*Hw - Hs* relationship](hw-hs.ipynb)
   * [Estimating the rate of superinfection](fws-compare-methods.ipynb)
1. [Migration and population structure](migration-simple.ipynb)
   * [Creating a metapopulation](create-metapopulation.ipynb)
   * [Creating a subpopulation](create-subpopulation.ipynb)
1. [Modelling epidemiological scenarios](epidemiological-scenarios.md)
   * [Time series analysis](time-series.ipynb)
   * [Transient scenarios](transient-scenarios.ipynb)
   * [Local outbreak](local-outbreak.ipynb)

Most of the worked examples use the Python package `coalestr` which works like this:

1. [First you create a `Population`](create-population.ipynb)
1. [Then you run `get_coalescent`](get-coalescent.ipynb)
1. [Then you run `get_diversity`](get-diversity.ipynb)
1. [You can create a subpopulation with migration from a metapopulation](create-subpopulation.ipynb)
1. [To analyse a time series you specify observation times](time-series.ipynb)