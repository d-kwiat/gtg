# Epidemiological scenarios

We can use `coalestr` to model how different epidemiological scenarios affect parasite genetic diversity and within-host variation.  For example, we can explore:

* how population genetic diversity and within-host variation are affected by changes in $N_h$, $Q$, $\chi$ and $N_m$
* how transmission parameters interact in their genetic effects
* how different epidemiological scenarios can lead to the same genetic effects
* the time it takes for changes in transmission parameters to be reflected in genetic changes

In modelling epidemiological scenarios we are typically interested in events that are relatively **local** and **recent**, e.g. what is happening in a particular district of a malaria-endemic country at the present time, as opposed to events that have occurred in the global parasite population over the past thousand years.

The problem is that local genetic diversity is greatly affected by migration from surrounding regions and global parasite dispersal.  Typical mean coalescence times in a local parasite subpopulation (based on measurements of nucleotide diversity) are around 4000-5000 years, so we cannot ignore the history of the global parasite metapopulation when we are analysing the current levels of genetic diversity in a local parasite population. 

Thus before we can model a recent epidemiological scenario we need to construct the history of the global parasite metapopulation. The function `coalestr.species` builds a toy model based loosely on *Plasmodium falciparum*, with a small founder population emerging approximately 50,000 years ago and an exponential population expansion approximately 10,000-20,000 years ago.  

, based on measurements of nucleotide diversity in malaria endemic region typ, levels of nucleotide diversity imply a coalescence time of  . That is, if  The problem is that levels of genetic diversity in a local subare strongly affected by events However we have to address the following problem.   is that However we know that the  , occuring on a timescale of a few years rather than centuries.  (i.e. affecting a relatively small subpopulation within the global metapopulation) and **recent** ( cal population.  between-host diversity, and understanding how the same genetic changes   transient rise in the crossing rate of transmission chains like Before we model an epidemiological scenario, we must establish the underlying genetic diversity of 

- [Species history](species_history.ipynb)
- [Scenarios #1](scenario_1.ipynb)
- [Local outbreak](local_outbreak.ipynb)
