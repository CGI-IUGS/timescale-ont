# Geologic Timescale model
Markdown documentation created by [pyLODE](http://github.com/rdflib/pyLODE)


## Metadata
* **IRI**
  * `http://resource.geosciml.org/ontology/timescale/gts`
* **Creators(s)**
  * <a href='https://orcid.org/0000-0002-3884-3420'>Simon Jonathan David COX, CSIRO Australia</a>
* **Contributor(s)**
  * <a href='https://orcid.org/0000-0001-6041-5302'>Stephen M RICHARD</a>
* **Created**
  * 2011-01-01
* **Modified**
  * 2017-04-28
* **Imports**
  * <a href="http://resource.geosciml.org/ontology/timescale/thors">http://resource.geosciml.org/ontology/timescale/thors</a>
* **License &amp; Rights**
  * <a href="http://creativecommons.org/licenses/by/4.0/">http://creativecommons.org/licenses/by/4.0/</a>
  * &copy; © 2012-2017 CSIRO
* **Ontology Source**
  * <a href="./rdf/gts.ttl">RDF (turtle)</a>
* **Code Repository**
  * <https://github.com/CGI-IUGS/timescale-ont>
### Description
<p>This is an RDF/OWL representation of the GeoSciML Geologic Timescale model, which has been adapted from the model described in <a href='https://doi.org/10.1130/GES00022.1
'>Cox, S.J.D, &amp; Richard, S.M. (2005) A formal model for the geologic timescale and GSSP, compatible with geospatial information transfer standards, Geosphere, Geological Society of America 1/3, 119–137</a>.</p>
<p>This ontology (GTS) imports and specializes a generic ontology for Temporal Hierarchical Ordinal Reference System (THORS). </p>
<p>It is recommended that the W3C OWL-Time ontology is used to encode details of temporal positions, and also to record temporal relationships between eras/intervals.</p>

## Table of Contents
1. [Classes](#classes)
1. [Object Properties](#objectproperties)
1. [Datatype Properties](#datatypeproperties)
1. [Namespaces](#namespaces)  


## Overview
![GTS main classes](./images/gts+thors.png)
**Figure 1:** Ontology overview  
## Classes
[Age](#Age),
[Eon](#Eon),
[Epoch](#Epoch),
[Era](#Era),
[Geochronologic Boundary](#GeochronologicBoundary),
[Geochronologic Era](#GeochronologicEra),
[Geochronologic Era Rank](#GeochronologicEraRank),
[Geologic Timescale](#GeologicTimescale),
[Numeric Era Boundary](#NumericEraBoundary),
[Period](#Period),
[Stratigraphic Event](#StratigraphicEvent),
[Stratigraphic Point](#StratigraphicPoint),
[Stratigraphic Section](#StratigraphicSection),
[Sub-Period](#Sub-Period),
[Super-Eon](#Super-Eon),
### Age <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Age`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Eon <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Eon`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Epoch <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Epoch`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Era <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Era`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Geochronologic Boundary <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#GeochronologicBoundary`
Super-classes |<a href="http://resource.geosciml.org/ontology/timescale/thors#EraBoundary">thors:EraBoundary</a><sup class="sup-c" title="class">c</sup><br />
Restrictions |<a href="#stratotype">gts:stratotype</a><sup class="sup-op" title="object property">op</sup> <span class="cardinality">only</span> <a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup><br />
In range of |<a href="#geochronologicboundary">gts:boundary</a><sup class="sup-op" title="object property">op</sup><br />
### Geochronologic Era <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#GeochronologicEra`
Super-classes |<a href="http://resource.geosciml.org/ontology/timescale/thors#Era">thors:Era</a><sup class="sup-c" title="class">c</sup><br />
Restrictions |<a href="http://www.w3.org/2004/02/skos/core#notation">skos:notation</a> <span class="cardinality">some</span> <a href="http://resource.geosciml.org/ontology/timescale/gts#EraCode">gts:EraCode</a><sup class="sup-c" title="class">c</sup><br /><a href="#stratotype">gts:stratotype</a><sup class="sup-op" title="object property">op</sup> <span class="cardinality">only</span> <a href="#StratigraphicSection">gts:StratigraphicSection</a><sup class="sup-c" title="class">c</sup><br />
Sub-classes |<a href="#Age">gts:Age</a><sup class="sup-c" title="class">c</sup><br /><a href="#Era">gts:Era</a><sup class="sup-c" title="class">c</sup><br /><a href="#Epoch">gts:Epoch</a><sup class="sup-c" title="class">c</sup><br /><a href="#Period">gts:Period</a><sup class="sup-c" title="class">c</sup><br /><a href="#Super-Eon">gts:Super-Eon</a><sup class="sup-c" title="class">c</sup><br /><a href="#Sub-Period">gts:Sub-Period</a><sup class="sup-c" title="class">c</sup><br /><a href="#Eon">gts:Eon</a><sup class="sup-c" title="class">c</sup><br />
In domain of |<a href="#Geochronologicerarank">gts:rank</a><sup class="sup-op" title="object property">op</sup><br />
In range of |<a href="#geochronologicera">gts:era</a><sup class="sup-op" title="object property">op</sup><br />
### Geochronologic Era Rank <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#GeochronologicEraRank`
Super-classes |<a href="http://www.w3.org/2004/02/skos/core#Concept">skos:Concept</a><sup class="sup-c" title="class">c</sup><br />
In range of |<a href="#Geochronologicerarank">gts:rank</a><sup class="sup-op" title="object property">op</sup><br />
### Geologic Timescale <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#GeologicTimescale`
Super-classes |<a href="http://resource.geosciml.org/ontology/timescale/thors#ReferenceSystem">thors:ReferenceSystem</a><sup class="sup-c" title="class">c</sup><br />
Restrictions |<a href="http://resource.geosciml.org/ontology/timescale/thors#referencePoint">thors:referencePoint</a> <span class="cardinality">only</span> (<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#NumericEraBoundary">gts:NumericEraBoundary</a><sup class="sup-c" title="class">c</sup>)<br /><a href="http://resource.geosciml.org/ontology/timescale/thors#component">thors:component</a> <span class="cardinality">only</span> <a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Numeric Era Boundary <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#NumericEraBoundary`
Super-classes |<a href="http://resource.geosciml.org/ontology/timescale/thors#EraBoundary">thors:EraBoundary</a><sup class="sup-c" title="class">c</sup><br />
Restrictions |<a href="#status">gts:status</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">exactly</span> 1<br />
### Period <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Period`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Stratigraphic Event <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#StratigraphicEvent`
Description | A subclass of Geologic Event (placeholder) 
In range of |<a href="#stratigraphicevent">gts:event</a><sup class="sup-op" title="object property">op</sup><br />
### Stratigraphic Point <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#StratigraphicPoint`
Restrictions |<a href="#correlationevent">gts:correlationEvent</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">exactly</span> 1<br /><a href="#ratified">gts:ratifiedGSSP</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">max</span> 1<br /><a href="#status">gts:status</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">exactly</span> 1<br />
In domain of |<a href="#correlationevent">gts:correlationEvent</a><sup class="sup-dp" title="datatype property">dp</sup><br /><a href="#geochronologicboundary">gts:boundary</a><sup class="sup-op" title="object property">op</sup><br /><a href="#boundarylevel">gts:boundaryLevel</a><sup class="sup-dp" title="datatype property">dp</sup><br />
### Stratigraphic Section <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#StratigraphicSection`
Restrictions |<a href="#geologicdescription">gts:geologicDescription</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">exactly</span> 1<br /><a href="#geologicsetting">gts:geologicSetting</a><sup class="sup-dp" title="datatype property">dp</sup> <span class="cardinality">exactly</span> 1<br />
In domain of |<a href="#geologicdescription">gts:geologicDescription</a><sup class="sup-dp" title="datatype property">dp</sup><br /><a href="#geologicsetting">gts:geologicSetting</a><sup class="sup-dp" title="datatype property">dp</sup><br /><a href="#geochronologicera">gts:era</a><sup class="sup-op" title="object property">op</sup><br />
### Sub-Period <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Sub-Period`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
### Super-Eon <sup>c</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#Super-Eon`
Super-classes |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />

## Object Properties
[geochronologic boundary](geochronologicboundary),
[correlating boundary or era](correlatingboundaryorera),
[geochronologic era](geochronologicera),
[stratigraphic event](stratigraphicevent),
[geologic manifestation](geologicmanifestation),
[Uncertainty in time position](Uncertaintyintimeposition),
[Geochronologic era rank](Geochronologicerarank),
[stratotype](stratotype),
[](geochronologicboundary)
### geochronologic boundary <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#boundary`
Description | geochronologic boundary corresponding with this point
Domain(s) |<a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup><br />
Range(s) |<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup><br />
[](correlatingboundaryorera)
### correlating boundary or era <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#correlatesWith`
Description | This property points from a geologic feature or event to a geochronologic element
Range(s) |<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup><br /><a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
[](geochronologicera)
### geochronologic era <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#era`
Description | geochronologic era corresponding with this section
Domain(s) |<a href="#StratigraphicSection">gts:StratigraphicSection</a><sup class="sup-c" title="class">c</sup><br />
Range(s) |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
[](stratigraphicevent)
### stratigraphic event <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#event`
Description | stratigraphic event corresponding with this boundary or point
Domain(s) |(<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup>)<br />
Range(s) |<a href="#StratigraphicEvent">gts:StratigraphicEvent</a><sup class="sup-c" title="class">c</sup><br />
[](geologicmanifestation)
### geologic manifestation <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#manifestedBy`
Description | This property points from a geochronologic element to a geologic feature
Domain(s) |(<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup>)<br />
[](Uncertaintyintimeposition)
### Uncertainty in time position <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#positionalUncertainty`
[](Geochronologicerarank)
### Geochronologic era rank <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#rank`
Description | Elements of all ranks are included in the class 'gts:GeochronologicEra'. 
The rank may be indicated by membership of a sub-class, or is indicated using the 'gts:rank' property.
Domain(s) |<a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup><br />
Range(s) |<a href="#GeochronologicEraRank">gts:GeochronologicEraRank</a><sup class="sup-c" title="class">c</sup><br />
[](stratotype)
### stratotype <sup>op</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#stratotype`
Description | the characteristic point or section corresponding with a geochronologic concept
Domain(s) |(<a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#GeochronologicEra">gts:GeochronologicEra</a><sup class="sup-c" title="class">c</sup>)<br />
Range(s) |<a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup><br /><a href="#StratigraphicSection">gts:StratigraphicSection</a><sup class="sup-c" title="class">c</sup><br />

## Datatype Properties
[boundary level](boundarylevel),
[correlation event](correlationevent),
[geologic description](geologicdescription),
[geologic setting](geologicsetting),
[ratified](ratified),
[status](status),
[](boundarylevel)
### boundary level <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#boundaryLevel`
Description | the level within the section of the point characterizing the boundary
Domain(s) |<a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup><br />
[](correlationevent)
### correlation event <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#correlationEvent`
Description | the stratigraphic event that is intended to be represented by this stratigraphic point
Domain(s) |<a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup><br />
[](geologicdescription)
### geologic description <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#geologicDescription`
Domain(s) |<a href="#StratigraphicSection">gts:StratigraphicSection</a><sup class="sup-c" title="class">c</sup><br />
[](geologicsetting)
### geologic setting <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#geologicSetting`
Domain(s) |<a href="#StratigraphicSection">gts:StratigraphicSection</a><sup class="sup-c" title="class">c</sup><br />
[](ratified)
### ratified <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#ratifiedGSSP`
Description | 'true' if ratified by ICS
Domain(s) |(<a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup> or <a href="#GeochronologicBoundary">gts:GeochronologicBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#NumericEraBoundary">gts:NumericEraBoundary</a><sup class="sup-c" title="class">c</sup>)<br />
Range(s) |<a href="http://www.w3.org/2001/XMLSchema#boolean">xsd:boolean</a><sup class="sup-c" title="class">c</sup><br />
[](status)
### status <sup>dp</sup>
Property | Value
--- | ---
IRI | `http://resource.geosciml.org/ontology/timescale/gts#status`
Description | formal ICS status of this boundary and point
Domain(s) |(<a href="#NumericEraBoundary">gts:NumericEraBoundary</a><sup class="sup-c" title="class">c</sup> or <a href="#StratigraphicPoint">gts:StratigraphicPoint</a><sup class="sup-c" title="class">c</sup>)<br />

## Namespaces
* **default (:)**
  * `http://resource.geosciml.org/ontology/timescale/gts#`
* **dc**
  * `http://purl.org/dc/elements/1.1/`
* **dcterms**
  * `http://purl.org/dc/terms/`
* **doap**
  * `http://usefulinc.com/ns/doap#`
* **gts**
  * `http://resource.geosciml.org/ontology/timescale/gts#`
* **owl**
  * `http://www.w3.org/2002/07/owl#`
* **prov**
  * `http://www.w3.org/ns/prov#`
* **rank**
  * `http://resource.geosciml.org/ontology/timescale/rank/`
* **rdf**
  * `http://www.w3.org/1999/02/22-rdf-syntax-ns#`
* **rdfs**
  * `http://www.w3.org/2000/01/rdf-schema#`
* **skos**
  * `http://www.w3.org/2004/02/skos/core#`
* **thors**
  * `http://resource.geosciml.org/ontology/timescale/thors#`
* **vann**
  * `http://purl.org/vocab/vann/`
* **voaf**
  * `http://purl.org/vocommons/voaf#`
* **xml**
  * `http://www.w3.org/XML/1998/namespace`
* **xsd**
  * `http://www.w3.org/2001/XMLSchema#`

## Legend
* Classes: c
* Object Properties :op
* Functional Properties: fp
* Data Properties: dp
* Annotation Properties: dp
* Properties: p
* Named Individuals: ni