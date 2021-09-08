## Introduction
{:#introduction}

<!-- Context      -->
The establishment of an interoperable
European railway area without frontiers,
while guaranteeing railway operation safety,
is the prime objective of the European Union Agency for Railways (ERA) [](cite:cites eu-796-2016).
Since 2019 [ERA became the European authority](https://www.era.europa.eu/content/era-becomes-european-authority-cross-border-rail-traffic-europe_en)[^eu-authority] for cross-border rail traffic in Europe,
mandated under the European Union (EU) law,
to devise the technical and legal framework for supporting harmonised
and safe cross-border railway operations.

<!-- What is the problem?      -->
The European railway ecosystem
presents a particularly challenging scenario for interoperability,
not only regarding physical aspects (e.g., infrastructure, energy systems, etc.) but also digital ones (e.g., information).
Multiple organisations, such as Infrastructure Managers[^im] (IMs)
and Railway Undertakings[^ru] (RUs) [](cite:cites eu-34-2012),
need to interact and exchange information to ensure safe cross-border railway operations.
These organisations rely on different information management systems
from multiple vendors, that are often incompatible with each other.
To increase digital interoperability
among heterogeneous data and information systems,
ERA supports and maintains a set of [base registries](https://www.era.europa.eu/registers_en)[^base-registry],
in the form of relational databases,
where organisations input and access
the different aspects of the information they manage and require.

However, following such traditional application-centric approach
lead to isolated digital environments
that consequently add barriers to digital interoperability.
Tightly coupling base registries to the applications that operate over them,
triggered the proliferation of often overlapping
and difficult to manage data models hidden inside application code,
which also increased the cost of maintenance and innovation.
Moreover, stakeholder organisations such as IMs,
are required to report the same information multiple times for different registries,
increasing the probability of data inconsistency issues,
while adding more costs to IMs due to duplicated efforts.

<!-- What is my solution?      -->
To address these issues,
we propose a digital interoperability strategy for ERA,
that adheres to the [Linked Data principles](https://www.w3.org/DesignIssues/LinkedData.html)[^ld-principles] [](cite:cites heath2011)
and relies on standard Semantic Web [](cite:cites bernerslee2001) technologies.
We built the foundations to establish a _semantic layer_ for data integration within the agency,
initially spanning three different [base registries](https://www.era.europa.eu/registers_en)[^era-registries]:,
Register of Infrastructure (RINF),
Register of Authorized Types of Vehicles (ERATV)
and the Centralized Virtual Vehicle Register (ECVVR).
We validate the usefulness of the approach
by reusing the produced semantic data to support route compatibility checks (RCC),
a highly-demanded use case in the railway domain.
The RCC use case is stipulated and specified in EU regulations 2016/797 and 2019/773 [](cite:cites eu-797-2016, eu-773-2019)
and was so far, unsupported by ERA
due to interoperability issues among base registries.
Additionally, we show the flexibility of graph-based data models,
by integrating an additional external data source
that complement the resulting Knowledge Graph.

The contributions of this paper include
(i) an [official ontology](http://era.ilabt.imec.be/era-vocabulary/index-en.html)[^era-ontology], modelling railway infrastructure aspects (e.g. topological, functional, etc.), rolling stock and authorized vehicle types, and 28 independently managed reference datasets;
(ii) a public and reusable [RDF Knowledge Graph](http://era.ilabt.imec.be/)[^era-kg] with 13.8 million triples about the European railway infrastructure and more than 800 thousand rolling stocks;
(iii) a cost-efficient system architecture that enables high-flexibility for use case support; and
(iv) an open source and [RDF native Web application](http://era.ilabt.imec.be/test/compatibility-check-demo/)[^era-ui] to support and process RCC queries.

<!-- What comes after my solution?      -->

This work demonstrates how data-centric system design,
powered by Semantic Web technologies,
provides a framework to achieve data interoperability
and unlock new and innovative use cases and applications.
The results of the work presented in this paper
had a [strong impact on ERA](https://www.era.europa.eu/sites/default/files/agency/docs/decision/decision_n250_annex1_linked_data_en.pdf)[^era-decision],
which decided on making Semantic Web technologies
the default setting for any future development of data,
registers and specifications, under the agency's remit,
for data exchange mandated by the EU legal framework.
The next steps, which are already underway,
include further extending the ontology
to consider additional aspects,
aligned with the requirements of the railway domain
and evolving the system architecture
towards a production-ready solution,
fully integrated with the data management workflows of ERA.

<!-- Outline of the paper      -->
The remainder of this paper is organized as follows.
Section 2 presents an overview of related work in the context
of modelling approaches and interoperability for the railway domain.
Section 3, describes the RCC use case its requirements.
Section 4 gives an overview and description
of our proposed solution architecture components.
Section 5 discusses the advantages and limitations of the approach,
and Section 6 presents our conclusions and perspectives for future work.

[^eu-authority]: ERA becomes European authority for cross-border rail traffic in Europe: <a href="https://www.era.europa.eu/content/era-becomes-european-authority-cross-border-rail-traffic-europe_en" target="_blank">https://www.era.europa.eu/content/era-becomes-european-authority-cross-border-rail-traffic-europe_en</a>

[^im]: An Infrastructure Manager is defined as any body or firm responsible in particular for establishing, managing and maintaining railway infrastructure, including traffic management, control-command and signalling.

[^ru]: A Railway Undertaking is defined as any public or private licensed undertaking, the principal business of which is to provide services for the transport of goods and/or passengers by rail with a requirement that the undertaking ensure traction.

[^base-registry]: _"A base registry is  a  trusted  and  authoritative  source  of  information  which  can  and  should be digitally reused by others, where one organisation is responsible and accountable  for  the  collection,  use,  updating  and  preservation  of  information."_ [](cite:cites eu-iop)

[^ld-principles]: Principles of Linked Data: <a href="https://www.w3.org/DesignIssues/LinkedData.html">https://www.w3.org/DesignIssues/LinkedData.html</a>

[^era-registries]: Base registries of ERA: <a href="https://www.era.europa.eu/registers_en">https://www.era.europa.eu/registers_en</a>

[^era-ontology]: <a href="http://era.ilabt.imec.be/era-vocabulary/index-en.html">http://era.ilabt.imec.be/era-vocabulary/index-en.html</a>

[^era-kg]: <a href="http://era.ilabt.imec.be/">http://era.ilabt.imec.be/</a>
 
[^era-ui]: <a href="http://era.ilabt.imec.be/test/compatibility-check-demo/">http://era.ilabt.imec.be/test/compatibility-check-demo/</a>

[^era-decision]: ERA's roadmap for Linked Data mainstreaming: <a href="https://www.era.europa.eu/sites/default/files/agency/docs/decision/decision_n250_annex1_linked_data_en.pdf">https://www.era.europa.eu/sites/default/files/agency/docs/decision/decision_n250_annex1_linked_data_en.pdf</a>
