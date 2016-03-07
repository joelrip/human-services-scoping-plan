---
layout: default
title:  "Data Ecosystem Analysis"
---

Coming soon.

## Possible Contents

- Human Services Dataset Inventory
- Data Schema Inventory
- Data Journey Maps

## County Public Data System Vendor Inventory

California's 57 counties offer human services information on a wide variety of open data portals, 211 search tools, and geographical information system (GIS) portals, along with countless ad-hoc offline services. The majority (62%) of these public data systems, however, are operated by three vendors: Socrata, iCarol, and Esri. 

### County Open Data Portals 

Open data portals, which offer datasets and APIs from various county departments freely to the public, typically include some human services datasets. Although only 11 California counties have some form of open data portal, seven of these (totalling 44% of the state's population) have a portal operated by Socrata. Other county portals are operated by Accela, Junar, NuCivic, and OpenGov.

### 211 Systems

211 systems offer human services directory information by phone and online. 37 California counties have an operational 211 system, of which 29 use a system built on iCarol referral and helpline software. Other counties offer 211 services from Bowman Systems, Eden I&R, ReferWeb, and Visionlink. Los Angeles and San Mateo counties have their own proprietary 211 systems. 

### GIS Portals

GIS portals offer digital maps, some of which provide layers containing human services location data. 37 California counties have a GIS portal, of which 17 have a portal built on Esri technology. Other counties offer portals from CalCAD, GISCloud, and SimpleLayers. Many counties have their own ad-hoc portals.

### Discussion

Because there are relatively few major vendors among California county open data, 211, and GIS portals, partnering directly with these vendors to access data offers an alternative to coordinating between multiple counties. Partnering primarily with vendors has many benefits: 
- Pre-existing APIs and other data pathways
- Low barrier to entry for counties with same vendor
- Fewer points of contact
- Easier access to technical collaborators
- Easier access to county data inventories

## Human Services Taxonomies 

There are several standards for classifying human services information. Two in particular are relevant to the State of California's current effort: the AIRS/211 LA County taxonomy, the *de facto* nationwide standard; the Open Eligibility taxonomy, a basic, nonproprietary alternative designed to be extended for specific use cases.

###AIRS/211 LA County
The AIRS/211 LA County taxonomy, first developed by the nonprofits Alliance of Information and Referral Systems (AIRS) and 211 LA County in 1983, has been widely adopted for human services classification in the U.S. and Canada. It comprises a hierarchical structure for specifying over 12,000 types of human services. However, as a proprietary standard, it is only available through an annual subscription, and cannot be freely modified or extended to accommodate additional information categories.

###Open Eligibility
The Open Eligibility taxonomy, developed by the public benefit corporation Aunt Bertha in 2013, is a proof-of-concept for an open-source human services classification system. Although it is freely available to use and modify, it is considerably less detailed than the AIRS/211 LA County taxonomy, and may be insufficiently complex to capture the full range of human services in California without additional development.

###Discussion
An ideal approach to federating human services information in the State of California would be open by default but interoperable with widely used proprietary taxonomies. Offering Open Eligibility as the default taxonomy, while offering AIRS/211 LA County for services that require more complex specification, represents such a compromise. The Human Service Data Specification (HSDS), discussed in greater detail below, represents one approach to reconciling these standards. 

<!-- {% highlight json %}
{% include openeligibility.json %}
{% endhighlight %} -->
