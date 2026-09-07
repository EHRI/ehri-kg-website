---
title: "The EHRI-KG is now aligned with RiC-O 1.1 and new services available"
linkTitle: "EHRI-KG aligned with RiC-O 1.1 and more"
date: 2026-09-07
image: sampo-screenshot.png
summary: |
  After almost one year since the last update, the EHRI-KG announces the release of the EHRI Ontology 0.2.0 aligned with Records in Contexts 1.1, as well as the update of the whole infrastructure to comply with this new version. In addition, new services have been implemented and launched seeking to cover the usage of the EHRI-KG by different types of users.
---

It has been almost a year since our last news, though the EHRI-KG team has been intensively working behind the curtains in a lot of new things, and it is now ready to face the last phase of the project.

The main highlight is the release of the EHRI Ontology 0.2.0, now aligned with the Records in Contexts Ontology (RiC-O) 1.1. The EHRI-KG and all the associated services have been updated to be compliant with this new version. This is a big milestone for the project since this is the latest version of RiC-O available and makes of the EHRI-KG a complete demonstrator on how trans-national archival data can be represented using this important standard, as well as making our partner's data readily-compatible with other initiatives implementing it.

However, this is only part of what kept us busy during the last year. In parallel, we have been working in a series of tools to facilitate the (re)-use and exploration of EHRI's KG. We acknowledge that semantic web technologies have a somewhat steep learning curve, so more user-friendly approaches are needed depending on the user's expertise. Therefore, we are happy to introduce the following tools and services:

* Sampo-UI: Sampo-UI is a software package created by the Semantic Computing Research Group (SeCO) at the Aalto University, which allows users to navigate a Knowledge Graph using a faceted search as well as generating different types of visualisations and graphics. At EHRI-KG we have adapted, configured and customised it to work with the EHRI-KG. If you are not an expert on semantic technologies, and just want an easy to use interface without losing any capabilities, this is your starting point.

* OpenAPI REST API: If SPARQL is not your cup of tea, but nevertheless want to re-use EHRI-KG's data in your application, we have you covered. Using grlc, a CLARIAH-hosted software library that converts a set of SPARQL queries in a fully-fledged REST API compliant with the OpenAPI specification, we have deployed a new REST API for the EHRI-KG. This API exposes a number of endpoints covering the most frequent consult operations, and some of them can be further parametrised.

# Data mapping architecture
Despite not being a new service, we have invested a lot of effort on streamlining our data mapping architecture, not only to adapt the conversions to RiC-O 1.1 and our EHRI ontology 0.2.0, but also to make it more resilient, ensure the validity of the data and monitor changes on the EHRI Portal, so that they are incrementally included in the EHRI-KG. Therefore, we are moving from a batch generated and static KG to a living one that is fully synchronised with the EHRI Portal data.

If you want to know more, you can read our recent paper, published and presented at the 7th International Workshop on Knowledge Graph Construction co-located with 23rd Extended Semantic Web Conference (ESWC 2026) (see [Deliverables](../../deliverables) section).

# Following steps
While the vast majority of the infrastructure is already implemented, we still have two more lines of work for the following months. 

On the one hand, before the end of the project, the EHRI-KG will be moved to a production server and IRIs will be consolidated (no need to worry, we will implement the necessary redirections). From this point forward, the EHRI-KG will be integrated as a new service of the EHRI-ERIC and the infrastructure sustained beyond this project timeline.

On the other hand, following recent advancements in AI and hybrid techniques combining LLMs and KGs, we are experimenting with new methods of accesing and consulting the resulting KG, so the information contained within can be more easily exploited by all kinds of users, and researchers can be more productive when using this type of data. If you are interested in this new line of work, stay tuned as we will share more soon!

# Links to main outputs:
* EHRI Ontology 0.2.0: [https://lod.ehri-project-test.eu/ontology/0.2.0](https://lod.ehri-project-test.eu/ontology/0.2.0)
* Sampo-UI: [https://lod.ehri-project-test.eu/sampo](https://lod.ehri-project-test.eu/sampo)
* OpenAPI REST API: [https://lod.ehri-project-test.eu/openapi/api-local](https://lod.ehri-project-test.eu/openapi/api-local)