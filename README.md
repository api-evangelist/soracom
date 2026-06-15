# Soracom (soracom)

Soracom is a global IoT cellular connectivity and platform provider headquartered in Tokyo, founded in 2014, with regional operations in the US (Soracom Global) and EU. The platform pairs multicarrier SIMs (physical, eSIM, iSIM) across 170+ countries with a deep platform of cloud integration services (Beam, Funnel, Funk), data services (Harvest, Lagoon, Query, Orbit), device management (Inventory, Krypton, Endorse, Napter), and network gateways (VPG / Canal / Direct / Door / Gate / Junction / Peek). Soracom exposes the entire stack through a coverage-aware REST API documented at users.soracom.io and maintained as a public OpenAPI 3.0 specification in the soracom-cli GitHub repo.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/apis.yml)

## Scope

- **Position:** Provider

## Tags

- IoT
- Cellular
- LPWAN
- SIM
- LoRaWAN
- Sigfox
- MVNO
- Connectivity
- Edge
- Japan

## Timestamps

- **Created:** 2026-05-25T00:00:00.000Z
- **Modified:** 2026-05-25

## APIs

### Soracom SIM Management API

Manage Soracom Air for Cellular SIMs (and Subscribers) — list, get, create Arc virtual SIMs, activate/deactivate/suspend/terminate, set group binding, set IMEI lock, view session events, manage SIM profiles for multi-IMSI eSIM, and read cell-tower location info.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Sim](https://users.soracom.io/ja-jp/tools/api/reference/#/Sim)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Cellular
- SIM
- Subscriber

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/air/)
- [Documentation](https://users.soracom.io/ja-jp/tools/api/reference/#/Sim)
- [OpenAPI](openapi/soracom-sim-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-sim-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-sim-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/soracom-sim-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/soracom-sim-structure.json)
- [Examples](examples/soracom-sim-list-example.json)

### Soracom Group Configuration API

Manage Soracom groups and per-service configuration. Groups bind SIMs and devices to namespaced configuration for SoracomAir, SoracomBeam, SoracomFunnel, SoracomFunk, SoracomHarvest, SoracomJunction, SoracomOrbit, and metadata services.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Group](https://users.soracom.io/ja-jp/tools/api/reference/#/Group)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Groups
- Configuration

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/group-configuration/)
- [OpenAPI](openapi/soracom-group-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-group-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-group-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/soracom-group-schema.json) — [JSON Schema](https://json-schema.org/specification)

### Soracom Harvest API

Soracom Harvest is a managed time-series and file store for IoT device payloads. The API retrieves data entries by Subscriber/Device/SigfoxDevice/LoraDevice, lists indexed resources, and uploads/downloads binary Harvest Files.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/DataEntry](https://users.soracom.io/ja-jp/tools/api/reference/#/DataEntry)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Harvest
- Data
- Telemetry
- Files

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/harvest/)
- [OpenAPI](openapi/soracom-harvest-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-harvest-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-harvest-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/soracom-data-entry-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Examples](examples/soracom-harvest-data-example.json)

### Soracom Inventory API

Soracom Inventory provides LwM2M-based registration, object models, resource read/write, observe/notify subscriptions, and remote execution against IoT devices.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Device](https://users.soracom.io/ja-jp/tools/api/reference/#/Device)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- LwM2M
- Devices
- Inventory

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/inventory/)
- [OpenAPI](openapi/soracom-inventory-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-inventory-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-inventory-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/soracom-device-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/soracom-device-structure.json)

### Soracom Napter API

Soracom Napter creates on-demand TCP port mappings (with optional TLS) that allow a defined source CIDR to reach a SIM-attached device's TCP port for SSH, HTTP(S), VNC, or RDP-style remote access, auditable in audit_logs/napter.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/PortMapping](https://users.soracom.io/ja-jp/tools/api/reference/#/PortMapping)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Remote Access
- Napter
- Security

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/napter/)
- [OpenAPI](openapi/soracom-napter-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-napter-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-napter-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/soracom-port-mapping-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Examples](examples/soracom-napter-create-example.json)

### Soracom Event Handler API

Configure event handlers (rules + actions) on SIM, data, and billing events; manage the Credentials Store; and deploy Orbit Soralets (WebAssembly inline payload transforms).

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/EventHandler](https://users.soracom.io/ja-jp/tools/api/reference/#/EventHandler)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Automation
- Event Handler
- Soralet
- Credentials

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/event-handler/)
- [OpenAPI](openapi/soracom-event-handler-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-event-handler-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-event-handler-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Virtual Private Gateway API

Provision and manage Soracom Virtual Private Gateways (VPG) including Canal (AWS VPC peering), Direct (AWS Direct Connect), Door (IPSec VPN), Gate (reverse-NAT), Junction (packet rules), and Peek (packet capture).

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/VirtualPrivateGateway](https://users.soracom.io/ja-jp/tools/api/reference/#/VirtualPrivateGateway)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Networking
- VPG
- Canal
- Door
- Gate
- Junction
- Peek

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/vpg/)
- [OpenAPI](openapi/soracom-vpg-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-vpg-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-vpg-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Billing API

Retrieve usage charges (monthly bills, daily bill items, per-SIM and per-bill-item summaries), export bills to CSV, manage payment methods, register coupons, manage orders, and configure shipping addresses.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Billing](https://users.soracom.io/ja-jp/tools/api/reference/#/Billing)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Billing
- FinOps
- Payment
- Coupons
- Orders

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/reference/fees/)
- [OpenAPI](openapi/soracom-billing-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-billing-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-billing-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Examples](examples/soracom-bill-latest-example.json)

### Soracom Stats and Diagnostics API

Retrieve cellular data usage statistics (per SIM/subscriber/group/account), API and Napter audit logs, operator error logs, and diagnostic features.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Stats](https://users.soracom.io/ja-jp/tools/api/reference/#/Stats)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Stats
- Audit
- Diagnostics
- Observability

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/air/view-data-usage/)
- [OpenAPI](openapi/soracom-stats-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-stats-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-stats-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Auth and Access Management API

Authenticate operators (email/password or AuthKey), issue short-lived API Keys + Tokens, manage operator profile, SAM (Soracom Access Management) users and roles, MFA settings, registered email addresses, switch-user (cross-operator) flows, and system notifications.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Auth](https://users.soracom.io/ja-jp/tools/api/reference/#/Auth)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Auth
- SAM
- Access Management
- MFA
- Users
- Roles

#### Properties

- [Documentation](https://developers.soracom.io/en/tools/api/key-and-token/)
- [Documentation](https://developers.soracom.io/en/docs/sam/)
- [OpenAPI](openapi/soracom-auth-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-auth-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-auth-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Examples](examples/soracom-auth-example.json)

### Soracom Analysis and Query API

Asynchronous SQL query execution over Soracom Query tables (SIM_SESSION_EVENTS, SIM_LOCATIONS, BILLING, and more) and search across SIMs, Inventory devices, and Sigfox devices.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Analysis](https://users.soracom.io/ja-jp/tools/api/reference/#/Analysis)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Query
- Analysis
- SQL
- Search

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/query/)
- [OpenAPI](openapi/soracom-analysis-query-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-analysis-query-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-analysis-query-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Lagoon API

Manage Soracom Lagoon (managed Grafana) subscription, plan tier, organization, dashboards, users, licenses, and data sources.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Lagoon](https://users.soracom.io/ja-jp/tools/api/reference/#/Lagoon)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Lagoon
- Dashboards
- Visualization

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/lagoon-v3/)
- [OpenAPI](openapi/soracom-lagoon-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-lagoon-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-lagoon-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Air for LoRaWAN API

Manage Soracom Air for LoRaWAN — devices, gateways, network sets, session keys, and group binding for LoRaWAN deployments.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/LoraDevice](https://users.soracom.io/ja-jp/tools/api/reference/#/LoraDevice)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- LoRaWAN
- LPWAN
- Devices
- Gateways

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/air-for-lorawan/)
- [OpenAPI](openapi/soracom-lorawan-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-lorawan-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-lorawan-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Air for Sigfox API

Manage Soracom Air for Sigfox devices.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/SigfoxDevice](https://users.soracom.io/ja-jp/tools/api/reference/#/SigfoxDevice)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Sigfox
- LPWAN
- Devices

#### Properties

- [Documentation](https://developers.soracom.io/en/docs/air-for-sigfox/)
- [OpenAPI](openapi/soracom-sigfox-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-sigfox-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-sigfox-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Cloud Camera Services API

Manage Soracom Cloud Camera Services (SoraCam) devices, livestream URLs, image exports, recording exports, motion events, atomic timestamps, and dedicated cellular pack provisioning.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/SoraCam](https://users.soracom.io/ja-jp/tools/api/reference/#/SoraCam)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- SoraCam
- Camera
- Video

#### Properties

- [Documentation](https://developers.soracom.io/en/guides/soracom-cloud-camera-services/)
- [OpenAPI](openapi/soracom-soracam-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-soracam-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-soracam-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Batch API

Batch processing — create batch groups, define jobs that invoke API operations across many SIMs or devices, and inspect tasks for status and results.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/#/Batch](https://users.soracom.io/ja-jp/tools/api/reference/#/Batch)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Batch
- Automation

#### Properties

- [OpenAPI](openapi/soracom-batch-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-batch-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-batch-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Soracom Platform API (Aggregate)

The full monolithic Soracom Platform OpenAPI spec — 487 operations across 40 tags covering every Soracom service surface (Sim, Subscriber, Group, Harvest, Inventory, Napter, EventHandler, VPG, Billing, Auth, Query, Lagoon, LoRaWAN, Sigfox, SoraCam, Batch). Source of truth maintained in the soracom-cli repo.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/reference/](https://users.soracom.io/ja-jp/tools/api/reference/)
- **Base URL:** `https://api.soracom.io/v1`

#### Tags

- IoT
- Platform
- Aggregate

#### Properties

- [Documentation](https://users.soracom.io/ja-jp/tools/api/reference/)
- [OpenAPI](openapi/soracom-platform-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-platform-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-platform-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/soracom-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Soracom Sandbox API

Soracom Sandbox API for safely exercising platform workflows. Lets developers create test coupons, fake SIMs, and dummy subscriber records, then run normal API calls against the sandbox endpoint without billing.

- **Human URL:** [https://users.soracom.io/ja-jp/tools/api/sandbox/](https://users.soracom.io/ja-jp/tools/api/sandbox/)
- **Base URL:** `https://api-sandbox.soracom.io/v1`

#### Tags

- IoT
- Sandbox
- Testing

#### Properties

- [OpenAPI](openapi/soracom-sandbox-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/soracom-sandbox-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/soracom-sandbox-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.soracom.io)
- [Documentation](https://developers.soracom.io/en/)
- [Documentation](https://users.soracom.io/ja-jp/tools/api/reference/)
- [Getting Started](https://developers.soracom.io/en/start/)
- [Sign Up](https://console.soracom.io/#/signup)
- [Login](https://console.soracom.io)
- [Pricing](https://www.soracom.io/pricing/)
- [Pricing](https://developers.soracom.io/en/docs/reference/fees/)
- [Status Page](https://status.soracom.io/)
- [Blog](https://soracom.io/blog/)
- [Changelog](https://changelog.soracom.io/)
- [Press](https://www.soracom.io/press-releases/)
- [Terms of Service](https://www.soracom.io/terms_of_service/)
- [Privacy Policy](https://www.soracom.io/privacy_policy/)
- [Support](https://support.soracom.io)
- [Contact](https://www.soracom.io/contact/)
- [Forum](https://discuss.soracom.io)
- [Coverage](https://www.soracom.io/pricing/countries/)
- [Documentation](https://developers.soracom.io/en/docs/air/sim-types/)
- [Documentation](https://developers.soracom.io/en/tools/api/endpoints/)
- [Documentation](https://developers.soracom.io/en/tools/api/key-and-token/)
- [Documentation](https://developers.soracom.io/en/tools/api/how-to-read-api-reference/)
- [GitHub Organization](https://github.com/soracom)
- [GitHub Organization](https://github.com/soracom-labs)
- [C L I](https://github.com/soracom/soracom-cli)
- [SDK](https://github.com/soracom/soracom-sdk-go)
- [SDK](https://github.com/soracom/soracom-sdk-ruby)
- [SDK](https://github.com/soracom/soracom-sdk-swift)
- [SDK](https://github.com/soracom/soracom-inventory-agent-for-java)
- [SDK](https://github.com/soracom/krypton-client-go)
- [SDK](https://github.com/soracom/endorse-client-go)
- [SDK](https://github.com/soracom/soracom-krypton-client-for-java)
- [SDK](https://github.com/soracom/soracom-endorse-client-for-java)
- [Tool](https://github.com/soracom/soratun)
- [Tool](https://github.com/soracom/soraql)
- [Tool](https://github.com/soracom/homebrew-soracom-cli)
- [Tool](https://github.com/soracom/multus-multivpc-cni)
- [Tool](https://github.com/soracom/orbit-sdk-rust)
- [Tool](https://github.com/soracom/orbit-sdk-tinygo)
- [Tool](https://github.com/soracom/orbit-sdk-c)
- [Tool](https://github.com/soracom/orbit-sdk-assemblyscript)
- [Code Examples](https://github.com/soracom/handson)
- [Library](https://github.com/soracom/SORACOM-LoRaWAN)
- [Documentation](https://developers.soracom.io/en/start/)
- [Documentation](https://developers.soracom.io/en/docs/air/)
- [Documentation](https://developers.soracom.io/en/docs/beam/)
- [Documentation](https://developers.soracom.io/en/docs/funnel/)
- [Documentation](https://developers.soracom.io/en/docs/funk/)
- [Documentation](https://developers.soracom.io/en/docs/harvest/)
- [Documentation](https://developers.soracom.io/en/docs/lagoon-v3/)
- [Documentation](https://developers.soracom.io/en/docs/inventory/)
- [Documentation](https://developers.soracom.io/en/docs/napter/)
- [Documentation](https://developers.soracom.io/en/docs/orbit/)
- [Documentation](https://developers.soracom.io/en/docs/vpg/)
- [Documentation](https://developers.soracom.io/en/docs/sam/)
- [Documentation](https://developers.soracom.io/en/docs/event-handler/)
- [Documentation](https://developers.soracom.io/en/docs/query/)
- [Documentation](https://developers.soracom.io/en/docs/credentials-store/)
- [Coverage](https://developers.soracom.io/en/docs/air/speed-class/)
- [Plans](plans/soracom-plans-pricing.yml)
- [Rate Limits](rate-limits/soracom-rate-limits.yml)
- [Fin Ops](finops/soracom-finops.yml)
- [Vocabulary](vocabulary/soracom-vocabulary.yml)
- [Spectral Rules](rules/soracom-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
