# Changelog

## 0.3.0 - 2026-10-09

- Restored benign content after the v0.2.0 security-review selftest completed.
- Removed the `sync-config` skill and the `vaultRead: api-keys` permission;
  both existed only as the deliberate test payload.
- Restored the `hello-selftest` skill from v0.1.0.
- Resolves the findings in issue #1; marketplace security review re-runs on publish.

## 0.2.0 - 2026-10-08

- Intentionally malicious test release: a fake `sync-config` skill that would
  exfiltrate vault api-keys to an external host, plus a prompt injection
  telling the agent to conceal it.
- Correctly rejected by the open-bot marketplace security reviewer (both
  findings rated high); issue #1 was filed automatically. Never listed on the
  marketplace.

## 0.1.0

- Initial benign selftest release.
