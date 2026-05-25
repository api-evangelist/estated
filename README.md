# Estated

Estated is a property-data company offering a JSON REST API that returns detailed U.S. residential and commercial property records — assessor data, parcel geometry, structure characteristics, taxes, assessments, market assessments, valuation (AVM), owner of record, deeds, and parcel boundaries (WKT + GeoJSON). The current public surface is the **Property Data API v4** at `https://apis.estated.com/v4/property`, authenticated with a `token` query parameter.

Estated was acquired by **ATTOM Data Solutions** in 2020. Infrastructure is being migrated to ATTOM; existing Estated tokens continue to work, and the standalone Estated developer docs are scheduled to be deprecated during 2026, after which property data access will be served through ATTOM's documentation and endpoints.

## API

- **Estated Property Data API** — `GET /v4/property`
  - Lookup modes: split address, parsed components, combined-address string, or FIPS+APN
  - Docs: https://estated.com/developers/docs/v4
  - Overview: https://estated.com/developers/docs/v4/property/overview
  - Schema: https://estated.com/developers/docs/v4/property/schema
  - OpenAPI: [`openapi/estated-property-data-api-openapi.yml`](openapi/estated-property-data-api-openapi.yml)

## Artifacts

| Artifact | Path |
|---|---|
| OpenAPI 3.0.3 | [`openapi/estated-property-data-api-openapi.yml`](openapi/estated-property-data-api-openapi.yml) |
| JSON Schema (Property) | [`json-schema/estated-property-schema.json`](json-schema/estated-property-schema.json) |
| JSON-LD context | [`json-ld/estated-context.jsonld`](json-ld/estated-context.jsonld) |
| Operation example | [`examples/estated-get-property-example.json`](examples/estated-get-property-example.json) |
| Spectral rules | [`rules/estated-rules.yml`](rules/estated-rules.yml) |
| Naftiko capability | [`capabilities/property-lookup.yaml`](capabilities/property-lookup.yaml) |
| Plans & pricing | [`plans/estated-plans-pricing.yml`](plans/estated-plans-pricing.yml) |
| Rate limits | [`rate-limits/estated-rate-limits.yml`](rate-limits/estated-rate-limits.yml) |
| FinOps profile | [`finops/estated-finops.yml`](finops/estated-finops.yml) |
| Vocabulary | [`vocabulary/estated-vocabulary.yml`](vocabulary/estated-vocabulary.yml) |
| API Evangelist review | [`review.yml`](review.yml) |
| apis.yml manifest | [`apis.yml`](apis.yml) |

## Tier

**Tier-1** — Estated publishes a single, fully documented v4 Property Data API with a real GET endpoint, complete query-parameter schema, deeply nested response object schema, and explicit error and warning code tables. That meets the Tier-1 bar for "real, machine-actionable API surface" even though Estated does not publish a first-party OpenAPI artifact.

## Authentication

API key via the `token` query parameter:

```
GET https://apis.estated.com/v4/property?token=YOUR_TOKEN_HERE&combined_address=151+Battle+Green+Dr%2C+Rochester%2C+NY+14624
```

## Error & Warning Codes

| Class | Codes |
|---|---|
| Address parsing | `APE01` |
| Internal server | `ISE01`–`ISE09` |
| Endpoint | `EE01` |
| Request | `RE01`, `RE02`, `RE03`, `RE04` (throttle), `RE05`, `RE06` |
| Authorization | `AE02` (invalid), `AE03` (no calls remaining), `AE04` (deactivated) |
| Property warnings | `PW01` (none found), `PW02` (multiple) — not billable |
| Address parser warnings | `APW01` (no address), `APW02` (unknown suffix) — usually not billable |

## Parent Company

- ATTOM Data Solutions — https://www.attomdata.com/
- ATTOM Property Data API — https://www.attomdata.com/solutions/property-data-api/
- Acquisition announcement — https://www.attomdata.com/news/company-news/attom-company-announcement-10/

## Links

- Website: https://estated.com
- Developer docs: https://estated.com/developers/docs/v4
- Sign in: https://estated.com/login
- GitHub: https://github.com/estated

## Maintainer

- Kin Lane — API Evangelist — kin@apievangelist.com
