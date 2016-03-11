---
layout: default
title:  "Data Ecosystem Analysis"
---

## Human Services Dataset Federation

A federated human services data system would pull information from numerous federal, state, and local data sources. Enumerating all the datasets the core API could consume is beyond the scope of this plan, but the examples below illustrate how services data from different jurisdictions could be combined in such a system.

### Example: Food Assistance

There are many avenues available for people seeking food assistance in the United States. These include the Federal Supplemental Nutrition Assistance Program (SNAP), state-administrated Women, Infants and Children (WIC) aid, and local food banks. A California human services API could consume [SNAP locations](http://www.fns.usda.gov/snap/retailerlocator), locations for the state's [authorized WIC vendors](https://cdph.data.ca.gov/Facilities-and-Services/Women-Infants-and-Children-WIC-Authorized-Vendors/i7wi-ei4m), and [county food bank contact information](http://www.cafoodbanks.org/cafb-member-food-banks). A suite of data like this could be used by community organizations that wish to offer food assistance directly, by showing gaps in existing service coverage and providing contact information for food bank suppliers nearby.

### Example: Mental Health Services

Mental health services information comes from cross-jurisdictional sources as well. A California human services API could bring together the federal Substance Abuse and Mental Health Services Administration's [facilities information](http://www.samhsa.gov/data/mental-health-facilities-data-nmhss/reports), the California Department of Rehabilitation's [traumatic brain injury center](https://chhs.data.ca.gov/Facilities-and-Services/California-Independent-Living-and-Traumatic-Brain-/s3hx-yvpp) and [office locations](https://chhs.data.ca.gov/Facilities-and-Services/Department-of-Rehabilitation-Office-Contact-Inform/exxu-vffk), and [county mental health provider directories like this one from Los Angeles County](https://data.lacounty.gov/Mental-Health/Department-of-Mental-Health-DMH-Provider-Directory/az6g-rq5y). This data suite could be used by caregivers to determine whether federal, state, or local services would be most convenient for a given patient.

## County Public Data System Vendor Inventory

California's 58 counties offer human services information on a wide variety of open data portals, 2-1-1 search tools, and geographical information system (GIS) portals, along with countless ad-hoc offline services. The majority (62%) of these public data systems, however, are operated by three vendors: Socrata, iCarol, and Esri.

#### [View the Complete Inventory](https://github.com/CAHealthData/human-services-scoping-plan/blob/gh-pages/data/county-assets.csv)

### County Open Data Portals

Open data portals, which offer datasets and APIs from various county departments freely to the public, typically include some human services datasets. Although only 11 California counties have some form of open data portal, seven of these (totalling 44% of the state's population) have a portal operated by Socrata. Other county portals are operated by Accela, Junar, NuCivic, and OpenGov.

### 2-1-1 Systems

2-1-1 systems offer human services directory information by phone and online. 37 California counties have an operational 2-1-1 system, of which 29 use a system built on iCarol referral and helpline software. Other counties offer 2-1-1 services from Bowman Systems, Eden I&R, ReferWeb, and Visionlink. Los Angeles and San Mateo counties have their own proprietary 2-1-1 systems.

### GIS Portals

GIS portals offer digital maps, some of which provide layers containing human services location data. 37 California counties have a GIS portal, of which 17 have a portal built on Esri technology. Other counties offer portals from CalCAD, GISCloud, and SimpleLayers. Many counties have their own ad-hoc portals.

### Discussion

Because there are relatively few major vendors among California county open data, 2-1-1, and GIS portals, partnering directly with these vendors to access data offers an alternative to coordinating between multiple counties. Partnering primarily with vendors has many benefits:

- Pre-existing APIs and other data pathways
- Low barrier to entry for counties with same vendor
- Fewer points of contact
- Easier access to technical collaborators
- Easier access to county data inventories

## Human Services Taxonomies

There are several standards for classifying human services information. Two in particular are relevant to the State of California's current effort: the AIRS/2-1-1 LA County taxonomy, the *de facto* nationwide standard; the Open Eligibility taxonomy, a basic, nonproprietary alternative designed to be extended for specific use cases.

### AIRS/2-1-1 LA County

The AIRS/2-1-1 LA County taxonomy, first developed by the nonprofits Alliance of Information and Referral Systems (AIRS) and 2-1-1 LA County in 1983, has been widely adopted for human services classification in the U.S. and Canada. It comprises a hierarchical structure for specifying over 12,000 types of human services. However, as a proprietary standard, it is only available through an annual subscription, and cannot be freely modified or extended to accommodate additional information categories.

### Open Eligibility

The Open Eligibility taxonomy, developed by the public benefit corporation Aunt Bertha in 2013, is a proof-of-concept for an open-source human services classification system. Although it is freely available to use and modify, it is considerably less detailed than the AIRS/2-1-1 LA County taxonomy, and may be insufficiently complex to capture the full range of human services in California without additional development.

#### [View the Open Eligibility Taxonomy](/open-eligibility)

### Discussion

An ideal approach to federating human services information in the State of California would be open by default but interoperable with widely used proprietary taxonomies. Offering Open Eligibility as the default taxonomy, while offering AIRS/2-1-1 LA County for services that require more complex specification, represents such a compromise. The Human Service Data Specification (HSDS), discussed in greater detail below, represents one approach to reconciling these standards.

## Data Schemas

In addition to taxonomies, there are also several database schemas that specify required, recommended, and optional information for describing services. These include various standards from AIRS; a "civic services schema" created by Google.org engineers to make services more machine-readable for search engines; and the National Information Exchange Model, a joint venture between the U.S. Departments of Homeland Security and Justice to create a highly general information-sharing schema.

One schema in particular attempts to reconcile these different formats into a single, open source medium of exchange: the Human Services Data Specification (HSDS). That schema was created by the Open Referral Initiative, with support from Code for America and the Knight Foundation. With HSDS, Open Referral attempts to establish interoperability between information-and-referral systems, such as 2-1-1, and web accessibility standards, such as the aforementioned "schema."

In addition to acting as an intermediary between other human services schemas, HSDS is agnostic with regard to taxonomy. As such, it can handle data categorized according to both the AIRS/2-1-1 LA County and Open Eligibility taxonomies.

Federating human services data across the State of California represents an ideal use-case for HSDS, insofar as it offers a common ground between the various systems and specifications already in use across the state.

<p class="pagination">
  <a href="/discovery-research">&larr; Prev</a>
  <span class="pull-right"><a href="/high-level-plan">Next &rarr;</a></span>
</p>
