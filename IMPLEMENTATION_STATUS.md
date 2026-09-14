# Implementation status

Snapshot: 14 Sep 2026. Exact development baseline and source checks are recorded in
[SOURCE.md](https://github.com/ApoCert-it/secure-integration-platform/blob/main/SOURCE.md). This is a source technical preview, not a production release.

<a id="product-status"></a>

## Included capabilities

| Surface | Available functionality | Qualification limits |
|---|---|---|
| Core Gateway | Installation authentication, operation grants, immutable Published configuration, restricted transport, provider capabilities and PostgreSQL persistence. | Synthetic evaluation and automated tests do not qualify every external protocol or production deployment. |
| Local Core pilot | Docker-first Direct client → Gateway → Published Connector → synthetic HTTPS/mTLS service. | No host .NET SDK, Node or curl needed for this path. It does not exercise the Windows Service or an external vendor. |
| Windows Local Broker | Authenticated Named Pipe SDK, installation identity, local key protection, credential adoption, service lifecycle and named-application registration/inspection/update/revocation. | Real-service and standard-account observations are scoped to the software and environments in the Local Broker guide; no universal Windows, MSI, COM or disaster-recovery claim. |
| Admin | Guided onboarding with searchable paged catalogs, stable identifiers, Active-enrollment readiness, distinct-role approval, exact-revision publication, responsive UI and embedded guidance. | Real Admin API/PostgreSQL lookup among 10,000 synthetic tenants is a correctness test, not a capacity benchmark; authentication and role configuration remain deployment responsibilities. |
| Audit | Metadata-only events, append-only application privileges and tenant-scoped bounded export with UTC interval and keyset pagination. | Does not prevent database-administrator access or establish regulatory conformity. |
| Package preflight | Expected source commit and manifest SHA-256 checked before Broker install/update effects. | Integrity against trusted expected values is not artifact signing or publisher authentication. |
| Optional providers | Azure and local PKCS#12 implementations outside the Core. | Identity permissions, custody, recovery and network configuration depend on the deployment. |
| FSE2 current-spec | Fourteen route contracts and supported provisioning, including durable validation/publication correlations. | Offline qualification within the frozen specification; not fourteen live-qualified routes. |
| FSE2 CDA VERIFICA | Observed OfficialTest validation success with workflow and trace. | Does not establish publication admission or overall accreditation. |
| FSE2 workflow status | Observed FOUND response after a real Gateway restart, with PostgreSQL correlation. | Specific validation workflow and observed event; not clinical completion. |
| FSE2 FHIR and publication | Offline implementations are included. | FHIR live validation remains unqualified after upstream 500 responses of undetermined cause; live document publication is not qualified. |

## Evaluation provenance

Current Core source is `2c2ff27`; the separately tested Windows package is `10a1300`.
The ordinary-account Windows Service observation uses Windows 10 Pro 22H2 x64
19045.6466 with Gateway disabled. It does not qualify a fresh current-source
package, portable restore or live Broker/Gateway continuity. Exact-source main CI
passed 22/22 jobs; no new provider or external-service qualification is asserted.
Two moderate development-tool dependency advisories remain deferred.
See [SOURCE.md](SOURCE.md) for exact commits, hashes and verification scope.

## Supported entry points

- [Evaluate SIP](docs/user/evaluation.md): separate Core and Windows delivery, integrity and recovery.
- [Core quickstart](docs/user/quickstart.md) and [local pilot](docs/user/local-pilot.md).
- [Local Broker](docs/user/local-broker.md): service delivery, local protection and application credential adoption.
- [Administration](docs/user/administration.md) and [guided onboarding](docs/user/guided-connector-onboarding.md).
- [FSE2 validation/status](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/user/fse2-validation-status.md) and [current specification](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/fse2/current-spec.md).
- [Azure provider](https://github.com/ApoCert-it/secure-integration-platform/blob/main/packs/deployment/azure/README.md) and [local PKCS#12 provider](https://github.com/ApoCert-it/secure-integration-platform/blob/main/packs/deployment/local-pkcs12/README.md).
- [CRA/NIS 2 adoption guidance](docs/security/cra-nis2-adoption.md).

## Boundaries

The software does not provide a universal secret-retrieval API to applications or
Admin. Vendor credentials remain server-side. Installation-local protection does
not hide plaintext returned to an authorized application, and Administrator/SYSTEM
remain privileged residual threats. A DPAPI blob alone is not portable key recovery.

Public source availability does not establish production readiness, certification,
accreditation, an SLA, complete regulatory conformity or signed build provenance.
Synthetic tests, controlled Windows observations and live-service observations remain
distinct. Private customer integrations and their evidence are not distributed here.
