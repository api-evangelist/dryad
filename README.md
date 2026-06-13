# Dryad

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
