---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: FAIR Data Point
--- 
# What is a FAIR Data Point
A FAIR Data Point is a realisation of the vision of a group of authors of the [original paper on FAIR](https://doi.org/10.1038/sdata.2016.18) on how (meta)data could be presented on the web using existing standards, and without the need of APIs.

A FAIR Data Point ultimately stores _information about data sets_, which is the definition of _metadata_. And just like the _webserver_ in the WWW in the beginning of the 1990s brought the power of publishing text to anyone, a FAIR data point aims to give anyone the power of putting their data on the web.

The system is called a FAIR data point because it takes care of a lot of the issues that need to be taken care of to make data FAIR; especially with the metadata needed for Findability and Reusability, and a uniform open way of Accessing the data. The FAIR data point also addresses the Interoperability of the metadata it stores, but it leaves the Interoperability aspects for the data to the user.

# Components
* Protocol (plus tester)
    * Standards based
         * DCAT v2
         * Dublin Core + …. (FIP / M4M ?)
         * LDP
* Metadata registration system
    * Store semantic metadata
* Web front end
    * Add and edit stuff in the FDP
    * Validates data types
    * Not a full-fledged CEDAR

# Examples of use
* Covid, VODAN

# Example implementations
* DTL Reference implementation
* Molgenis
* Castor
* eScience Center 
* SURF

# Links
* Home.fairdatapoint.org
* Github
* FDP specifications
* Resources
* Luiz’ intro videos
* FAQ
