# Cargoson (cargoson)

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

Cargoson is an Estonian B2B cloud transport management software (TMS) platform for manufacturers and wholesalers. Its unified REST API lets shippers request freight rates, book shipments, generate labels, and track deliveries across 2,000+ carriers using one set of endpoints, authentication, and data formats. Cargoson is carrier-neutral; customers contract directly with their own carriers and upload their own freight rates.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/apis.yml)

## Tags

- Transport Management
- TMS
- Freight
- Shipping
- Logistics
- Carriers

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Cargoson Shipments API

Create shipment queries or direct bookings via POST /queries, then retrieve labels and generate return labels for existing bookings. A query can be created without a carrier (for later comparison) or booked directly by supplying a direct_booking_service_id.

- **Human URL:** [https://www.cargoson.com/en/integrations](https://www.cargoson.com/en/integrations)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Shipments
- Bookings
- Labels

#### Properties

- [Documentation](https://www.cargoson.com/en/integrations)
- [OpenAPI](openapi/cargoson-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cargoson.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cargoson.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cargoson Price Requests & Quotes API

Retrieve live freight rate quotes across activated carriers via POST /freightPrices/list, comparing cost, speed, and service level before selecting a carrier. Prices are pulled directly from each carrier's system.

- **Human URL:** [https://www.cargoson.com/en/integrations](https://www.cargoson.com/en/integrations)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Price Requests
- Quotes
- Freight Rates

#### Properties

- [Documentation](https://www.cargoson.com/en/integrations)
- [OpenAPI](openapi/cargoson-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cargoson.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cargoson.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cargoson Transports & Tracking API

Retrieve transport and tracking details for an existing shipment via GET /bookings/{reference} using the Cargoson booking reference.

- **Human URL:** [https://www.cargoson.com/en/integrations](https://www.cargoson.com/en/integrations)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Transports
- Tracking
- Status

#### Properties

- [Documentation](https://www.cargoson.com/en/integrations)
- [OpenAPI](openapi/cargoson-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cargoson.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cargoson.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cargoson Carriers & Services API

List the carrier services available on your company account via GET /services/list. Returned service IDs can be used for direct booking through the Shipments API.

- **Human URL:** [https://www.cargoson.com/en/integrations](https://www.cargoson.com/en/integrations)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Carriers
- Services

#### Properties

- [Documentation](https://www.cargoson.com/en/integrations)
- [OpenAPI](openapi/cargoson-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cargoson.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cargoson.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cargoson Addresses API

Collection and delivery address details (country, postcode, address rows, city, company, contact name and phone) are supplied inline on query and pricing requests. A standalone documented address-book endpoint was not confirmed in public documentation.

- **Human URL:** [https://www.cargoson.com/en/integrations](https://www.cargoson.com/en/integrations)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Addresses
- Collection
- Delivery

#### Properties

- [Documentation](https://www.cargoson.com/en/integrations)
- [OpenAPI](openapi/cargoson-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/cargoson.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/cargoson.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Cargoson Webhooks

Cargoson can deliver real-time event notifications (shipment status updates, booking confirmations, shipment changes) to a customer-configured endpoint URL, set up under Settings > Integrations > Webhooks. Public payload schemas are not documented; setup is arranged with Cargoson support.

- **Human URL:** [https://www.cargoson.com/en/blog/what-are-webhooks-and-how-do-they-work](https://www.cargoson.com/en/blog/what-are-webhooks-and-how-do-they-work)
- **Base URL:** `https://www.cargoson.com/api/v1`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://www.cargoson.com/en/blog/what-are-webhooks-and-how-do-they-work)

## Common Properties

- [GitHub Organization](https://github.com/cargoson)
- [LinkedIn](https://www.linkedin.com/company/cargoson)
- [Website](https://www.cargoson.com/)
- [Documentation](https://www.cargoson.com/en/integrations)
- [Plans](plans/cargoson-plans-pricing.yml)
- [Rate Limits](rate-limits/cargoson-rate-limits.yml)
- [Fin Ops](finops/cargoson-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
