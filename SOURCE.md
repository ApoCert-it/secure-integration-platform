# Source provenance

## Snapshot published on 14 Sep 2026

This repository is the curated source distribution maintained by ApoCert S.r.l.
It has independent, linear Git history. Publication commits identify the corporate
publisher; they do not replace the authorship of the underlying contributions.
Original contribution history and DCO attestations remain in the development
repository. Licenses, copyright notices and third-party attribution are preserved.

The exact development baseline is
[`2c2ff275afefb52c02e7660ec80944bcaf3d44a3`](https://github.com/msala9/secure-integration-platform/commit/2c2ff275afefb52c02e7660ec80944bcaf3d44a3),
tree `d0e10e158f5762f85b50666e3a7503a6a6aa9cbf`, integrated through PR #79.
The previous institutional snapshot is
[`f89f50c37ddfb7671c885bf2fbb753974a467952`](https://github.com/ApoCert-it/secure-integration-platform/commit/f89f50c37ddfb7671c885bf2fbb753974a467952),
based on development commit `b13e6ba781a90d331836d37ec363baf27248737f`.

## Distribution inventory and boundaries

The distribution retains every previously published path and adds the seven new
Core source files selected by the qualified Core export. It includes the Core,
Windows Local Broker, SDK, Admin UI/API, synthetic evaluation tools and tests,
plus the previously published optional FSE2, Azure and local PKCS#12 components.
No additional pack is introduced. Optional components depend on Core contracts;
Core does not depend on them.

Private customer integrations, operational material, local evidence, development
history/branches, internal agent instructions and internal planning/review diaries
are excluded. `docs/internal/complexity-governance.md` remains excluded, as in the
previous institutional snapshot, although the upstream Core export includes it.
The upstream allowlist and original export metadata have not been changed.

[DISTRIBUTION_MANIFEST.json](DISTRIBUTION_MANIFEST.json) is the closed inventory for
this institutional distribution. It lists all 712 payload paths, byte lengths,
SHA-256 values of canonical Git blob contents and source/curation classification.
Only the manifest itself and its [SHA-256 sidecar](DISTRIBUTION_MANIFEST.json.sha256)
are excluded from that inventory. Checkout line endings may differ under
`.gitattributes`; the inventory describes committed contents, not generated output.

Runtime, SDK, tests, dependencies, build configuration and operational scripts
match the exact development baseline. Documentation retains the institutional
README, architecture illustration and navigation, with updated facts, public
traceability, this provenance record and the changelog. The original architecture
image is unchanged; no local untracked image is included.

## Core archive and Windows package provenance

The separately verified Core archive is
`sip-core-0.1.0-alpha.1-2c2ff275afef.zip`:

- Archive SHA-256: `C794AC3E10744FD0DCCEA7C88F342229A95E44EBD1B6D5AF055648C4BCB1B0C2`.
- Original manifest SHA-256: `4883E3952B2F0C4573E6932CBF538065296CCA04A06180CA8E5B3E1CD17FD3B9`.
- Original inventory: 534 source files plus four metadata files.

That archive and its unchanged manifest are distinct from this curated repository.
`Test-OpenSourceCoreInventory.ps1` verifies an extracted original Core export, not
the expanded institutional distribution. No binary or ZIP is uploaded by this update.

The existing Windows evaluation package remains tied to source
`10a13009c369249cd3c23cf1ab72623fcf1ae929`, not to a newly built package at `2c2ff27`.
Its archive SHA-256 is
`2CC06EA8846992FDC81937140AA1688B27A2F6D389EACF4BEA8FE6575D7BED77`;
package-manifest SHA-256 is
`A1D918402FE1EF6A02AF187DCF2898787FA3D31BCB86CB634D923DBD625B31C8`.
The observed ordinary-account Windows Service path on Windows 10 Pro 22H2 x64
19045.6466 covered registration, status, protection, verification, restart,
application executable update and revocation, with Gateway disabled. It does not
qualify live Broker/Gateway continuity, universal Windows compatibility or portable
machine/profile recovery. Historical observations retain their own source identities.

## Verification and limits

The exact source main passed 22/22 jobs without a final manual rerun:

- [General CI](https://github.com/msala9/secure-integration-platform/actions/runs/34854788553): 7/7.
- [M5/Admin CI](https://github.com/msala9/secure-integration-platform/actions/runs/34854788543): 15/15.

Publication checks cover the actual staged inventory, exact-source equality,
unchanged licensing and architecture image, Core/provider boundaries, documentation
links/anchors, secret scanning and whitespace. Existing exact-source CI is reused;
no new laboratory, SBOM or live provider/service qualification is claimed.
The two CI definitions are preserved because source-level tests read them.
GitHub Actions remains disabled on this distribution repository, as before;
there is no destination CI result to attribute to this snapshot.

The Admin search test uses the real HTTP pipeline and isolated PostgreSQL with
10,000 synthetic tenants. It proves bounded search, pagination and authorization
cases, not a production capacity benchmark or a 10,000-row browser test.
Two moderate development-tool dependency advisories remain deferred; this is not
a zero-vulnerability claim.

Historical live-matrix tools that update development review diaries must be run
from the development repository. They are not the supported Core quickstart or
Windows adoption commands. See [evaluation](docs/user/evaluation.md) for those paths.

This is an unsigned alpha evaluation source snapshot. It creates no tag, GitHub
Release, binary publication, stable-API promise, production qualification,
certification, accreditation or CRA/NIS 2 conformity claim. Hashes establish
integrity against an expected value, not publisher authenticity; DCO is not a
cryptographic signature. FSE2 and other live observations retain their existing limits.
