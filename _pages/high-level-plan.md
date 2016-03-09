---
layout: default
title:  "High Level Plan"
---

## High Level Design/System Map

The pilot project would consist of the following components:

- **Federal, State, and Local Open Data Portals:** A distributed network of open data portals (including geographic information system “geoportals”) across federal, state, and local agencies would source datasets about community resources in the Human Services Data Specification (HSDS) format.
- **2-1-1 Systems:** Local 2-1-1 organizations that opt-in to the pilot project would expose community resource directory data via application programming interface (API) in HSDS format.
- **Core Application:** A core application that includes a database and API would consume relevant datasets across the distributed network of open data portals and store records locally. The application would make data available to external applications via its API to ensure that application developers only need a single endpoint to consume data.
- **Version Control Protocol:** A version control protocol would sit between the core application and each open data portal, enabling the update of records at the field level rather than at the entire dataset level. The protocol also would identify conflicting fields in common records sourced from multiple data stores.
- **Intelligent Reconciliation:** An algorithm would automate reconciliation between conflicting records in easy cases and escalate records for human review and manual reconciliation in harder cases. The core application would expose the resulting records via its API. Unreconciled records would be flagged as such.

## Project Partners

We believe the following organizations would be strong candidates to partner in the pilot project:

### United Ways of California

[United Ways of California](https://www.unitedwaysca.org/) coordinates the work of local United Ways throughout California. Led by President & CEO Pete Manzo, the organization champions the role of 2-1-1 in providing information and referral services to individuals in need. Specifically, California United Ways operate or provide funding for 2-1-1 programs in 28 of the 35 counties where 2-1-1 is available in California.

### CharityLogic

CharityLogic is the company that makes [iCarol](http://www.icarol.com/), Neil McKechnie, COO and Director of Services and Development for iCarol, is leading internal efforts to develop an Open Referral API. Because the company has such substantial market share (used in 30 of 35 California counties), the pilot project would complement existing efforts to create a single statewide database of community resource providers.

### Socrata

[Socrata](https://www.socrata.com/) open data portals are in use by seven California counties, along with the [California Health and Human Services Agency](https://chhs.data.ca.gov/), making them the most popular open data portal vendor in the state. The [Socrata API](https://dev.socrata.com/consumers/getting-started.html) uses RESTful (REpresentational State Transfer) design pattern that simplifies consumption of data by applications. The company has expressed interest in supporting counties that wish to participate in a pilot project.

### U.S. Open Data

[U.S. Open Data](https://usopendata.org/) manages the [Dat project](http://dat-data.com/). Dat is an emerging protocol that enables version control for datasets across a distributed network. [Dat 1.0](http://dat-data.com/blog/2016-02-01-dat-1) was recently released and will power [PublicBits](http://dat-data.com/blog/2016-02-01-announcing-publicbits), a registry for sharing datasets across an open network. This promising technology would allow a single, authoritative version of data to be made available from many sources, while retaining version history at an atomic field level (rather than at the [line-level](http://blog.okfn.org/2013/07/02/git-and-github-for-data/)).

### County Welfare Directors Association of California

The [County Welfare Directors Association of California](http://www.cwda.org/) (CWDA) plays an instrumental role in shaping state policy for vulnerable Californians. The organization represents human service directors from all 58 counties in the state and has actively engaged with our research process. The organization is well-positioned to advise on identifying the specific opportunities when grants or other funding to community resource providers might trigger an update to a dataset regarding available resources in a community.  

### Department of Social Services

The [California Department of Social Services](http://www.cdss.ca.gov/cdssweb/default.htm) (CDSS) has a mission *"to serve, aid, and protect needy and vulnerable children and adults in ways that strengthen and preserve families, encourage personal responsibility, and foster independence."* With leadership from Deputy Director Pete Cervinka and Assistant Director for Horizontal Integration, Adam Dondro, CDSS continues to express interest in supporting efforts that align with their mission and that might integrate well with the California Health and Human Services Agency's open data initiative.

<!-- ## User Stories



## Implementation Plan

Managed onboarding...

Grant triggers...

## Sustainability Plan



## High Level Project Budget/Cost Estimate


## Recommendations and Next Steps -->

<p class="pagination">
  <a href="/data-ecosystem">&larr; Prev</a>
  <span class="pull-right"><a href="/works-cited-and-thanks">Next &rarr;</a></span>
</p>
