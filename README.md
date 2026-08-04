# Estated (estated)

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
