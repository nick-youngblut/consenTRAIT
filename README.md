# consenTRAIT
Phylogenetic conservatism of functional traits in microorganisms

The concsnTRAIT algorithm from [Martiny et al., (2013)](http://www.nature.com/ismej/journal/v7/n4/full/ismej2012160a.html) but made executable from the command line, and the bootstrapping can be conducted in parallel. 

See the [Martiny Lab website](http://www.ess.uci.edu/group/amartiny/research/consentrait) for more information



# INSTALL

Just make sure the R package dependencies are installed:  data.table, adephylo, ape, docopt, parallel


# Example

Making example files with 100 taxa and 2 traits: the 1st trait is conserved and the 2nd is not. 

`Rscript consenTRAIT.r -x 100 TEST TEST TEST`

Running consenTRAIT with bootstrapping in parallel (4 cores)

`Rscript  consenTRAIT.r -p 4 consentrait_TEST.nwk t1 consentrait_TEST.txt` 

