# Tokenia — Privacy Policy

This is a commitment, not a description of current intent, and it survives
any change of ownership of the product.

Tokenia is a local proxy. It sees your Claude Code traffic because that is
the only way to read the rate-limit headers Anthropic returns. Given that:

- **Request and response bodies are never logged, stored, or transmitted.**
  They are relayed and forgotten.
- **The `Authorization` header is never logged.** It is forwarded to
  `api.anthropic.com` and forgotten.
- Only parsed numbers are retained — utilisation, status, and reset times —
  and only on your own machine.
- Nothing is sent anywhere except `api.anthropic.com` and, for licence
  validation only, the Licensor's validation endpoint (see below).
- The process that handles your traffic and your credentials is separate
  from the one that validates licences, and has no network path to the
  Licensor at all.

Adding telemetry, analytics, or crash reporting that carries any part of
your traffic would breach this policy.

## Licence validation

If you activate a paid licence, Tokenia sends a validation request
containing **only**: the licence key, an opaque machine identifier, and the
application version. It carries no usage data, no quota figures, no
credentials, and no content of any kind.

The machine identifier is a salted one-way hash computed on your device. The
Licensor never receives a hardware serial number, a MAC address, or any
identifier that could be linked back to you or to another product.

Activation and validation are served from **Supabase** infrastructure
operated by the Licensor.

Validation is cached locally, so Tokenia keeps working while offline.

## Purchases

Purchases are processed by **Lemon Squeezy**, which acts as merchant of
record and handles payment details, invoicing, and refunds. The Licensor
does not receive or store your card details.

## Contact

Questions about this policy: support@tokenia.dev.

## Proof, not just a promise

A test in Tokenia's build asserts that no logging path can emit body or
credential content, so this is enforced by the build rather than promised by
a page.

## Changes

This policy may be updated. Material changes will be posted in this
repository's [Discussions](../../discussions).
