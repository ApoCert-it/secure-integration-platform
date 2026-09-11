# Changelog

## 11 Sep 2026 — Initial institutional source snapshot

First curated ApoCert source distribution, based on the exact development revision
listed in [SOURCE.md](https://github.com/ApoCert-it/secure-integration-platform/blob/main/SOURCE.md). This entry summarizes the included software; it
does not claim all components were newly implemented on this date.

- Windows Local Broker with authenticated IPC, installation-local protection,
  DPAPI/CNG key handling, service lifecycle and application credential adoption.
- Gateway with installation identity, operation grants, immutable Published
  configuration, restricted egress and separate provider capabilities.
- Admin UI/API with guided onboarding, distinct-role approval and bounded,
  tenant-scoped metadata-only audit export.
- Package install/update preflight binding the expected source commit and manifest
  hash before service stop or file replacement; no publisher-signature claim.
- Docker-first synthetic Core evaluation, .NET SDK and optional FSE2, Azure and
  local PKCS#12 packs.
- English architecture overview, operator/developer documentation, security model
  and CRA/NIS 2 adoption guidance with explicit responsibility and claim limits.

FSE2 offline coverage and specific OfficialTest observations remain distinct. FHIR
live validation and live document publication are not qualified. Production
readiness, universal Windows compatibility and overall regulatory conformity are
not claimed. No binary assets or product-version tag accompany this source snapshot.
