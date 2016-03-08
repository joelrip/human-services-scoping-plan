---
layout: default
title:  "High Level Plan"
---

Coming soon.

## Possible Contents
- High Level Design/System Map
- Project Partners
- User Stories
- Implementation Plan
- Sustainability Plan
- High Level Project Budget/Cost Estimate

## High Level Design/System Map

The pilot project would consist of the following components:

**Federal, State, and Local Open Data Portals:** A distributed network of open data portals (including geographic information system “geoportals”) across federal, state, and local agencies would source datasets about community resources in the Human Services Data Specification (HSDS) format.

**2-1-1 Systems:** Local 2-1-1 organizations that opt-in to the pilot project would expose community resource directory data via application programming interface (API) in HSDS format.

**Core Application:** A core application that includes a database and API would consume relevant datasets across the distributed network of open data portals and store records locally. The application would make data available to external applications via its API to ensure that application developers only need a single endpoint to consume data.

**Version Control Protocol:** A version control protocol would sit between the core application and each open data portal, enabling the update of records at the field level rather than at the entire dataset level. The protocol also would identify conflicting fields in common records sourced from multiple data stores.

**Intelligent Reconciliation:** An algorithm would automate reconciliation between conflicting records in easy cases and escalate records for human review and manual reconciliation in harder cases. The core application would expose the resulting records via its API. Unreconciled records would be flagged as such.
