# Welcome

Here you can explore the [concept of a genomic transmission graph](underlying-concepts.md) for modelling parasite transmission dynamics and population genetics.  This website accompanies a paper on this topic in [Wellcome Open Research](https://wellcomeopenresearch.org/articles/8-22).

Before getting started, take a quick look at [how to use this book](how-to-use-this-book.md) as it contains worked examples with Python code that you can run in the cloud for yourself even if you are new to programming.

Please go ahead and browse.  The sections aren't strictly ordered but this is a logical sequence to work through the scientific concepts:

1. [Underlying concepts](underlying-concepts.md)
1. [The basic model](basic-model.md)
1. [Time to coalescence](coalescence-time-basic.ipynb)
1. [Nucleotide diversity](nucleotide-diversity.ipynb)
1. [Haplotype homozygosity](haplotype-homozygosity.ipynb)
1. [Identity by descent](ibd.ipynb)
1. [Effect of migration](migration-simple.ipynb)
1. [Within-host diversity](within-host.ipynb)
1. Estimating the quantum of transmission
1. [*Hw - Hs* relationship](hw-hs.ipynb)
1. [Estimating the rate of superinfection](fws-compare-methods.ipynb)
1. [Epidemiological scenarios](epidemiological-scenarios.md)

Most of the worked examples use the Python package `coalestr` which works like this:

1. [First you create a `Population`](population-class.ipynb)
1. [Then you run `get_coalescent`](get-coalescent.ipynb)
1. [Then you run `get_diversity`](get-diversity.ipynb)
1. [To analyse a time series you specify observation times](time-series.ipynb)