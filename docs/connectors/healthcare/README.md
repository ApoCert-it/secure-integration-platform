# Healthcare connector characterization

This optional pack directory contains public-safe characterization, the Wave 1 Regional
ePrescription foundation and the FSE2 Organization integration. The Core does not depend
on Healthcare. No production qualification or overall certification is claimed.

## Package contents

- [FSE2 Organization](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/fse2/README.md): [current validation/status pilot](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/user/fse2-validation-status.md),
  [frozen offline route contract](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/fse2/current-spec.md) and historical profile references.
  The [capability summary](../../../IMPLEMENTATION_STATUS.md#product-status) owns current status.
- [Complete integration inventory](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/integration-inventory.md)
- [Protocol matrix](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/protocol-matrix.md)
- [Execution-location matrix](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/execution-location-matrix.md)
- [Minimal authentication primitives](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/auth-primitives-required.md)
- [Clean-implementation provenance](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/provenance.md)
- [Historical implementation waves and GO/NO-GO](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/M6-IMPLEMENTATION-PLAN.md)
- [Regional ePrescription Wave 1 foundation](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/regional-eprescription/README.md)
- Connector specifications:
  - [SOGEI Basic + session](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/sogei-basic-session/spec.md)
  - [Lombardia OAuth helper](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/lombardia-oauth-helper/spec.md)
  - [FVG PKCE + JWT](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/fvg-pkce-jwt/spec.md)
  - [Umbria mTLS + dual JWT](https://github.com/ApoCert-it/secure-integration-platform/blob/main/docs/connectors/healthcare/umbria-mtls-jwt/spec.md)
- Synthetic vectors: `tests/characterization/healthcare`

`KNOWN` is a historical characterization label, not current official or live-verified evidence. Each production profile remains `NEEDS_PUBLIC_SOURCE` and NO-GO until its unresolved questions are closed with current official provenance.
