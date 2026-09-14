# Changelog

## 14 Sep 2026 — Alpha evaluation source update

Updates the previous institutional snapshot `f89f50c` from development source
`b13e6ba` to exact source `2c2ff27`. See [SOURCE.md](SOURCE.md) for provenance.

- Local Broker: supported registration, inspection, executable update and revocation
  of a named application, plus a distinct .NET adopter sample and package checks.
  Local credential adoption and install/update preflight were already available.
- Evaluation: separate Core and Windows paths with integrity checks, prerequisites,
  Admin inspection and recovery. The tested Windows package remains `10a1300`;
  this source update publishes no new binary package.
- Admin: one searchable, paginated selector per onboarding choice, stable selected
  identifiers, corrected Installation context and readiness tied to Active enrollment.
  Search among 10,000 tenants is verified through Admin APIs and PostgreSQL, not
  a performance benchmark. Keyboard, narrow-screen and reload regressions are covered.
- Dependencies: `js-yaml` 4.3.2 addresses the identified high-severity advisory;
  two moderate development-tool advisories remain deferred.
- Existing FSE2 laboratory scripts supply the synthetic security-environment input
  required by shared Compose. Public FSE2/Azure/local PKCS#12 components are retained;
  no provider runtime or live qualification is added.

This remains alpha evaluation software with the limits in [the status](IMPLEMENTATION_STATUS.md).
Audit export and package preflight are retained capabilities, not new in this delta.
No tag, GitHub Release, binary asset or production/conformity claim accompanies it.

## 11 Sep 2026 — Initial institutional source snapshot

First curated ApoCert source distribution, based on the exact development revision
listed in [the original SOURCE.md](https://github.com/ApoCert-it/secure-integration-platform/blob/f89f50c37ddfb7671c885bf2fbb753974a467952/SOURCE.md). This entry summarizes the included software; it
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
