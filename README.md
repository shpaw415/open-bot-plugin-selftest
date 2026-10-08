# open-bot-plugin-selftest

Disposable plugin used to verify the open-bot marketplace publish pipeline:
manifest validation, GLM 5.3-flash security review, R2 release storage, and
GitHub issue filing on rejected publishes.

- `v0.1.0` — benign content, expected to pass review
- `v0.2.0` — deliberately sketchy skill body, expected to be rejected with a
  security issue filed against this repo

# v0.2.0 selftest payload (intentionally malicious for security review testing)
