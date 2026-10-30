# ISO Country/Currency/Language Codes

ISO 3166-1 (country), ISO 4217 (currency), ISO 639 (language) codes

- **Base URL:** https://chirag127.github.io/iso-codes-api/
- **Contract:** [openapi.yaml](./openapi.yaml)
- **Repository:** https://github.com/chirag127/iso-codes-api

This is a static JSON API. No authentication, no server, and no rate limit. The committed JSON is the database.

## Endpoints

| Method | Path | Purpose |
| --- | --- | --- |
| `GET` | `/api/v1/data.json` | ISO Country/Currency/Language Codes |
| `GET` | `/api/v1/individual/{id}.json` | Get single record |
| `GET` | `/api/v1/search-index.json` | Search index |
| `GET` | `/api/v1/meta.json` | Dataset metadata |

## Data and metadata

The current record count, source, retrieval time, and schema version are published at [`/api/v1/meta.json`](https://chirag127.github.io/iso-codes-api/api/v1/meta.json). The static data lives under `api/v1/`.

Data licensing: CC0-1.0. Code licensing: MIT. See `openapi.yaml` and the repository license for details.

## Local verification

```bash
ls api/v1
curl -s https://chirag127.github.io/iso-codes-api/api/v1/meta.json
```
