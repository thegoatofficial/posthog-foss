---
upstream: https://github.com/PostHog/posthog-foss
kind: commit
pinned: 2026-10-04
pinned_commit: 8998e44ef3ecce4f5b4d21bd8c7361b1515f7fe7
licence: MIT
licence_file: LICENSE
fork: true
fork_url: https://github.com/thegoatofficial/posthog-foss
reviewed: 2026-10-04
intake_status: incomplete
intake_covers_pinned_checkout: false
---

# PostHog FOSS upstream fork

The DreamWild founder requested an official upstream fork and selected PostHog
Cloud for the running service on 4 October 2026. This repository retains the full
official FOSS source. DreamWild integrates the official SDKs with PostHog Cloud;
it does not run this checkout as a production service.

The root LICENSE is MIT, copyright PostHog Inc. 2020-2026. The official FOSS tree
contains no `ee` directory. The main PostHog repository has separate enterprise
terms; those terms and that code are not represented as MIT by this fork.

The upstream HEAD was rechecked on 4 October 2026 and matched the immutable pin
above. Our only addition at this point is this provenance record. The freshness
checker's commit mode uses the date in `pinned`; `pinned_commit` identifies the
exact source. Its default discovery does not include the third-party directory.

## Intake coverage

The initial bounded scan overlapped checkout completion and is incomplete. It
inventoried 5,662 files, reported truncation and snapshot changes, and did not
cover the final 55,464 tracked files. Its 19 secret-detector findings were
reviewed without reproducing values: 17 fixture/example contexts, one public
local OAuth client identifier and one tokenizer checksum. No suspicious
production-secret context was identified; no credential validity was tested.

This is provenance and a scoped intake record, not execution clearance or a
claim that the upstream application has no vulnerabilities. No code from this
checkout was executed during DreamWild setup. The original LICENSE remains
alongside this record.
