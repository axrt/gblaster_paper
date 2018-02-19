# Algorithmic detection of lateral gene transfer using regression analysis
## (Supplementary Materials)

This page supplies additional research materials that an interested reader may
use to reproduce/extend the results.

The 'gBLASTer' workflow pipeline consists of three components:

- [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) + [DerbyDB](https://db.apache.org/derby/) backend that is responsible for coordinating [gpuBLASTP](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3018811/)
  and storing the results in an SQL database for further retrieval;
  a corresponding repository can be found here: [gBLASTer](https://github.com/axrt/gBLASTer.git)
- R-package (gbra) that contains common helper functions use in this study;
  a corresponding repository can be found here: [gbra](https://github.com/axrt/gbra)
- Custom R scripts, available as Rmarkdown files to facilitate reproduction;
  a corresponding repository can be found here: [gBLASTer repo](https://github.com/axrt/gBLASTer_research/tree/master/stat/67.genomes.quadruple.model)

Due to an exceedingly large volume on the raw data (SQL database, over 0.5TB),
we do not have an opportunity to make it available online, but will gladly
share the data upon request.

The "combed" input data can be found as follows:

- A genome legend that maps genome names to their database IDs: [legend](https://raw.githubusercontent.com/axrt/gBLASTer_research/master/stat/master/legend.txt) (please note, that some of the genomes were excluded, see the [processing script](https://github.com/axrt/gBLASTer_research/blob/master/stat/bootstrapped.models.Rmd)
- A [raw bit-score matrix](https://github.com/axrt/gBLASTer_research/blob/master/stat/67.genomes/bh.data.raw.rda)
- A [filtered bit-score matrix](https://github.com/axrt/gBLASTer_research/blob/master/stat/67.genomes/bh.data.normal.rda)
- A block of Rmd code that was used to operate on the matrix above to obtain
  the results and produce output graphics:
- A Perl script used to perform the domain search in PFAM[]:
- A Perl script used to perform statistics on the domain distribution:

Computer systems used in this study: [layout of from the system]

## Supplementary Diagrams and Tables
