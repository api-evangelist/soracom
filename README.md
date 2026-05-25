# Soracom (soracom)

Soracom is a global IoT cellular connectivity and platform provider headquartered in Tokyo, founded in 2014, with regional operations in the US (Soracom Global) and EU. The platform pairs multicarrier SIMs (physical, eSIM, iSIM) across 170+ countries with a deep platform of cloud integration services (Beam, Funnel, Funk), data services (Harvest, Lagoon, Query, Orbit), device management (Inventory, Krypton, Endorse, Napter), and network gateways (VPG / Canal / Direct / Door / Gate / Junction / Peek).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/soracom/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- IoT, Cellular, LPWAN, SIM, LoRaWAN, Sigfox, MVNO, Connectivity, Edge, Japan

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## Coverage and Endpoints

Soracom exposes coverage-aware API endpoints. Pick the one matching the SIM/resource coverage:

| Coverage | Base URL |
|---|---|
| Japan | `https://api.soracom.io/v1` (alias `https://jp.api.soracom.io/v1`) |
| Global | `https://g.api.soracom.io/v1` |
| Sandbox | `https://api-sandbox.soracom.io/v1` |

Authenticate via `POST /v1/auth` (email + password, or `authKeyId` + `authKey`) and present the issued short-lived `X-Soracom-API-Key` and `X-Soracom-Token` headers on subsequent calls.

## APIs

### Soracom SIM Management API
Manage Soracom Air for Cellular SIMs (and Subscribers) — list, get, create Arc virtual SIMs, activate/deactivate/suspend/terminate, set group binding, set IMEI lock, view session events, manage SIM profiles for multi-IMSI eSIM, and read cell-tower location info.

**Human URL:** [Soracom API Reference — Sim](https://users.soracom.io/ja-jp/tools/api/reference/#/Sim)

- [Documentation — Soracom Air](https://developers.soracom.io/en/docs/air/)
- [OpenAPI](openapi/soracom-sim-api-openapi.yml)
- [JSON Schema — SIM](json-schema/soracom-sim-schema.json)
- [JSON Structure — SIM](json-structure/soracom-sim-structure.json)
- [Example — list SIMs](examples/soracom-sim-list-example.json)
- [Naftiko Capability — SIM Management](capabilities/sim-management.yaml)

### Soracom Group Configuration API
Manage Soracom groups and per-service configuration. Groups bind SIMs and devices to namespaced configuration for SoracomAir, SoracomBeam, SoracomFunnel, SoracomFunk, SoracomHarvest, SoracomJunction, SoracomOrbit, and metadata services.

**Human URL:** [Soracom API Reference — Group](https://users.soracom.io/ja-jp/tools/api/reference/#/Group)

- [Documentation — Group Configuration](https://developers.soracom.io/en/docs/group-configuration/)
- [OpenAPI](openapi/soracom-group-api-openapi.yml)
- [JSON Schema — Group](json-schema/soracom-group-schema.json)
- [Naftiko Capability — Group Configuration](capabilities/group-configuration.yaml)

### Soracom Harvest API
Soracom Harvest is a managed time-series and file store for IoT device payloads. The API retrieves data entries by Subscriber/Device/SigfoxDevice/LoraDevice, lists indexed resources, and uploads/downloads binary Harvest Files.

**Human URL:** [Soracom API Reference — DataEntry](https://users.soracom.io/ja-jp/tools/api/reference/#/DataEntry)

- [Documentation — Harvest](https://developers.soracom.io/en/docs/harvest/)
- [OpenAPI](openapi/soracom-harvest-api-openapi.yml)
- [JSON Schema — Data Entry](json-schema/soracom-data-entry-schema.json)
- [Example — Harvest data](examples/soracom-harvest-data-example.json)
- [Naftiko Capability — Harvest Data](capabilities/harvest-data.yaml)

### Soracom Inventory API
LwM2M-based device registration, object models, resource read/write, observe/notify subscriptions, and remote execution against IoT devices.

**Human URL:** [Soracom API Reference — Device](https://users.soracom.io/ja-jp/tools/api/reference/#/Device)

- [Documentation — Inventory](https://developers.soracom.io/en/docs/inventory/)
- [OpenAPI](openapi/soracom-inventory-api-openapi.yml)
- [JSON Schema — Device](json-schema/soracom-device-schema.json)
- [JSON Structure — Device](json-structure/soracom-device-structure.json)
- [Naftiko Capability — Inventory Devices](capabilities/inventory-devices.yaml)

### Soracom Napter API
On-demand TCP port mappings (with optional TLS) that allow a defined source CIDR to reach a SIM-attached device's TCP port for SSH, HTTP(S), VNC, or RDP-style remote access, auditable in `audit_logs/napter`.

**Human URL:** [Soracom API Reference — PortMapping](https://users.soracom.io/ja-jp/tools/api/reference/#/PortMapping)

- [Documentation — Napter](https://developers.soracom.io/en/docs/napter/)
- [OpenAPI](openapi/soracom-napter-api-openapi.yml)
- [JSON Schema — Port Mapping](json-schema/soracom-port-mapping-schema.json)
- [Example — create Napter mapping](examples/soracom-napter-create-example.json)
- [Naftiko Capability — Napter Port Mappings](capabilities/napter-portmappings.yaml)

### Soracom Event Handler API
Configure event handlers (rules + actions) on SIM, data, and billing events; manage the Credentials Store; and deploy Orbit Soralets (WebAssembly inline payload transforms).

**Human URL:** [Soracom API Reference — EventHandler](https://users.soracom.io/ja-jp/tools/api/reference/#/EventHandler)

- [Documentation — Event Handler](https://developers.soracom.io/en/docs/event-handler/)
- [OpenAPI](openapi/soracom-event-handler-api-openapi.yml)
- [Naftiko Capability — Event Handler](capabilities/event-handler.yaml)

### Soracom Virtual Private Gateway API
Provision and manage Soracom Virtual Private Gateways (VPG) including Canal (AWS VPC peering), Direct (AWS Direct Connect), Door (IPSec VPN), Gate (reverse-NAT), Junction (packet rules), and Peek (packet capture).

**Human URL:** [Soracom API Reference — VirtualPrivateGateway](https://users.soracom.io/ja-jp/tools/api/reference/#/VirtualPrivateGateway)

- [Documentation — VPG](https://developers.soracom.io/en/docs/vpg/)
- [OpenAPI](openapi/soracom-vpg-api-openapi.yml)
- [Naftiko Capability — VPG Management](capabilities/vpg-management.yaml)

### Soracom Billing API
Retrieve usage charges (monthly bills, daily bill items, per-SIM and per-bill-item summaries), export bills to CSV, manage payment methods, register coupons, manage orders, and configure shipping addresses.

**Human URL:** [Soracom API Reference — Billing](https://users.soracom.io/ja-jp/tools/api/reference/#/Billing)

- [Documentation — Pricing & Fee Schedule](https://developers.soracom.io/en/docs/reference/fees/)
- [OpenAPI](openapi/soracom-billing-api-openapi.yml)
- [Example — latest bill](examples/soracom-bill-latest-example.json)
- [Naftiko Capability — Billing](capabilities/billing.yaml)

### Soracom Stats and Diagnostics API
Cellular data usage statistics (per SIM/subscriber/group/account), API and Napter audit logs, operator error logs, and diagnostic features.

**Human URL:** [Soracom API Reference — Stats](https://users.soracom.io/ja-jp/tools/api/reference/#/Stats)

- [Documentation — View Data Usage](https://developers.soracom.io/en/docs/air/view-data-usage/)
- [OpenAPI](openapi/soracom-stats-api-openapi.yml)
- [Naftiko Capability — Stats and Diagnostics](capabilities/stats-diagnostics.yaml)

### Soracom Auth and Access Management API
Authenticate operators (email/password or AuthKey), issue short-lived API Keys + Tokens, manage operator profile, SAM (Soracom Access Management) users and roles, MFA settings, registered email addresses, switch-user (cross-operator) flows, and system notifications.

**Human URL:** [Soracom API Reference — Auth](https://users.soracom.io/ja-jp/tools/api/reference/#/Auth)

- [Documentation — Generate API Key and Token](https://developers.soracom.io/en/tools/api/key-and-token/)
- [Documentation — Access Management (SAM)](https://developers.soracom.io/en/docs/sam/)
- [OpenAPI](openapi/soracom-auth-api-openapi.yml)
- [Example — authenticate](examples/soracom-auth-example.json)
- [Naftiko Capability — Auth and Access Management](capabilities/auth-access.yaml)

### Soracom Analysis and Query API
Asynchronous SQL query execution over Soracom Query tables (`SIM_SESSION_EVENTS`, `SIM_LOCATIONS`, `BILLING`, and more) and search across SIMs, Inventory devices, and Sigfox devices.

**Human URL:** [Soracom API Reference — Analysis](https://users.soracom.io/ja-jp/tools/api/reference/#/Analysis)

- [Documentation — Query](https://developers.soracom.io/en/docs/query/)
- [OpenAPI](openapi/soracom-analysis-query-api-openapi.yml)
- [Naftiko Capability — Analysis and Query](capabilities/analysis-query.yaml)

### Soracom Lagoon API
Manage Soracom Lagoon (managed Grafana) subscription, plan tier, organization, dashboards, users, licenses, and data sources.

**Human URL:** [Soracom API Reference — Lagoon](https://users.soracom.io/ja-jp/tools/api/reference/#/Lagoon)

- [Documentation — Lagoon v3](https://developers.soracom.io/en/docs/lagoon-v3/)
- [OpenAPI](openapi/soracom-lagoon-api-openapi.yml)
- [Naftiko Capability — Lagoon Dashboards](capabilities/lagoon-dashboards.yaml)

### Soracom Air for LoRaWAN API
Manage Soracom Air for LoRaWAN — devices, gateways, network sets, session keys, and group binding for LoRaWAN deployments.

**Human URL:** [Soracom API Reference — LoraDevice](https://users.soracom.io/ja-jp/tools/api/reference/#/LoraDevice)

- [Documentation — Air for LoRaWAN](https://developers.soracom.io/en/docs/air-for-lorawan/)
- [OpenAPI](openapi/soracom-lorawan-api-openapi.yml)
- [Naftiko Capability — LoRaWAN Devices](capabilities/lorawan-devices.yaml)

### Soracom Air for Sigfox API
Manage Soracom Air for Sigfox devices.

**Human URL:** [Soracom API Reference — SigfoxDevice](https://users.soracom.io/ja-jp/tools/api/reference/#/SigfoxDevice)

- [Documentation — Air for Sigfox](https://developers.soracom.io/en/docs/air-for-sigfox/)
- [OpenAPI](openapi/soracom-sigfox-api-openapi.yml)
- [Naftiko Capability — Sigfox Devices](capabilities/sigfox-devices.yaml)

### Soracom Cloud Camera Services API
Manage Soracom Cloud Camera Services (SoraCam) devices, livestream URLs, image exports, recording exports, motion events, atomic timestamps, and dedicated cellular pack provisioning.

**Human URL:** [Soracom API Reference — SoraCam](https://users.soracom.io/ja-jp/tools/api/reference/#/SoraCam)

- [Documentation — Cloud Camera Services](https://developers.soracom.io/en/guides/soracom-cloud-camera-services/)
- [OpenAPI](openapi/soracom-soracam-api-openapi.yml)
- [Naftiko Capability — SoraCam](capabilities/soracam.yaml)

### Soracom Batch API
Batch processing — create batch groups, define jobs that invoke API operations across many SIMs or devices, and inspect tasks for status and results.

**Human URL:** [Soracom API Reference — Batch](https://users.soracom.io/ja-jp/tools/api/reference/#/Batch)

- [OpenAPI](openapi/soracom-batch-api-openapi.yml)
- [Naftiko Capability — Batch Jobs](capabilities/batch-jobs.yaml)

### Soracom Platform API (Aggregate)
The full monolithic Soracom Platform OpenAPI spec — 487 operations across 40 tags covering every Soracom service surface (Sim, Subscriber, Group, Harvest, Inventory, Napter, EventHandler, VPG, Billing, Auth, Query, Lagoon, LoRaWAN, Sigfox, SoraCam, Batch). Source of truth maintained in the `soracom-cli` repo at `generators/assets/soracom-api.en.yaml`.

- [Interactive API Reference](https://users.soracom.io/ja-jp/tools/api/reference/)
- [OpenAPI](openapi/soracom-platform-api-openapi.yml)
- [JSON-LD context](json-ld/soracom-context.jsonld)

### Soracom Sandbox API
Sandbox API for safely exercising platform workflows. Lets developers create test coupons, fake SIMs, and dummy subscriber records, then run normal API calls against the sandbox endpoint without billing.

- [OpenAPI](openapi/soracom-sandbox-api-openapi.yml)

## SDKs, CLIs, and Tools

- [soracom CLI](https://github.com/soracom/soracom-cli) — Go CLI auto-generated from the OpenAPI spec
- [soracom-sdk-go](https://github.com/soracom/soracom-sdk-go) — Go SDK
- [soracom-sdk-ruby](https://github.com/soracom/soracom-sdk-ruby) — Ruby gem
- [soracom-inventory-agent-for-java](https://github.com/soracom/soracom-inventory-agent-for-java) — Java LwM2M Inventory agent
- [krypton-client-go](https://github.com/soracom/krypton-client-go) — Krypton client (Go)
- [endorse-client-go](https://github.com/soracom/endorse-client-go) — Endorse client (Go)
- [soracom-krypton-client-for-java](https://github.com/soracom/soracom-krypton-client-for-java) — Krypton client (Java)
- [soracom-endorse-client-for-java](https://github.com/soracom/soracom-endorse-client-for-java) — Endorse client (Java)
- [soratun](https://github.com/soracom/soratun) — Wireguard-based Arc client
- [soraql](https://github.com/soracom/soraql) — Soracom Query CLI
- [orbit-sdk-rust](https://github.com/soracom/orbit-sdk-rust), [orbit-sdk-tinygo](https://github.com/soracom/orbit-sdk-tinygo), [orbit-sdk-c](https://github.com/soracom/orbit-sdk-c), [orbit-sdk-assemblyscript](https://github.com/soracom/orbit-sdk-assemblyscript) — Orbit Soralet SDKs
- [SORACOM-LoRaWAN](https://github.com/soracom/SORACOM-LoRaWAN) — Arduino library
- [multus-multivpc-cni](https://github.com/soracom/multus-multivpc-cni) — EKS multi-VPC CNI

## Plans, Rate Limits, and FinOps

- [Plans and pricing](plans/soracom-plans-pricing.yml) — API Commons Plans 0.1
- [Rate limits](rate-limits/soracom-rate-limits.yml) — API Commons Rate Limits 0.1
- [FinOps](finops/soracom-finops.yml) — FOCUS-aligned FinOps definition
- [Vocabulary](vocabulary/soracom-vocabulary.yml)
- [Spectral rules](rules/soracom-rules.yml)

## Resources

- [Developer portal](https://developers.soracom.io/en/)
- [Interactive API reference](https://users.soracom.io/ja-jp/tools/api/reference/)
- [Pricing & fee schedule](https://developers.soracom.io/en/docs/reference/fees/)
- [Status page](https://status.soracom.io/)
- [Changelog](https://changelog.soracom.io/)
- [GitHub organization](https://github.com/soracom)
- [Soracom Labs (samples)](https://github.com/soracom-labs)
