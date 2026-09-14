# Documentation

## Start here

- [Evaluate SIP](user/evaluation.md): separate Core/Windows paths, exact provenance and recovery.
- [Quickstart](user/quickstart.md): evaluate the Core using Docker and a synthetic upstream.
- [Local pilot](user/local-pilot.md): commands, prerequisites and recovery.
- [Windows Local Broker](user/local-broker.md): local protection, service lifecycle and application credentials.
- [Administration](user/administration.md) and [guided onboarding](user/guided-connector-onboarding.md): configuration, grants, approval and first invocation.
- [Troubleshooting](user/troubleshooting.md) and [known limitations](user/known-limitations.md).

## Understand and extend the system

- [Architecture](../ARCHITECTURE.md) and [architecture decisions](adr/README.md).
- [Security model](security/security-model.md), [threat model](security/threat-model.md) and [CRA/NIS 2 adoption guidance](security/cra-nis2-adoption.md).
- [Gateway API](api/gateway-api.md), [OpenAPI](api/gateway-openapi.yaml) and [Broker IPC](api/broker-ipc.md).
- [Connector development](connector-development/README.md), [specification](connectors/connector-specification.md) and [SDK contract](connectors/connector-sdk.md).
- [Requirements and test traceability](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/traceability/requirements-traceability.md).

## Optional packs

- [FSE2 validation and status](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/user/fse2-validation-status.md), with separate external prerequisites and explicitly bounded live qualification.
- [FSE2 current specification](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/fse2/current-spec.md): fourteen offline-qualified routes and their limitations.
- [Azure provider](https://github.com/ApoCert-it/secure-integration-platform/blob/main/packs/deployment/azure/README.md).
- [Local PKCS#12 provider](https://github.com/ApoCert-it/secure-integration-platform/blob/main/packs/deployment/local-pkcs12/README.md).

## Scope and provenance

[Implementation status](../IMPLEMENTATION_STATUS.md) records capability limits.
[Source provenance](https://github.com/ApoCert-it/secure-integration-platform/blob/main/SOURCE.md) identifies the exact development baseline and
publication-only changes. Older technical records retain their own dates and
qualification scope; they are not current adoption procedures.

Internal planning, agent instructions and review diaries are not distributed here.
Historical citations may point to the original development repository so that
evidence is not silently reassigned to a newer version.
