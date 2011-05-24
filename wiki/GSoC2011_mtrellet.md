---
title: GSoC2011 mtrellet
permalink: wiki/GSoC2011_mtrellet
layout: wiki
---

Author & Mentors
----------------

[Mikael Trellet](User%3AMtrellet "wikilink") mikael.trellet@gmail.com

**Mentors**

  
Joao Rodrigues

Eric Talevich

Abstract
--------

Analysis of protein-protein complexes interfaces at a residue level
yields significant information on the overall binding process. Such
information can be broadly used for example in binding affinity studies,
interface design, and enzymology. To tap into it, there is a need for
tools that systematically and automatically analyze protein structures,
or that provide means to this end. Protorop
(http://www.bioinformatics.sussex.ac.uk/protorp/) is an example of such
a tool and the elevated number of citations the server has had since its
publication acknowledge its importance. However, being a webserver,
Protorop is not suited for large-scale analysis and it leaves the
community dependent on its maintainers to keep the service available. On
the other hand, Biopython’s structural biology module, Bio.PDB, provides
the ideal parsing machinery and programmatic structures for the
development of an offline, open-source library for interface analysis.
Such a library could be easily used in large-scale analysis of
protein-protein interfaces, for example in the CAPRI experiment
evaluation or in benchmark statistics. It would be also reasonable, if
time permits, to extend this module to deal with protein-DNA or
protein-RNA complexes, as Biopython supports nucleic acids already.

Project Schedule
----------------

### Week 1 \[23rd May - 31st June\]

#### Add the new module backbone in current Bio.PDB code base

-   Evaluate possible code reuse and call it into the new module
-   Try simple calculations to be sure that there is stability between
    the different modules (parsing for example) and functions

#### Define a stable benchmark

-   Select few PDB files among interface size and proteins size would be
    different
-   Add some basics unit tests

### Weeks 2-3 \[1st - 13th June\]

#### Extend IUPAC.Data module with residue information

-   Deduce residues weight from Atom instead of direct dictionnary
    storage
-   -   [pKa values
        algorithm](http://www3.interscience.wiley.com/journal/112117957/abstract)
