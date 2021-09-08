# Rebuttal Letter

Dear reviewers,



First of all, we would like to thank you for your kind comments and observations on our work. We are very happy to see that all reviewers found our work to be fitting for the In-Use track.

We completely agree with the reviewers comments regarding the room for improvement of our demonstrator application (http://era.ilabt.imec.be/test/compatibility-check-demo/).

Aiming to facilitate its use, we included a “help page” in the application (click on the circled i symbol next to the Route Compatibility Check title on the top left) that shows how to use it and explains what happens “under the hood”. We did not mention this in the paper and will add a remark about it in the paper, as it is not intuitive enough for the users. 

Currently we are working on a follow up project where we are taking this architecture and its components into a production-ready state. Multiple improvements are being applied, including type-in autocompletion for the FROM and TO fields in the RCC application (as mentioned by reviewer 2). Ultimately, our architecture will be deployed within DIGIT’s (https://ec.europa.eu/info/departments/informatics_en) and ERA’s IT infrastructure; offering RCC as a new service application open for the European railway domain. In this project we will also properly publish our ontology, making its IRIs dereferenceable. All the different components will be kept open source and “containerized” aiming to lower the technological entry barrier as pointed out by reviewer 1. 

We tested importing our ontology directly from its URL (http://era.ilabt.imec.be/era-vocabulary/ontology.ttl) into Protege v5.5.0. Indeed schema.org fails to be imported because its IRI (https://schema.org) does not dereference to machine readable content, but the rest of ontologies are imported successfully, including the era-skos ontology. We are able to visualize its class hierarchy and run reasoners that do not show any consistency issues. We have added some screenshots of this in the ontology Github repository (https://github.com/julianrojas87/era-vocabulary/tree/master/protege) as proof.

Lastly, we will address all the pointed grammatical issues and specially follow the improvement suggestions made by reviewer 3, to better explain and clarify our contributions in section 3.



Kind regards,

Julian, Marina, Polynmia, Ivo, Dylan, Pieter and Ruben.