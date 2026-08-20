# Tokenia — End User Licence Agreement

**Licensor:** Mykhailo Laskavyi
**Contact:** support@tokenia.dev

This agreement is between you and the Licensor, and governs your use of the
Tokenia application. Installing or using Tokenia means you accept it.

The **source code** is not covered here and is not distributed. Access to it
grants no right to use, copy, or redistribute it — see "Source code" below.

---

## 1. Trial

Tokenia may be used free of charge for an evaluation period of **7 days**
from first launch, with no restriction on functionality during that period.
No payment details, account, or email address are required to start the
trial.

The trial is per person, not per installation. Reinstalling, using a
different machine, or clearing application data does not start a new trial,
and circumventing the trial period is a breach of this agreement.

When the trial ends, Tokenia stops displaying usage-limit data until a
licence is activated. It does not disable, modify, or interfere with Claude Code, and it
releases `ANTHROPIC_BASE_URL` cleanly on uninstall — an expired trial must
never leave your development environment in a broken state.

## 2. Lifetime licence

A paid licence costs **$9.99 (USD), once**, and grants you a **perpetual,
non-exclusive, non-transferable** right to use Tokenia for as long as you
wish on **one Mac at a time**.

The price is inclusive of VAT and sales tax. Purchases are processed by
**Lemon Squeezy**, which acts as merchant of record and is the seller for
tax purposes.

"Lifetime" refers to the lifetime of the product, not of the purchaser. It
means:

- **No recurring fee.** You pay once.
- **All future updates** to Tokenia are included at no additional cost.
- If the product is discontinued, your existing installation keeps working.
  The Licensor undertakes to publish a release that removes the licence check
  before shutting down licence validation, so a purchased copy never becomes
  unusable because a server went away.

**Moving to another Mac.** A licence is bound to one machine at a time, not
to one machine forever. Tokenia provides a **"Deactivate this device"**
button that releases the licence immediately, after which the same key
activates on another Mac. If the original machine is lost, stolen, or no
longer starts, contact the Licensor and the activation will be cleared
manually — you will not be left without the software you paid for.

## 3. What the licence does not permit

You may not:

- redistribute, resell, rent, lease, or sublicense Tokenia or any part of it;
- share your licence key, or use one key for more than one person;
- remove, disable, or circumvent the licence check;
- reverse engineer, decompile, or disassemble the software, except where
  applicable law expressly forbids that restriction.

## 4. Licence keys and validation

A validation request carries **only** the licence key, an opaque machine
identifier, and the application version. It carries no usage data, no
usage-limit figures, no credentials, and no content of any kind — see
[PRIVACY.md](PRIVACY.md).

The machine identifier is a salted one-way hash computed on your device. The
Licensor never receives a hardware serial number, a MAC address, or any
identifier that could be linked back to you or to another product.

Activation and validation are served from **Supabase** infrastructure
operated by the Licensor.

Validation is cached locally and Tokenia remains fully functional while
offline. A network outage on either side must never cost you access to
software you have paid for.

## 5. Updates and support

Updates are provided at the Licensor's discretion and are included in the
licence fee. No specific update, feature, or response time is promised.

Tokenia depends on undocumented Anthropic response headers to read the usage
limit. If Anthropic changes or removes them, Tokenia may stop showing
usage-limit data through no fault of the Licensor. This is a known and disclosed risk, and is
not grounds for a refund outside the period in §6.

## 6. Refunds

Full refund on request within **14 days** of purchase, no justification
required. The trial exists so that you can determine whether the product
works for you before paying; the refund window is a backstop, not the
primary evaluation route.

## 7. Termination

This licence terminates automatically if you breach §3. On termination you
must stop using Tokenia and uninstall it. Sections 4, "Privacy" (see
[PRIVACY.md](PRIVACY.md)), 8, and 9 survive termination.

## 8. Warranty and liability

Tokenia is provided **"as is"**, without warranty of any kind, express or
implied, including but not limited to warranties of merchantability, fitness
for a particular purpose, and non-infringement.

To the maximum extent permitted by law, the Licensor's total liability under
this agreement is limited to the amount you paid for the licence. The
Licensor is not liable for indirect, incidental, or consequential damages,
including lost work or lost profits.

Nothing in this agreement limits liability that cannot be limited by law,
including liability for fraud, or your statutory consumer rights.

## 9. Governing law

This agreement is governed by the laws of Norway, without regard to its
conflict-of-laws principles. Nothing in this section limits a consumer's
statutory rights under the mandatory law of their country of residence.

## 10. Changes to these terms

The Licensor may change these terms for future purchases. **Changes do not
apply retroactively to a licence already purchased** — the terms you bought
under are the terms you keep.

---

## Source code

Tokenia's source is proprietary. No licence is granted by this document, and
none is implied by anything in this repository. In particular, no permission
is given to use, copy, modify, merge, publish, distribute, sublicense, sell,
or create derivative works of the software, in whole or in part, except
under a separate written licence granted by the copyright holder.

Copyright (c) 2026 Mykhailo Laskavyi. All rights reserved.
