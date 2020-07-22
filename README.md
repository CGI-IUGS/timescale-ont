# Geologic Timescale Ontology
This repository holds an OWL ontology for the RDF representation of the Geologic Timescale. 

The ontology is packaged in two primary graphs: 

* [Temporal Hierarchical Ordinal Reference System ontology THORS](./rdf/thors.ttl)
  * [documentation](https://raw.githack.com/CGI-IUGS/timescale-ont/master/html/thors.html)
* [Geologic TimeScale ontology](./gts.ttl)
  * [documentation](https://raw.githack.com/CGI-IUGS/timescale-ont/master/html/gts.html)

The structure is based on the model described in UML in [Cox & Richard 2005 _A formal model for the geologic time scale and global stratotype section and point, compatible with geospatial information transfer standards_](https://doi.org/10.1130/GES00022.1), and updated in RDF/OWL in [Cox & Richard 2015 _A geologic timescale ontology and service_](http://link.springer.com/article/10.1007/s12145-014-0170-6). Those models used the Temporal Reference System model from [ISO 19108](https://www.iso.org/standard/26013.html) at the core. The current THORS ontology has been disentangled from the ISO model so the ontology file thors.ttl has no remaining dependencies on any non-standard RDF graphs, and gts.ttl only imports the clean thors.ttl 

An alignment with the ISO 19100 models is now provided through 
[thors/iso.ttl](./rdf/thors/iso.ttl) and [gts/iso.ttl](./rdf/gts/iso.ttl)

Datasets (timescales) that use this ontology are in https://github.com/CGI-IUGS/timescale-data. 

**NOTE:** this repository is a subtree forked from https://github.com/GeoscienceAustralia/geosciml.org/tree/master/resource/static/ontology/timescale
