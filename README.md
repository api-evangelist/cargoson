# Cargoson (cargoson)

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
