# Underlying concepts

The genetic structure of a parasite population is shaped by its transmission dynamics - but superinfection, cotransmission and recombination make this relationship complex and hard to analyse.  

*Superinfection* means that a host acquires infection from multiple independent sources, and therefore carries a mixture of parasite genotypes with different ancestral histories, which may then be *cotransmitted* to other hosts.  *Recombination* within genetically mixed infections causes different regions of the genome to have different genealogies.  This presents an extremely complex problem for genetic inference of parasite transmission dynamics.

![superinfection](superinfection.png)
[See figure caption](superinfection.md)

The **genomic transmission graph** aims to simplify the problem.  It is a directed acyclic graph in which the nodes represent hosts and edges represent vectors, as illustrated below. The graph is plotted on an axis of time and we make the simplifying assumption that a host exists at a discrete point in time.

![transmission-graph](transmission-graph.png)
[See figure caption](transmission-graph.md) 

If we pick any node and trace a path forward in time along the edges to some other node, that is a *transmission chain*. Transmission chains can *branch* when a host is the source of parasites for multiple other hosts.  Transmission chains can also *cross* when a host acquires parasites from multiple sources, i.e when there is superinfection.

Parasites reproduce as they flow along transmission chains, and parasites that are flowing along the same transmission chain can genetically recombine with each other.

A *lineage* is a path through the transmission graph that we define by taking an allele at a point locus and tracing its ancestry back in time through the generations ([see glossary](glossary.md)). 

An individual parasite could have many different lineages each following a unique path back in time because, whenever transmission chains cross, the paths of different lineages can diverge. 

Thus the genomic transmission graph allows for superinfection and recombination because lineages at different loci within an individual parasite can take different pathways through the graph.  

Our challenge is to define the essential parameters of the genomic transmission graph and to understand how they are related to genetic variation.  To understand the scientific concepts you could work through the sections of this book in the following order:

1. [The basic model](basic-model.md)
   * [Time to coalescence](coalescence-time-basic.ipynb)
   * [Nucleotide diversity](nucleotide-diversity.ipynb)
   * [Haplotype homozygosity](haplotype-homozygosity.ipynb)
   * [Identity by descent](ibd.ipynb)
1. [Migration and population structure](migration-simple.ipynb)
   * [Creating a metapopulation](create-metapopulation.ipynb)
   * [Creating a subpopulation](create-subpopulation.ipynb)
1. [Within-host diversity](within-host.ipynb)
   * [Using $\pi_W$ to estimate the quantum of transmission $Q$](within-host-pi.ipynb)
   * [*Hw - Hs* relationship](hw-hs.ipynb)
   * [Using $F_{WS}$ to estimate the rate of superinfection $\chi$](fws-compare-methods.ipynb)
1. [Epidemiological scenarios](epidemiological-scenarios.md)
   * [Analysing a time series](time-series.ipynb)
   * [Transient scenarios](transient-scenarios.ipynb)
   * [Local outbreak](local-outbreak.ipynb)