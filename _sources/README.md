# Introduction

Welcome!  This website introduces the concept of a **genomic transmission graph** for modelling parasite transmission dynamics and population genetics.  It accompanies the paper on this topic that is published in [Wellcome Open Research](https://wellcomeopenresearch.org/articles/8-22).

We will use code to examine specific examples of the genomic transmission graph.  You may want to look at the [glossary](glossary.md).

There are four main parts to this book.

1. We describe how to use this book.  It allows you to use interactive programming to work through examples.  This will require using an interactive cloud computing service and you will need to get [set up to use Google Colab](using-google-colab.md). 

1. We will briefly describe the underlying concepts of the genomic transmission graph.  You can also fast forward to the [glossary](glossary.md).

1. We will look at specific features of the 'coalestr' module.

1. We will play around with some epidemiological scenarios.



The remainder of this page can be deleted once the content is all in place.

## A framework for analysing the coalescent process

- [Time to coalescence - a basic version showing all the steps](coalescence_time_basic.ipynb)
- [Time to coalescence using `coalestr`](coalescence_time.ipynb)
- [Time to coalescence - examples using `coalestr`](coalescence_time_examples.ipynb)

## Genetic variation at a point locus

- [Nucleotide diversity of the global population](diversity_global.ipynb)

## Genetic variation at a haplotype locus

- [Haplotype homozygosity of a 2 centimorgan locus](haplotype_homozygosity_27kb.ipynb)
- [Variation of homozygosity with haplotype length](haplotype_homozygosity_vs_length.ipynb)
- [IBD metrics vs Nh](ibd_vs_nh.ipynb)

## Population structure and migration

- [Effect of global dispersal on local genetic diversity](migration_simple.ipynb)
- [Hierarchical population structure](hierarchical_population_structure.ipynb)
- [Migration and Fst](migration_Fst.ipynb)
- [Migration time series](migration_time_series.ipynb)

## Fws methods

- [Hw versus Hs](hw_vs_hs.ipynb)
- [Fws compare methods](fws_compare_methods.ipynb)

## Time series epidemiological scenarios

- [Species history](species_history.ipynb)
- [Scenarios #1](scenario_1.ipynb)
- [Local outbreak](local_outbreak.ipynb)

## `coalestr` module

- [View the code](coalestr.py)
