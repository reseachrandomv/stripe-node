---
title: Reject malformed webhook v1 signatures with StripeSignatureVerificationError
semver_level: patch
---

- `constructEvent` raises `StripeSignatureVerificationError` when a `v1` value in the `Stripe-Signature` header is empty or encodes to a different number of bytes than the expected signature.
