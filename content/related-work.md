## Related Work
{:#related-work}

In this section, we present different (semantic) data models
to describe the railway domain focusing on different aspects of the domain
and motivated by different use cases.
Also existing related work
applying semantic technologies in the railway domain.
We studied these models,
aiming on reusing as much as possible
their embedded domain-specific knowledge (e.g. definitions, categorizations, naming conventions, etc.),
during the creation of ERA's ontology.

Multiple domain data models were proposed (some still under active development),
to bridge the interoperability challenges
by uniformly describing the different technical aspects related to the railway domain.
However, most lack semantic definitions
that promote/guarantee the use of persistent identifiers across data sources,
hindering interoperability when exchanging data across organizations.
Available models range from company-specific
to industrial consortium-driven standardization efforts.
For example, the _Informatie Model Spoor_ ([IMSpoorXML](https://confluence.rigd-loxia.nl/display/IMSP/IMSpoor+Publicatie+Home)[^imspoor]),
developed by the Dutch IM ProRail,
provides an XML Schema-based model with integrated
functional and geographic information about the railway infrastructure.
IMSpoorXML is currently used within ProRail
and is under active maintenance and development.
The International Railway Standard IRS:30100 [RailTopoModel](http://www.railtopomodel.org/en/download/irs30100-apr16-7594BCA1524E14224D0.html?file=files/download/RailTopoModel/180416_uic_irs30100.pdf)[^rtm][](cite:cites irs30100)
was developed under the patronage of the International Union of Railways (UIC)
and provides a systemic UML-based model
for describing the topological aspects of railway infrastructure.
It relies on the _connexity graph_ mathematical concept [](cite:cites gely2010)
to describe the interconnection of the different railway network elements.
Implementations of RailTopoModel include
[RailML](https://wiki3.railml.org/wiki/Main_Page)[^railml] [](cite:cites hlubucek2017)
and the [EULYNX](https://dataprep.eulynx.eu/2020-10/index.htm)[^eulynx] initiative,
both currently developed by industrial consortiums.

The use of semantic technologies,
for modelling the railway domain is not new.
In 2011, the results of the EU project InteGRail,
included an ontology integrating the major railway sub-systems,
to achieve higher levels of performance in terms of capacity,
average speed and punctuality, safety and the optimised usage of resources
in railway systems [](cite:cites verstichel2011).
Smart Rail is another EU project that applied semantic technologies
for modelling more organizational aspects of the railway domain.
It produced an [ontology](https://ontology.tno.nl/smart-rail/)[^smart-rail],
focused on modelling stakeholders and physical resources of the railway infrastructure.
RaCoOn (Rail Core Ontologies) is a set of domain ontologies
that model areas of the rail domain commonly used in railway data exchange [](cite:cites tutcher2017).
An study of how Linked Data was applied
in the British railway domain,
highlights the reduction of costs
as a consequence of more efficient data flows,
and hints towards the need for increasing adoption from industry [](cite:cites morris2014).
More recently, Bischof et al. [](cite:cites bischof2020) outlined
the requirements and challenges to define an open
standard ontology for railway topologies based on existing standards.
None of these approaches evolved beyond academic exercises
and the produced ontologies are currently unmaintained or no longer available.
In contrast, one of the main goals of ERA,
as an European authority for the domain,
is to provide a fully supported and open reference ontology
not only for internal data management operations
but targeting also its adoption and extension
by the stakeholders of the railway domain,
as an asset that supports their own use cases.

[^imspoor]: <a href="https://confluence.rigd-loxia.nl/display/IMSP/IMSpoor+Publicatie+Home">https://confluence.rigd-loxia.nl/display/IMSP/IMSpoor+Publicatie+Home</a>

[^rtm]: RailTopoModel specification<a href="http://www.railtopomodel.org/en/download/irs30100-apr16-7594BCA1524E14224D0.html?file=files/download/RailTopoModel/180416_uic_irs30100.pdf">http://www.railtopomodel.org/en/download/irs30100-apr16-7594BCA1524E14224D0.html?file=files/download/RailTopoModel/180416_uic_irs30100.pdf</a>

[^railml]: <a href="https://wiki3.railml.org/wiki/Main_Page">https://wiki3.railml.org/wiki/Main_Page</a>

[^eulynx]: <a href="https://dataprep.eulynx.eu/2020-10/index.htm">https://dataprep.eulynx.eu/2020-10/index.htm</a>

[^smart-rail]: Smart Rail ontology: <a href="https://ontology.tno.nl/smart-rail/">https://ontology.tno.nl/smart-rail/</a>