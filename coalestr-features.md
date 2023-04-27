# How to use `coalestr`

We can use `coalestr` to evaluate the genetic diversity of a parasite population. There are three stages to this process: 

1. [Creating a `Population`](create-population.ipynb) by specifying its history of transmission parameters.
2. [Running `get_coalescent`](get-coalescent.ipynb) to perform a Markov chain simulation of coalescence times.
3. [Running `get_diversity`](get-diversity.ipynb) to evaluate nucleotide diversity and haplotype homozygosity using the simulated coalescence times.

We can [create a subpopulation](create-subpopulation.ipynb) by specifying the metapopulation within which it is embedded and by giving the rate of migration from the metapopulation into the subpopulation.

We can [analyse a time series](time-series.ipynb) by specifying a set of observation times.  At each observation time we sample two alleles from the population and perform a simulation of their times to coalescence.

You can view the [Python code for the `coalestr` module](https://github.com/d-kwiat/coalestr-python/blob/main/coalestr/cs.py).