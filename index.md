---
layout: default
title:  "Home"
---

We're scoping a potential pilot project in California to develop a **[federated publishing platform](https://openreferral.org/data-for-good-exchange-a-new-paper-with-an-old-concept/)** for human services information.

We're exploring:

1. **A vendor driven, standards-based approach**. We will recommend pursuing the pilot in a geography that uses information and referral systems with an open API, structured in the [Human Services Data Specification](https://github.com/codeforamerica/OpenReferral/blob/master/Human%20Services%20Data%20Specification%20%20v1.0.md) format. Similarly, we seek to federate from city, county, and state open data portals that might contain relevant information. That is, the willingness of vendors to participate in this pilot will determine the specific geography (or set of geographies) where we believe the pilot should take place.
2. **Touchpoints for updated information**. We seek to identify the touchpoints or transactions which might trigger opportunities for updating a community resource provider's information. The most logical touchpoint is centered around the administration of grants. We've heard from stakeholders that a community resource provider's services will vary based on the objectives of their funders. This is a ripe opportunity to trigger updates to a resource directory as a condition of receiving funds.
3. **Version control tools**. The federated publishing platform we envision will pull data from many different sources, likely leading to conflicting information. Therefore, we will recommend that a version control system such as [Git](https://git-scm.com/) or [Dat](http://dat-data.com/) ([PublicBits.org](http://dat-data.com/blog/2016-02-01-announcing-publicbits)) be used to help reconcile such conflicts.

Our design principles are:

- **Accessibility**. The federated publishing platform must be openly accessible, enabling use by many different applications and tools.
- **Robustness**. The platform should consume data from as many sources as possible to provide end users with the most complete picture of available resources in their communities.
- **Freshness**. In order to be relevant, a core objective of the platform must be to ensure the most up-to-date information about community resources as possible.
- **Credible**. While we believe that any user should be able to flag information or (possibly) suggest updates, such information must be verified by trusted sources to ensure credibility.
