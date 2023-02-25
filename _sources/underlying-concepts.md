# Underlying concepts

The genetic structure of a parasite population is shaped by its transmission dynamics but superinfection and recombination make this relationship complex and hard to analyse.  Superinfection means that a host acquires infection from multiple independent sources, and therefore carries a mixture of parasite genotypes with different ancestral histories, which may then be cotransmitted to other hosts.  Recombination within genetically mixed infections causes different regions of the genome to have different genealogies, as shown in the figure below, and this presents an extremely complex problem for genetic inference of parasite transmission dynamics.

![superinfection](superinfection.png).
[See figure caption](superinfection.md)

The **genomic transmission graph** aims to simplify the problem.  It is a directed acyclic graph in which the nodes represent hosts and edges represent vectors, as illustrated below. The graph is plotted on an axis of time and we make the simplifying assumption that a host exists at a discrete point in time. 

![transmission-graph](transmission-graph.png)
[See figure caption](transmission-graph.md)

If we pick any node and trace a path forward in time along the edges to some other node, that is a *transmission chain*. Transmission chains can *branch* when a host is the source of parasites for multiple other hosts.  Transmission chains can also *cross* when a host acquires parasites from multiple sources, i.e when there is superinfection.

Parasites reproduce as they flow along transmission chains, and parasites that are flowing along the same transmission chain can genetically recombine with each other.

We define a *lineage* as a path through the transmission graph that we define by taking an allele at a point locus and tracing its ancestry back in time through the generations ([see glossary](glossary.md)). 

An individual parasite could have many different lineages each following a unique path through the graph because whenever transmission chains cross, the paths of different lineages can diverge.

These simple concepts suggest a logical framework for thinking about how genetic variation is related to transmission dynamics in a recombining parasite population.  Instead of attempting to construct a phylogenetic tree, we imagine a genomic transmission graph onto which we can map the lineages of different loci in the genome. This allows for superinfection and recombination because lineages at different loci can take different pathways through the graph.  

The challenge is then to define the essential parameters of the graph and to understand how they are related to genetic variation.  To understand the scientific concepts it is a good idea to work through the sections in this order:

1. [The basic model](basic-model.md)
1. [Time to coalescence](coalescence-time-basic.ipynb)
1. [Nucleotide diversity](nucleotide-diversity.ipynb)
1. [Haplotype homozygosity](haplotype-homozygosity-2cM.ipynb)
1. [Effect of migration](migration-simple.ipynb)
1. [Rate of superinfection](fws-compare-methods.ipynb)