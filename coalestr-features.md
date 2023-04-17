# How to use `coalestr`

We can use `coalestr` to obtain the genetic diversity of a parasite population by Markov chain simulation of coalescence times.  There are three stages to this process: 

1. [Creating a `Population`](create-population.ipynb) by specifying its history of transmission parameters.
2. [Running `get_coalescent`](get-coalescent.ipynb) to perform a simulation of coalescence times in our population.
3. [Running `get_diversity`](get-diversity.ipynb) to estimate nucleotide diversity and haplotype homozygosity using our simulated coalescence times.

We can also [analyse a time series](time-series.ipynb) by specifying a set of observation times.  At each observation time we sample two alleles from the population and perform a simulation of their times to coalescence.

You can view the [Python code for the `coalestr` module](https://github.com/d-kwiat/gtg/blob/main/coalestr.py).

