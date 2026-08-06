# Licence Terms, Refund Policy, Privacy

*(Category: General — pin this after posting.)*

This is the plain-language version of [LICENSE.md](../LICENSE.md) and
[PRIVACY.md](../PRIVACY.md). Read those two for the actual terms; this post
exists so you don't have to.

## Free vs. paid

Tokenia is free to try for **5 days**, full functionality, no account and no
payment details required to start. After that, a licence is **$9.99 once** —
not a subscription. That covers the current version and every future update;
if the product is ever discontinued, the licence check gets removed in a
final release so your copy keeps working.

## Refunds

**14 days, no questions asked.** The trial is meant to answer "does this
work for me" before you pay, so the refund window is a backstop, not the
main way to evaluate it.

## One Mac at a time, not one Mac forever

A licence is tied to a single Mac, but you can move it: the app has a
"Deactivate this device" button that frees the key immediately for another
machine. Lost or dead Mac and can't deactivate first? Email
support@tokenia.dev and it'll be cleared manually.

## Privacy

Tokenia is a local proxy sitting between Claude Code and Anthropic — it sees
your OAuth token and the full text of every conversation, because that's the
only way to read the usage-limit headers. So, as a hard rule:

- Request/response bodies are never logged or stored — relayed and
  forgotten.
- The `Authorization` header is never logged.
- Only numbers are kept: utilisation, status, reset times — locally, on your
  machine.
- Nothing leaves your machine except calls to `api.anthropic.com` (exactly
  what Claude Code would have sent anyway) and, only if you activate a
  licence, a validation request containing the licence key, a salted
  per-device hash, and the app version — no traffic, no credentials.

A build-time test asserts no logging path can emit body or credential
content, so this isn't just a promise on a page.

## Questions

Ask below — licensing, refunds, privacy, whatever's unclear. General bugs
and feature requests belong in their own Discussions categories or Issues,
not this thread.
