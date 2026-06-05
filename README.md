# Estated (estated)

Estated is a property-data company that operates a JSON REST API returning detailed U.S. residential and commercial property records — assessor data, parcel geometry, structure characteristics, taxes, assessments, market assessments, valuation (AVM), owner of record, deeds, and parcel boundaries. Lookups can be performed by split address, parsed address components, a single combined address string, or by FIPS county code + assessor parcel number (APN). The current public surface is the Property Data API v4 at `https://apis.estated.com/v4/property`, authenticated with a `token` query parameter. Estated was acquired by ATTOM Data in 2020 and its infrastructure is being migrated to ATTOM; the Estated developer documentation is scheduled to be deprecated during 2026, after which property data access will be served through ATTOM's documentation and endpoints. Existing Estated tokens continue to work through the transition and no integration changes are required during the migration window.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/estated/refs/heads/main/apis.yml)

## Scope

- **Type:** API
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Property Data
- Real Estate
- Property Records
- Assessor
- Parcels
- APN
- FIPS
- Deeds
- AVM
- Valuation
- Boundaries
- GIS
- Owner Of Record
- Tax Assessment

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Estated Property Data API

Look up a U.S. property record by address (split, parsed, or combined) or by FIPS+APN. Returns a Property object containing address, parcel, structure, taxes, assessments, market_assessments, valuation, owner, deeds, and boundary (WKT + GeoJSON MultiPolygon). Authenticated via `token` query parameter.

- **Human URL:** [https://estated.com/developers/docs/v4](https://estated.com/developers/docs/v4)
- **Base URL:** `https://apis.estated.com`

#### Tags

- Property Data
- Real Estate
- Parcels
- Deeds
- AVM

#### Properties

- [Documentation](https://estated.com/developers/docs/v4)
- [Documentation](https://estated.com/developers/docs/v4/property/overview)
- [Documentation](https://estated.com/developers/docs/v4/property/schema)
- [Documentation](https://estated.com/developers/docs/v4/property/values)
- [Sign Up](https://estated.com/login)
- [OpenAPI](openapi/estated-property-data-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/estated-property-data-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/estated-property-data-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/estated-property-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/estated-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/estated-get-property-example.json)
- [Spectral Rules](rules/estated-rules.yml)
- [Plans](plans/estated-plans-pricing.yml)
- [Rate Limits](rate-limits/estated-rate-limits.yml)
- [Fin Ops](finops/estated-finops.yml)
- [Vocabulary](vocabulary/estated-vocabulary.yml)

## Common Properties

- [Website](https://estated.com)
- [Developers](https://estated.com/developers/docs/v4)
- [Documentation](https://estated.com/developers/docs/v4/property/overview)
- [Schema](https://estated.com/developers/docs/v4/property/schema)
- [Sign Up](https://estated.com/login)
- [Parent Company](https://www.attomdata.com/)
- [Acquisition Announcement](https://www.attomdata.com/news/company-news/attom-company-announcement-10/)
- [Parent Company Product](https://www.attomdata.com/solutions/property-data-api/)
- [Terms Of Use](https://www.attomdata.com/terms-of-use/)
- [Privacy Policy](https://www.attomdata.com/privacy/)
- [Contact](https://www.attomdata.com/contact-us/)
- [Git Hub](https://github.com/estated)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
