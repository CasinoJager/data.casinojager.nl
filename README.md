# Data

## Status endpoint

`GET /api/v1/status.json`

- [Hosted endpoint](https://data.casinojager.nl/api/v1/status.json)
- [GitHub Raw — main](https://raw.githubusercontent.com/CasinoJager/data.casinojager.nl/main/public/api/v1/status.json)

The same static JSON file is published through Astro and GitHub. It is an availability test for the public files, not a live check of a collector or database. No casino records are included.

- `service`: the service hostname.
- `status`: `ok` for this test document.
- `apiVersion`: the major format version, matching `v1` in the URL.
- `updatedAt`: the last metadata update in UTC (ISO 8601). Update it when this document changes; do not regenerate it on each build or request. It does not indicate dataset freshness.

[Cloudflare Pages](https://developers.cloudflare.com/pages/configuration/serving-pages/#behavior) provides ETag-based cache revalidation for hosted files. GitHub Raw uses GitHub's own caching policy.
