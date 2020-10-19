---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: FAIR Data Point
--- 
# What is a FAIR Data Point
A FAIR Data Point (sometimes abbreviated to FDP) is the realisation of the vision of a group of authors of the [original paper on FAIR](https://doi.org/10.1038/sdata.2016.18) on how (meta)data could be presented on the web using existing standards, and without the need of APIs.

A FAIR Data Point ultimately stores _information about data sets_, which is the definition of _metadata_. And just like the _webserver_ in the WWW in the beginning of the 1990s brought the power of publishing text to anyone, a FAIR data point aims to give anyone the power of putting their own data on the web.

The system is called a **FAIR** data point because it takes care of a lot of the issues that need to be taken care of to make data FAIR; especially with the metadata needed for **F**indability and **R**eusability, and a uniform open way of **A**ccessing the data. The FAIR data point also addresses the **I**nteroperability of the metadata it stores, but it leaves the Interoperability aspects for the data itself to the data provider.

# Components
The FAIR Data Point as we have implemented it has three components.

The first and most important component is a _definition_ of the [FAIR Data Point "API"](https://github.com/FAIRDataTeam/FAIRDataPoint). It is completely based on semantic metadata standards (mostly [Data Catalog (DCAT)](https://www.w3.org/TR/vocab-dcat-2/) and [Dublin Core](https://dublincore.org/), combined with the [Linked Data Platform (LDP)](https://www.w3.org/TR/ldp/)), and based on the [REST](https://en.wikipedia.org/wiki/Representational_state_transfer) philosophy. This combination targets the the highest possible technical interoperability in combination with a relatively simple implementation. The FAIR data point protocol comes with a tool that can be used to test the compliance of an implementation.

The second component is a _reference implementation_ of the metadata registration service: A service implementing the API specification. It contains an authentication system to allow maintainers to define and update metadata. Read-only access to the data is public.

The third component is a _client_ of the API: a web front end that can be used to add and edit the information in the metadata registration service, or to query it. As an editor, it contains a simple validation of data types based on the [Shapes Constraint Language (SHACL)](https://www.w3.org/TR/shacl/). It facilitates the creation of metadata profiles as well as filling them, but this is meant to support the FAIR data point, and not meant to replace complete metadata profile development systems like [CEDAR](https://metadatacenter.org/).

# Examples of use
Several projects are under way that will use FAIR Data Points to make data sets known to other researchers. Some examples:
* The [VODAN](https://www.vodan-totafrica.info/about-vodan) project installs FAIR data points in several different (firstly African) countries, and uses these to collect information on COVID-19 patients. This network will also work on implementing the [FAIR Data Train](https://personalhealthtrain.org/) in order to allow distributed analysis of the data.
* Dutch academic hospitals will be implementing FAIR Data Points to collect COVID-19 data too, with the primary aim of reducing the maintenance burden of several Covid-19 data portals.

# Networking FAIR Data Points together
The FAIR Data Point protocol contains a component to notify a client of updates to its data. This _ping_ system allows for the creation of networks of FAIR Data points that can be queried as a single unit. You can see a first instance of this at work in the FAIR Data Point [HOME Server](https://home.fairdatapoint.org/). This functionality will still be extended.

# Protocol implementations
There are several FAIR Data Point implementations in existence:
* The [reference implementation](https://github.com/FAIRDataTeam/FAIRDataPoint) as described above.
* The [MOLGENIS](https://www.molgenis.org) software supports the FAIR Data Point protocol.
* [Castor](https://www.castoredc.com) currently supports a previous version.
* The [Netherlands eScience Center](https://www.esciencecenter.nl) have their own [implementation](https://github.com/NLeSC/fairdatapoint).
* The [SURF Repository](https://repository.surfsara.nl) implements the protocol.

<!--- DANS? And how far are we with DataVerse? -->

# Links
* Introductory Videos by Luiz Bonino:
    * [Introduction to the FAIR Data Point](https://www.youtube.com/watch?v=PtS_ek7BXSA)
    * [Local deployment of the FAIR Data Point](https://www.youtube.com/watch?v=rN_IVwppL_E)
* Resources
* FAQ
