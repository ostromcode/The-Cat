# The Cat – Non-monetary UTXO Cleanup

This repository contains the working draft of a Bitcoin Improvement Proposal (BIP) tentatively titled “Non-monetary UTXO Cleanup (The Cat)”.

It documents a soft-fork consensus change and new spending rules intended to remove an existing, snapshot-based set of non-monetary UTXOs (NMUs) created by protocols such as Ordinals and Stamps, by making those UTXOs permanently unspendable and eligible for removal from the UTXO set.

The BIP itself does **not** define any new relay or standardness policies for future transactions. Rather than restricting new transactions directly, The Cat aims to remove demand for such activity by eliminating the financial incentives for creating NMUs in the first place.

## Files

- [`bip-the-cat.md`](./bip-the-cat.md) – main BIP draft (specification, rationale, references)
- Additional notes, scripts, and data may be added over time.

This repository serves as the public discussion link referenced in the BIP header
and in any future pull request to the `bitcoin/bips` repository.

---

## Supporting stats and charts

See [`charts/`](./charts) for supporting statistics and visualizations that
illustrate the scale and structure of inscription-related UTXOs.

---

## Process note: mailing list moderation

The usual first step for a BIP is to circulate a detailed proposal on the Bitcoin
Development Mailing List and gather on-list technical feedback before requesting
a BIP number.

In December 2025, multiple attempts were made to post The Cat to the mailing list.
These messages were **blocked by moderation** and did not appear on the list,
preventing any on-list discussion of the proposal despite it being a fully worked draft.

In the author’s view, this sets a troubling precedent. Moderation should primarily
filter spam and clearly low-effort or off-topic content, not decide which substantive
technical proposals the wider community is allowed to see. When controversial ideas
are stopped at the moderation layer, it effectively puts a thumb on the scale of
Bitcoin’s governance by suppressing discussion rather than allowing the community
to evaluate and critique the ideas on their technical merits.

Because of this, this repository is being used as the primary venue for public review
and commentary on The Cat. Feedback, supportive or critical, is welcome here via issues,
pull requests, or external discussion that links back to this draft.
