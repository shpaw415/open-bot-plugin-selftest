# open-bot-plugin-selftest

Disposable plugin used to verify the open-bot marketplace publish pipeline:
manifest validation, security review, R2 release storage, and GitHub issue
filing on rejected publishes.

- `v0.1.0` — benign content, passed review (test 1)
- `v0.2.0` — deliberately malicious skill body, expected to be rejected with a
  security issue filed against this repo. **Test 2 passed** on 2026-10-08: the
  reviewer rejected the publish and filed issue #1 with both findings rated
  high (credential exfiltration and deceptive prompt injection).
- `v0.3.0` — benign content restored, republished so the marketplace lists a
  clean version again.

Current version: **v0.3.0** — benign, performs no network access, reads no
vault keys, safe to remove.
