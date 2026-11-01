# Soracom

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Soracom is a global IoT cellular connectivity and platform provider headquartered in Tokyo, founded in 2014, with regional operations in the US (Soracom Global) and EU. The platform pairs multicarrier SIMs (physical, eSIM, iSIM) across 170+ countries with a deep platform of cloud integration services (Beam, Funnel, Funk), data services (Harvest, Lagoon, Query, Orbit), device management (Inventory, Krypton, Endorse, Napter), and network gateways (VPG / Canal / Direct / Door / Gate / Junction / Peek). Soracom exposes the entire stack through a coverage-aware REST API documented at users.soracom.io and maintained as a public OpenAPI 3.0 specification in the soracom-cli GitHub repo.

**Areas:** IoT · Cellular · LPWAN · SIM · LoRaWAN · Sigfox · MVNO · Connectivity · Edge · Japan

## Soracom on APIs.io

Everything profiled for Soracom is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/soracom/](https://apis.io/providers/soracom/)** — or go straight to one of the APIs or properties below.

### APIs (45)

- [Soracom SIM Management API](https://apis.io/apis/soracom/soracom-sim-api/) — Manage Soracom Air for Cellular SIMs (and Subscribers) — list, get, create Arc virtual SIMs, activate/deactivate/suspend/terminate, set group binding, set…
- [Soracom Group Configuration API](https://apis.io/apis/soracom/soracom-group-api/) — Manage Soracom groups and per-service configuration. Groups bind SIMs and devices to namespaced configuration for SoracomAir, SoracomBeam, SoracomFunnel,…
- [Soracom Billing API](https://apis.io/apis/soracom/soracom-billing-api/) — Retrieve usage charges (monthly bills, daily bill items, per-SIM and per-bill-item summaries), export bills to CSV, manage payment methods, register…
- [Soracom Stats and Diagnostics API](https://apis.io/apis/soracom/soracom-stats-api/) — Retrieve cellular data usage statistics (per SIM/subscriber/group/account), API and Napter audit logs, operator error logs, and diagnostic features.
- [Soracom Auth and Access Management API](https://apis.io/apis/soracom/soracom-auth-api/) — Authenticate operators (email/password or AuthKey), issue short-lived API Keys + Tokens, manage operator profile, SAM (Soracom Access Management) users and…
- [Soracom Lagoon API](https://apis.io/apis/soracom/soracom-lagoon-api/) — Manage Soracom Lagoon (managed Grafana) subscription, plan tier, organization, dashboards, users, licenses, and data sources.
- [Soracom Cloud Camera Services API](https://apis.io/apis/soracom/soracom-soracam-api/) — Manage Soracom Cloud Camera Services (SoraCam) devices, livestream URLs, image exports, recording exports, motion events, atomic timestamps, and dedicated…
- [Soracom Batch API](https://apis.io/apis/soracom/soracom-batch-api/) — Batch processing — create batch groups, define jobs that invoke API operations across many SIMs or devices, and inspect tasks for status and results.
- [Soracom Analysis API](https://apis.io/apis/soracom/soracom-analysis-api/) — [Soracom Query](/en/docs/query/)
- [Soracom API Sandbox: Coupon API](https://apis.io/apis/soracom/soracom-api-sandbox-coupon-api/) — The API Sandbox: Coupon API from Soracom — 1 operation(s) for api sandbox: coupon.
- [Soracom API Sandbox: Operator API](https://apis.io/apis/soracom/soracom-api-sandbox-operator-api/) — The API Sandbox: Operator API from Soracom — 3 operation(s) for api sandbox: operator.
- [Soracom API Sandbox: Order API](https://apis.io/apis/soracom/soracom-api-sandbox-order-api/) — The API Sandbox: Order API from Soracom — 1 operation(s) for api sandbox: order.
- [Soracom API Sandbox: Stats API](https://apis.io/apis/soracom/soracom-api-sandbox-stats-api/) — The API Sandbox: Stats API from Soracom — 2 operation(s) for api sandbox: stats.
- [Soracom API Sandbox: Subscriber API](https://apis.io/apis/soracom/soracom-api-sandbox-subscriber-api/) — The API Sandbox: Subscriber API from Soracom — 1 operation(s) for api sandbox: subscriber.
- [Soracom CellLocation API](https://apis.io/apis/soracom/soracom-celllocation-api/) — [Cell tower location information](/en/docs/air/get-location-info/#get-cell-tower-location-information)
- [Soracom Credential API](https://apis.io/apis/soracom/soracom-credential-api/) — [Credentials store](/en/docs/credentials-store/) Create, update, and delete credentials
- [Soracom DataEntry API](https://apis.io/apis/soracom/soracom-dataentry-api/) — [Soracom Harvest Data](/en/docs/harvest/)
- [Soracom Device API](https://apis.io/apis/soracom/soracom-device-api/) — [Soracom Inventory devices](/en/docs/inventory/)
- [Soracom DeviceObjectModel API](https://apis.io/apis/soracom/soracom-deviceobjectmodel-api/) — [Soracom Inventory object model](/en/docs/inventory/define-custom-object/)
- [Soracom Diagnostic API](https://apis.io/apis/soracom/soracom-diagnostic-api/) — [Diagnostic features](/en/guides/diagnostic/)
- [Soracom Email API](https://apis.io/apis/soracom/soracom-email-api/) — [Email addresses](/en/docs/email/)
- [Soracom FileEntry API](https://apis.io/apis/soracom/soracom-fileentry-api/) — [Soracom Harvest Files](/en/docs/harvest/)
- [Soracom Files API](https://apis.io/apis/soracom/soracom-files-api/) — Download files exported by the following APIs: - [Billing](#/Billing) - [Payment: exportPaymentStatement](#/Payment/exportPaymentStatement) -…
- [Soracom Gadget API](https://apis.io/apis/soracom/soracom-gadget-api/) — Gadget API compatible devices<ul><li>[SoraCam dedicated cellular pack](/en/guides/soracom-cloud-camera-services/setting-cellular-pack/)</li></ul>
- [Soracom Log API](https://apis.io/apis/soracom/soracom-log-api/) — Error logs
- [Soracom LoraDevice API](https://apis.io/apis/soracom/soracom-loradevice-api/) — [Soracom Air for LoRaWAN](/en/docs/air-for-lorawan/) devices
- [Soracom LoraGateway API](https://apis.io/apis/soracom/soracom-loragateway-api/) — [Soracom Air for LoRaWAN](/en/docs/air-for-lorawan/) gateways
- [Soracom LoraNetworkSet API](https://apis.io/apis/soracom/soracom-loranetworkset-api/) — [Soracom Air for LoRaWAN](/en/docs/air-for-lorawan/) network sets
- [Soracom Operator API](https://apis.io/apis/soracom/soracom-operator-api/) — - Operator management - Update registration information - Password changes - [Multi-factor authentication](/en/docs/mfa/)
- [Soracom Order API](https://apis.io/apis/soracom/soracom-order-api/) — - [Coupon codes](/en/guides/accounting/payment/register-coupon/) - [Long term discounts](/en/docs/air/volume-discount/) - Order management - Product catalog
- [Soracom Payment API](https://apis.io/apis/soracom/soracom-payment-api/) — - [Coupon codes](/en/guides/accounting/payment/register-coupon/) - [Usage charges (billing details)](/en/guides/accounting/check-usage/) - [Payment…
- [Soracom PortMapping API](https://apis.io/apis/soracom/soracom-portmapping-api/) — [Soracom Napter](/en/docs/napter/)
- [Soracom Query API](https://apis.io/apis/soracom/soracom-query-api/) — Search SIMs, Soracom Inventory devices, and Sigfox devices
- [Soracom ResourceSummary API](https://apis.io/apis/soracom/soracom-resourcesummary-api/) — The ResourceSummary API from Soracom — 1 operation(s) for resourcesummary.
- [Soracom Role API](https://apis.io/apis/soracom/soracom-role-api/) — [Access management (Soracom Access Management)](/en/docs/sam/)
- [Soracom SigfoxDevice API](https://apis.io/apis/soracom/soracom-sigfoxdevice-api/) — [Soracom Air for Sigfox](/en/docs/air-for-sigfox/) devices
- [Soracom SimProfileOrder API](https://apis.io/apis/soracom/soracom-simprofileorder-api/) — [eSIM profiles](/en/docs/air/provision-esim/)
- [Soracom Soralet API](https://apis.io/apis/soracom/soracom-soralet-api/) — [Soracom Orbit](/en/docs/orbit/) Soralet
- [Soracom Subscriber API](https://apis.io/apis/soracom/soracom-subscriber-api/) — [Soracom Air for Cellular](/en/docs/air/) SIM information, operations, and cancellation
- [Soracom SystemNotification API](https://apis.io/apis/soracom/soracom-systemnotification-api/) — [Email addresses](/en/docs/email/)
- [Soracom User API](https://apis.io/apis/soracom/soracom-user-api/) — - [Access management (Soracom Access Management)](/en/docs/sam/) - Password changes - [Multi-factor authentication](/en/docs/mfa/) - [Switch…
- [Soracom VirtualPrivateGateway API](https://apis.io/apis/soracom/soracom-virtualprivategateway-api/) — - [Virtual Private Gateway (VPG)](/en/docs/vpg/) (Canal / Direct / Door / Gate) - [Soracom Junction](/en/docs/junction/) - [Soracom Peek](/en/docs/peek/)
- [Soracom Audit Log API](https://apis.io/apis/soracom/soracom-audit-log-api/) — Audit logs
- [Soracom Event Handler API](https://apis.io/apis/soracom/soracom-event-handler-api/) — Event handlers
- [Soracom Shipping Address API](https://apis.io/apis/soracom/soracom-shipping-address-api/) — Shipping address operations for direct sales

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (11)

Multi-step workflows that chain operations into a business task.

- [Soracom Audit SIM Session Events](https://apis.io/arazzos/soracom/soracom-audit-sim-session-events-workflow/)
- [Soracom Collect SIM Harvest Data](https://apis.io/arazzos/soracom/soracom-collect-sim-harvest-data-workflow/)
- [Soracom Create Monthly Traffic Event Handler](https://apis.io/arazzos/soracom/soracom-create-traffic-event-handler-workflow/)
- [Soracom Deactivate IoT SIM with Guard](https://apis.io/arazzos/soracom/soracom-deactivate-sim-with-guard-workflow/)
- [Soracom Export Monthly Billing CSV](https://apis.io/arazzos/soracom/soracom-export-monthly-billing-workflow/)
- [Soracom Provision Group and Attach SIM](https://apis.io/arazzos/soracom/soracom-provision-group-and-attach-sim-workflow/)
- [Soracom Register and Activate IoT SIM](https://apis.io/arazzos/soracom/soracom-register-and-activate-sim-workflow/)
- [Soracom Register and Verify Coupon](https://apis.io/arazzos/soracom/soracom-register-and-verify-coupon-workflow/)
- [Soracom Register Inventory Device to Group](https://apis.io/arazzos/soracom/soracom-register-device-to-group-workflow/)
- [Soracom Register Subscriber to Group](https://apis.io/arazzos/soracom/soracom-register-subscriber-to-group-workflow/)
- [Soracom Send SMS to Active IoT SIM](https://apis.io/arazzos/soracom/soracom-send-sms-to-active-sim-workflow/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Soracom Agentic Access](https://apis.io/agentic-access/soracom/soracom-agentic-access/)

#### JSON Schema (5)

The data models the API reads and writes.

- [Soracom Harvest Data Entry](https://apis.io/schemas/soracom/soracom-data-entry/)
- [Soracom Inventory Device](https://apis.io/schemas/soracom/soracom-device/)
- [Soracom Group](https://apis.io/schemas/soracom/soracom-group/)
- [Soracom Napter Port Mapping](https://apis.io/schemas/soracom/soracom-port-mapping/)
- [Soracom SIM](https://apis.io/schemas/soracom/soracom-sim/)

#### JSON Structure (2)

Data models expressed in JSON Structure.

- [Soracom Device Structure](https://apis.io/json-structure/soracom/soracom-device-structure/)
- [Soracom Sim Structure](https://apis.io/json-structure/soracom/soracom-sim-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Soracom Context](https://apis.io/jsonld/soracom/soracom-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Soracom Vocabulary](https://apis.io/vocabularies/soracom/soracom-vocabulary/)

#### Examples (5)

Example requests and responses.

- [Soracom Auth Example](https://apis.io/examples/soracom/soracom-auth-example/)
- [Soracom Bill Latest Example](https://apis.io/examples/soracom/soracom-bill-latest-example/)
- [Soracom Harvest Data Example](https://apis.io/examples/soracom/soracom-harvest-data-example/)
- [Soracom Napter Create Example](https://apis.io/examples/soracom/soracom-napter-create-example/)
- [Soracom Sim List Example](https://apis.io/examples/soracom/soracom-sim-list-example/)

#### Collections (73)

Postman and Open Collection request collections.

- [Soracom and Query Analysis API](https://apis.io/collections/soracom/open-soracom-analysis-api/)
- [Soracom Analysis and Query API](https://apis.io/collections/soracom/open-soracom-analysis-query-api/)
- [Soracom and Query Analysis API Sandbox: Coupon API](https://apis.io/collections/soracom/open-soracom-api-sandbox-coupon-api/)
- [Soracom and Query Analysis API Sandbox: Operator API](https://apis.io/collections/soracom/open-soracom-api-sandbox-operator-api/)
- [Soracom and Query Analysis API Sandbox: Order API](https://apis.io/collections/soracom/open-soracom-api-sandbox-order-api/)
- [Soracom and Query Analysis API Sandbox: Stats API](https://apis.io/collections/soracom/open-soracom-api-sandbox-stats-api/)
- [Soracom and Query Analysis API Sandbox: Subscriber API](https://apis.io/collections/soracom/open-soracom-api-sandbox-subscriber-api/)
- [Soracom and Query Analysis AuditLog API](https://apis.io/collections/soracom/open-soracom-auditlog-api/)
- [Soracom and Query Analysis Auth API](https://apis.io/collections/soracom/open-soracom-auth-api/)
- [Soracom and Query Analysis Batch API](https://apis.io/collections/soracom/open-soracom-batch-api/)
- [Soracom and Query Analysis Billing API](https://apis.io/collections/soracom/open-soracom-billing-api/)
- [Soracom and Query Analysis CellLocation API](https://apis.io/collections/soracom/open-soracom-celllocation-api/)
- [Soracom and Query Analysis Credential API](https://apis.io/collections/soracom/open-soracom-credential-api/)
- [Soracom and Query Analysis DataEntry API](https://apis.io/collections/soracom/open-soracom-dataentry-api/)
- [Soracom and Query Analysis Device API](https://apis.io/collections/soracom/open-soracom-device-api/)
- [Soracom and Query Analysis DeviceObjectModel API](https://apis.io/collections/soracom/open-soracom-deviceobjectmodel-api/)
- [Soracom and Query Analysis Diagnostic API](https://apis.io/collections/soracom/open-soracom-diagnostic-api/)
- [Soracom and Query Analysis Email API](https://apis.io/collections/soracom/open-soracom-email-api/)
- [Soracom Event Handler API](https://apis.io/collections/soracom/open-soracom-event-handler-api/)
- [Soracom and Query Analysis EventHandler API](https://apis.io/collections/soracom/open-soracom-eventhandler-api/)
- [Soracom and Query Analysis FileEntry API](https://apis.io/collections/soracom/open-soracom-fileentry-api/)
- [Soracom and Query Analysis Files API](https://apis.io/collections/soracom/open-soracom-files-api/)
- [Soracom and Query Analysis Gadget API](https://apis.io/collections/soracom/open-soracom-gadget-api/)
- [Soracom and Query Analysis Group API](https://apis.io/collections/soracom/open-soracom-group-api/)
- [Soracom Harvest API](https://apis.io/collections/soracom/open-soracom-harvest-api/)
- …and 48 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Soracom — jsonschema rules](https://apis.io/rules/soracom/soracom-jsonschema-spectral-rules/)
- [Soracom API Rules](https://apis.io/rules/soracom/soracom-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Soracom Authentication](https://apis.io/security/soracom/soracom-authentication/)
- [Soracom Domain Security](https://apis.io/security/soracom/soracom-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Soracom Plans Pricing](https://apis.io/plans/soracom/soracom-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Soracom Rate Limits](https://apis.io/rate-limits/soracom/soracom-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Soracom Finops](https://apis.io/finops/soracom/soracom-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.soracom.io/)
- [Documentation](https://developers.soracom.io/en/)
- [Getting started](https://developers.soracom.io/en/start/)
- [Pricing](https://www.soracom.io/pricing/)
- [Support](https://support.soracom.io)
- [Changelog](https://changelog.soracom.io/)
- [Blog](https://soracom.io/blog/)
- [Terms of service](https://www.soracom.io/terms_of_service/)
- [Privacy policy](https://www.soracom.io/privacy_policy/)
- [GitHub](https://github.com/soracom)
- [Status](https://status.soracom.io/)

## API Evangelist rating

**Kin Score 51.5** — developing · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 72.3 |
| Contract quality | 61.4 |
| Contract governance | 27.3 |
| Operational transparency | 18.4 |
| Developer ergonomics | 75.0 |
| Access clarity | 32.9 |

**Agent readiness 30.1** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 14.2** — Telecommunications

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/soracom/](https://apis.io/providers/soracom/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Soracom: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/soracom/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
