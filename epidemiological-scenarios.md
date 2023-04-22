# Epidemiological scenarios

We can use `coalestr` to model how different epidemiological scenarios affect parasite genetic diversity and within-host variation.  For example, we can explore:

* how population genetic diversity and within-host variation are affected by changes in $N_h$, $Q$, $\chi$ and $N_m$
* how transmission parameters interact in their genetic effects
* how different epidemiological scenarios can lead to the same genetic effects
* the time it takes for changes in transmission parameters to be reflected in genetic changes

In modelling epidemiological scenarios we are typically interested in events that are relatively **local** and **recent**, e.g. what is happening in a particular district of a malaria-endemic country at the present time, as opposed to events that have occurred in the global parasite population over the past thousand years.

The problem is that local genetic diversity is greatly affected by migration from surrounding regions and global parasite dispersal.  Typical mean coalescence times in a local parasite subpopulation (based on measurements of nucleotide diversity) are around 4000-5000 years, so we cannot ignore the history of the global parasite metapopulation when we are analysing the current levels of genetic diversity in a local parasite population. 

Thus before we can model a recent epidemiological scenario we need to consider the history of the global parasite metapopulation. The function `coalestr.species` builds a toy model based loosely what is known about the emergence of *Plasmodium falciparum*, with a small founder population undergoing an exponential population expansion approximately 10,000 years ago.  

- [Modelling the global parasite metapopulation](global-metapopulation.ipynb)
- [Modelling transient changes in transmission parameters](scenario_1.ipynb)
- [Modelling a local outbreak in a near-elimination setting](local_outbreak.ipynb)
