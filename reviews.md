# Reviewer 1

SCORE: 2 (accept)

----- TEXT:

This looks like a dream use case for semantic technologies, where you have different distributed datasets that need an interoperability layer to provide uniform access regardless of their individual silos.



The work described in the paper looks solid from an engineering point of view, although the online demonstrator (http://era.ilabt.imec.be/test/compatibility-check-demo/) can still be improved in terms of responsiveness and ease of use in order to be ready for production. Reproducibility also seems to be properly taken care of, with code and data publicly available. This could encourage the development of applications by third parties, although for the time being my impression is that the technological entry barrier is still too high for generalized adoption.



The official commitment of ERA to adopt semantic technologies for future deployments is an important step in the direction of actual deployment as a production system. In the past, we have seen many brilliant use cases of semantic technologies in key sectors that nevertheless ended up failing when this crucial step needed to be taken. Hopefully, ERA will still remain committed at that point.



# Reviewer 2

SCORE: 2 (accept)

----- TEXT:

This paper describes an application of semantic web technologies in the railway domain at the european scale: for the European Union Agency for Railways.



The approach provides a data interoperability layer for a set of heterogeneous data sources, using RML, an ontology developed for the domain, and a set of SKOS terminologies partially automatically generated using RML, exposes data using Linked Data Fragments for geospatial data, and provide a web application with shortest path detection algorithms including ad-hoc rules to check the compability between a specific vehicle and the tracks it can use. This cocktail of semantic web technologies



There is no evidence that the ERA or other stakeholders already adopted this specific solution. However, the solution had an impact at the European scale, as the European Railway Agency officially decided to make Semantic Web and Linked Data-based approaches the default setting for any future development in the data and data-exchang domain under their mandate by EU legal framework. The approach is pretty generic and many other application domains could benefit from this work.



The paper is very well written, each part of the approach is clearly motivated and described and there are pointers to online resources and demonstrations for the approach.



I definetly recommend this paper for the ISWC In-Use track. However, there are a few minor issues in the paper and the online resources, that could be corrected before the conference:



Paper:

- please check acronyms are all defined

- data source that complement -> complements

- the RCC use case its requirements -> check

- Table 1 "Connected" column seems not correct wrt Figure 1

- a certain route, is -> it is



Online:

- from the page[ http://era.ilabt.imec.be/era-vocabulary/](http://era.ilabt.imec.be/era-vocabulary/) , links are broken

- IRIs in the ontology do not dereference.

- the ontology cannot be loaded in protege: failing to import schema.org, then issues in the era-skos file (due to its automatic generation using RML ?) . For example at line 1178  

- the demo[ http://era.ilabt.imec.be/test/compatibility](http://era.ilabt.imec.be/test/compatibility) is not functional: from and to fields are currently disabled

- IRIs in the application do not dereference



# Reviewer 3

SCORE: 2 (accept)

----- TEXT:

This work shows how Semantic Web technologies can be leveraged to create a data integration layer across data registries in the European Railway domain.



Reading this paper, I felt it represented the ideal example of an ISWC In-Use paper. The use-case tackled is compelling and to the best of my knowledge new (in a ISWC context that is), the presentation of the paper quite nice (modulo a few typos), and the impact of the approach seems substantial ("Based on the results obtained during this work, ERA officially decided to make Semantic Web and Linked Data-based approaches, the default setting for any future development [...]"). Overall, the solution put forward, though still in its infancy, is imho quite pragmatic and makes a lot of sense; I particularly enjoyed the discussion on how the path finding feature was implemented (some might complain that it should be implemented more efficiently / server-side, but I think the solution provided in the paper is quite pragmatic). Same for the ETL part, which sounds a bit old-school but which imho makes a lot of sense -- at least for a first iteration/deployment. 



A few points to improve in case the paper is accepted:

- I felt like a picture summarizing the various data sources, their contents and how they are interlinked, was missing at the very beginning of Section 3

- Along similar lines, it would be good to have a short section explaining how a rail network is operated (e.g., in terms of operational points) early in the paper.

- It is unclear how RING and ERATV "highlights a clear need for interoperability" (some additional detail would be welcome in that context).