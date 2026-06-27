# AU10TIX (au10tix)

AU10TIX is an identity verification and document authentication provider delivering KYC, document analysis, biometric face comparison, liveness, and fraud detection through a single REST API (the Back Office Server, "BOS") and web/mobile SDKs. The platform orchestrates verification workflows/sessions, returns structured results, and notifies clients via webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/apis.yml)

## Tags

- Identity Verification
- Document Authentication
- KYC
- Biometrics
- Fraud Detection

## Timestamps

- **Created:** 2026-06-25
- **Modified:** 2026-06-25

## APIs

### AU10TIX Identity Verification API

Orchestrates identity verification workflows (the Back Office Server, "BOS"). Creates a verification session/workflow, accepts document and selfie media, and returns a unique session/document identifier used to retrieve results. Authentication is OAuth2 (bearer/JWT) or certificate-based depending on integration.

- **Human URL:** [https://www.au10tix.com/products/platform/](https://www.au10tix.com/products/platform/)
- **Base URL:** `https://eus-api.au10tixservices.com`

#### Tags

- Identity Verification
- Workflows
- Sessions
- KYC

#### Properties

- [Documentation](https://www.au10tix.com/products/platform/)
- [OpenAPI](openapi/au10tix-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/au10tix.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/au10tix.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AU10TIX Document Authentication API

Authenticates government-issued ID documents (passports, driver's licenses, national ID cards) using document structure checks, data integrity validation, and digital forensic analysis, returning extracted fields and an authenticity verdict.

- **Human URL:** [https://www.au10tix.com/solutions/document-verification/](https://www.au10tix.com/solutions/document-verification/)
- **Base URL:** `https://eus-api.au10tixservices.com`

#### Tags

- Document Authentication
- OCR
- ID Documents

#### Properties

- [Documentation](https://www.au10tix.com/solutions/document-verification/)
- [OpenAPI](openapi/au10tix-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/au10tix.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/au10tix.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AU10TIX Face Comparison & Liveness API

Compares a captured selfie against the portrait on a verified ID document (1:1 face match) and performs passive/active liveness and deepfake detection to confirm a genuine, present person.

- **Human URL:** [https://www.au10tix.com/solutions/sdk/](https://www.au10tix.com/solutions/sdk/)
- **Base URL:** `https://eus-api.au10tixservices.com`

#### Tags

- Biometrics
- Face Comparison
- Liveness

#### Properties

- [Documentation](https://www.au10tix.com/solutions/sdk/)
- [OpenAPI](openapi/au10tix-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/au10tix.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/au10tix.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AU10TIX Results API

Retrieves the structured result of a verification session by its session/document identifier (polling with retry/backoff), returning the verification status (e.g. VERIFIED, FAILED, REVIEW) and the consolidated result payload.

- **Human URL:** [https://www.au10tix.com/products/platform/](https://www.au10tix.com/products/platform/)
- **Base URL:** `https://eus-api.au10tixservices.com`

#### Tags

- Results
- Decisions
- Polling

#### Properties

- [Documentation](https://www.au10tix.com/products/platform/)
- [OpenAPI](openapi/au10tix-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/au10tix.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/au10tix.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AU10TIX Webhooks API

Pushes verification decisions to a customer-registered callback URL the moment a workflow reaches a terminal state, removing the need to poll for status. Payload schemas are documented in AU10TIX's authenticated developer portal.

- **Human URL:** [https://www.au10tix.com/company/integrations/](https://www.au10tix.com/company/integrations/)
- **Base URL:** `https://eus-api.au10tixservices.com`

#### Tags

- Webhooks
- Callbacks
- Events

#### Properties

- [Documentation](https://www.au10tix.com/company/integrations/)
- [OpenAPI](openapi/au10tix-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/au10tix.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/au10tix.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/au10tix)
- [Website](https://www.au10tix.com)
- [Documentation](https://www.au10tix.com/products/platform/)
- [Plans](plans/au10tix-plans-pricing.yml)
- [Rate Limits](rate-limits/au10tix-rate-limits.yml)
- [Fin Ops](finops/au10tix-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
