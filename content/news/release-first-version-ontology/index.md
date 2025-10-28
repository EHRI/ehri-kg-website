---
title: "The first version of the EHRI Ontology has been released"
linkTitle: "EHRI Ontology 0.1.0 released"
date: 2025-10-24
image: ehri-ontology-crop.svg
summary: |
  The EHRI-KG team has released version 0.1.0 of the EHRI Ontology, marking a significant milestone in the ongoing effort to publish the EHRI Portal data as Linked Open Data. This ontology extends Records in Contexts Ontology (RiC-O) 1.0.2, integrating schema.org and EHRI-specific properties to fill semantic gaps.
---

Last week, we hit one of the main milestones in this project by releasing [the very first version of our EHRI Ontology](http://lod.ehri-project-test.eu/ontology/0.1.0). This ontology encapsulates the work of the last three years in trying to convert the EHRI Portal data into RDF, aligning as much as possible with the Records in Contexts Ontology (RiC-O). It all started with an initial conversion to the formerly latest RiC-O version available (0.2) which was the subject of our [paper at ISWC 2023](https://doi.org/10.1007/978-3-031-47243-5_20). During the first phase of this project, we have reexamined the conversion between the [EHRI's Data Model](https://portal.ehri-project.eu/help/datamodel) and the now first stable version of RiC-O (1.x) with the ambition to offer an updated transformation of the EHRI Portal data and a formalisation of our additions to RiC-O (the latter materialised in the form of an ontology).

Therefore, the resulting ontology works as an extension of RiC-O 1.0.2, complementing it with schema.org properties and EHRI's own ones to represent some missing semantics. It has been encoded in OWL following Semantic Web standards and best practices, and the documentation has been generated using [Widoco](https://github.com/dgarijo/Widoco). 

At the same time, we have reworked our mapping workflow to match this ontology version alongside many tehcnical improvements, including new attributes previously missing, more meaningful IRIs, and additional links between entities (such as the copy-original links). This whole workflow is available in a [GitHub repository](https://github.com/EHRI/ehri-kg-mapping) and contains a number of supplementary resources which might be useful for other practitioners:
- ShExML mapping rules used for the conversion: The set of mapping rules can be adapted and reused by other projects seeking to undertake a similar conversion.
- Crosswalks between the EHRI Portal data and RiC-O: These represent a more easily readable version of the used mapping rules and can be used to understand how the conversion was established.
- Validation shapes: SHACL and ShEx validation rules aligned with the current EHRI Ontology version are provided, they can be reused and adapted to similar domains.

## What's next?
In the following months we will focus our efforts on the alignment with RiC-O 1.1, which will lead us to the release of the EHRI Ontology 0.2 and the update of the current mapping workflow. Moreover, we are currently working in the development of a real-time update service capable of processing update events from the EHRI Portal and trigger the necessary update actions in our KG. This will, ultimately, mean that the KG data will no longer be frozen to the data conversion date but rather it will be perfectly synchronised with the data hosted in the EHRI Portal.

## Links to the main outputs:
- EHRI Ontology 0.1.0: [http://lod.ehri-project-test.eu/ontology/0.1.0](http://lod.ehri-project-test.eu/ontology/0.1.0)
- EHRI-KG LodView interface: [https://lod.ehri-project-test.eu/](https://lod.ehri-project-test.eu/)
- EHRI Ontology GitHub repository: [https://github.com/EHRI/ehri-kg-ontology](https://github.com/EHRI/ehri-kg-ontology)
- EHRI-KG mapping GitHub repository: [https://github.com/EHRI/ehri-kg-mapping](https://github.com/EHRI/ehri-kg-mapping)
