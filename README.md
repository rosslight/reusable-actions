# reusable-actions

This repository is a collection of reusable actions which are used by rosslight GmbH.

Pushing a commit which follows semantic commits triggers a new release, automatically.

## SBOM license policy

`sbom-check` uses its bundled `license-policy.json` by default, including SQLite's
`blessing` identifier and `LicenseRef-rosslight-Internal-1.0`. It rejects licenses
outside the allowlist, licenses requiring review, and undeclared licenses.

Callers can supply `license_policy_path` to use a policy file from their checkout.
Package-specific SPDX declarations still belong in `additional_sbom_info_path`.
