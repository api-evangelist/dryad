# Dryad

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Dryad is a nonprofit open data publishing platform and repository that enables researchers to publish, preserve, and access research datasets associated with peer-reviewed publications. It serves biology, ecology, and related disciplines, assigning citable DOIs to datasets and providing long-term preservation with curation support.

## API

The Dryad REST API v2 (current version 2.1.0) supports:

- **Search API** — Anonymous dataset discovery by keyword, affiliation (ROR), journal ISSN, modification date, and related work identifiers
- **Dataset API** — Retrieve dataset metadata, versions, and file listings
- **Submission API** — Create, update, and submit datasets with file uploads (direct binary or URL reference)
- **Reporting API** — Access automatically generated repository reports

Base URL: `https://datadryad.org/api/v2`

Documentation: https://datadryad.org/api/v2/docs

## Authentication

The API uses OAuth2 client credentials grant. Tokens are obtained via:

```
POST https://datadryad.org/oauth/token
```

Tokens are valid for 10 hours. Anonymous access is available for public dataset search and retrieval.

## Pricing

Data Publishing Charges (DPC) apply to dataset submission, starting at $150 for datasets up to 5 GB. Institutional and publisher partners can sponsor submissions for affiliated authors. Full pricing: https://datadryad.org/help/requirements/costs

## Links

- Website: https://datadryad.org
- API Documentation: https://datadryad.org/api/v2/docs
- GitHub: https://github.com/datadryad
- Blog: https://blog.datadryad.org
- Contact: help@datadryad.org
