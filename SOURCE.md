# Source provenance

## Snapshot published on 11 Sep 2026

This repository is the curated source distribution maintained by ApoCert S.r.l.
It has independent Git history: publication commits represent source snapshots,
not the authorship of all underlying code.

The development baseline is
[`b13e6ba781a90d331836d37ec363baf27248737f`](https://github.com/msala9/secure-integration-platform/commit/b13e6ba781a90d331836d37ec363baf27248737f),
tree `bb7115056de5b0b8feaa53f09b7f03170b7cfc85`.
Original contribution history and DCO attestations remain in that repository.
Licenses, copyright notices and third-party attribution are preserved.

## Included and excluded

The snapshot includes the public Core, Windows Local Broker, SDK, Admin UI/API,
synthetic evaluation tools, tests and the optional FSE2, Azure and local PKCS#12
packs. Private customer-specific integrations and operational material are excluded.
Development branches, internal agent instructions, planning/review diaries and
development CI workflows are not copied.

Runtime source, SDK, tests, dependency lock files and build configuration are
unchanged from the development baseline. Publication-only edits consist of the
architecture illustration, README and documentation navigation, publication status,
contribution instructions, this provenance record and the changelog. Historical
references retain their original qualification scope.

## Verification

The unchanged development baseline passed:

- [General CI](https://github.com/msala9/secure-integration-platform/actions/runs/34505053638): 7/7 jobs.
- [M5/Admin CI](https://github.com/msala9/secure-integration-platform/actions/runs/34505053656): 15/15 jobs.

Publication checks cover the actual distributed file inventory, source equality,
licenses, secret scanning, documentation links and whitespace. These checks do not
constitute a fresh run of every platform, cloud or live-service test on this
repository. Removing development history is not a new functional qualification.

This is a source technical preview, not a signed binary release or a production,
certification, accreditation or CRA/NIS 2 conformity claim. Current API/package
versions are preserved; no new product-version tag is created by this snapshot.
